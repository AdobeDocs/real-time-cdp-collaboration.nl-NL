---
title: AWS-machtigingen voor audiobronnen configureren
description: Leer hoe te om de toestemmingen van het Beheer van de Identiteit en van de Toegang van AWS te vormen (IAM) om veilige, read-only toegang van Adobe tot uw  [!DNL Amazon S3]  emmer voor publieksbron in Real-Time CDP Collaboration te verlenen.
source-git-commit: 4f223890dabb4897c9e9264655ff9217e323dc91
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# AWS-machtigingen configureren voor publiekssourcing

Gebruik deze gids om het beleid en de rollen van het Beheer van de Identiteit en van de Toegang van AWS te vormen (IAM) die Adobe veilige, read-only toegang tot uw Amazon S3 emmertje verlenen. Deze toegang laat Real-Time CDP Collaboration toe om publiek van uw S3 emmertje te bron.

## Vereisten {#prerequisites}

Bevestig voordat u doorgaat dat u aan de volgende vereisten voldoet en toegang hebt tot de vereiste informatie.

### Vereiste AWS-machtigingen

Om deze instelling te voltooien, moet uw account toegang hebben tot AWS-beheerders. De toegang van de beheerder zorgt ervoor dat u het beleid en de rollen van IAM kunt tot stand brengen en beheren die worden vereist om Adobe toegang tot uw S3 emmertje te verlenen. Als u geen beheerdersrechten hebt, neemt u contact op met uw AWS-beheerder voordat u verdergaat.

### Vereiste informatie

Houd de volgende informatie bij het doorlopen van de onderstaande stappen. Deze details worden gebruikt in de [[!DNL Amazon S3]  publiek bronende gids UI &#x200B;](./configure-aws-s3-audience-sourcing.md).

* De S3 emmer naam waar uw publieksdossiers worden opgeslagen.
* Het mappad (voorvoegsel) waaronder de publieksbestanden zich bevinden.
* De Amazon Resource Name (ARN) voor uw nieuwe IAM-rol, bijvoorbeeld: `arn:aws:s3:::my-company-data/audience-files/`

>[!TIP]
>
>Een Amazon Resource Name (ARN) identificeert uniek de middelen van AWS, zoals S3 emmers en IAM rollen. Gebruik de volgende indeling om uw emmertje en het optionele mappad op te geven:
>
>```
>arn:aws:s3:::<bucket-name>/<optional-folder-path>
>```

## Een IAM-beleid maken {#create-policy}

Om met de opstelling te beginnen, creeer eerst een beleid IAM dat **read-only toegang** aan uw S3 emmertje verleent. Met dit beleid kan Adobe de bestanden lezen die nodig zijn voor het zoeken naar een publiek, maar dit beleid staat schrijven of verwijderen niet toe.

Open de [&#x200B; Console van het Beheer van AWS &#x200B;](https://aws.amazon.com/console/), en navigeer aan **[!DNL IAM]** > **[!DNL Policies]** > **[!DNL Create policy]**.

In AWS creeer beleidswerkruimte, selecteer het **JSON** lusje en kleef het volgende voorbeeldbeleid.

>[!NOTE]
>
>Vervang `<Your AWS ARN for bucket folder path>` en `<Your AWS ARN for bucket>` door uw specifieke S3 ARNs. Wanneer u het pad van de emmermap opgeeft, neemt u `/*` op aan het einde van de ARN (bijvoorbeeld `arn:aws:s3:::my-company-data/audience-files/*` ). Dit zorgt ervoor dat Adobe toegang heeft tot alle bestanden en submappen binnen het opgegeven mappad.

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Statement1",
      "Effect": "Allow",
      "Action": [
        "s3:GetObject",
        "s3:ListBucket",
        "s3:GetBucketLocation"
      ],
      "Resource": "<Your AWS ARN for bucket folder path>"
    },
    {
      "Sid": "Statement2",
      "Effect": "Allow",
      "Action": [
        "s3:ListBucket"
      ],
      "Resource": "<Your AWS ARN for bucket>"
    }
  ]
}
```

Controleer de beleidsinstellingen en selecteer **[!DNL Create policy]** . Neem de naam van het beleid voor gebruik op in een latere stap.

>[!TIP]
>
>Om van uw emmer naam en omslagweg de plaats te bepalen, open de **Console van het Beheer van Amazon S3**. Voor de **pagina van emmers**, selecteer uw emmer naam om het te openen. De **mening van Objecten** maakt een lijst van uw dossiers en omslagen, en de weg bij de bovenkant van de pagina toont uw huidige omslagweg.

## Een IAM-rol maken {#create-role}

Daarna, creeer een rol IAM en plaats de rol van Real-Time CDP Collaboration AWS IAM als **vertrouwde op entiteit**. Dit laat de diensten van Adobe toe om de rol te nemen en veilig uw S3 publieksgegevens te lezen.

Navigeer op het tabblad **[!DNL IAM]** van de Amazon S3 Management Console naar **[!DNL Roles]** > **[!DNL Create role]** .

Selecteer onder [!DNL Step 1] van de [!DNL Create role] -workflow in de **[!DNL Trusted entity type]** -sectie **[!DNL Custom trust policy]** . Plak vervolgens in de **[!DNL Custom trust policy]** -editor het volgende voorbeeld en vervang `<Adobe IAM Role ARN>` door de waarde voor het gebied.

* De juiste Adobe IAM Role ARN voor uw regio:

| Regio | Adobe IAM Role ARN |
|---------|-------------------|
| Noord-Amerika | `arn:aws:iam::590183896800:role/rtcdp-collab-prod-va6-role` |
| Australië | `arn:aws:iam::590183896800:role/rtcdp-collab-prod-aus3-role` |

Een voorbeeld van een vertrouwensbeleid:

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "Statement1",
      "Effect": "Allow",
      "Principal": {
        "AWS": "<Adobe IAM Role ARN>"
      },
      "Action": "sts:AssumeRole"
    }
  ]
}
```

Herzie het beleid en selecteer **daarna** om verder te gaan.

In [!DNL Step 2] **[!DNL Add permissions]** sectie van het [!DNL Create role] werkschema, onderzoek naar en maak het beleid IAM vast u [&#x200B; vroeger &#x200B;](#create-policy) creeerde. Selecteer het beleid dat wordt gevolgd door **[!DNL Next]** om door te gaan naar [!DNL Step 3] .

Geef in de sectie [!DNL Step 3] **[!DNL Name review, and create - Role details]** een rolnaam (bijvoorbeeld `s3-iam-role` ) en een optionele beschrijving op.

Op deze pagina worden het beleid voor vertrouwde entiteiten, de samenvatting van het beleid voor machtigingen en alle tags weergegeven die u hebt toegevoegd voor interne organisatie en tracering.

Tot slot selecteer **creeer rol** om de opstelling te bevestigen.

>[!IMPORTANT]
>
>U moet de naam van het Middel van Amazon (ARN) registreren nadat het creëren van de rol. U zult IAM ARN van de Rol tijdens **moeten verstrekken verifieert uw S3 verbinding** stap in [&#x200B; AWS S3 voor publiek dat &#x200B;](./configure-aws-s3-audience-sourcing.md) werkschema aankomt vormt.

## Volgende stappen {#next-steps}

Deze opstelling verleent Adobe read-only toegang tot uw S3 emmertje en vestigt een vertrouwde op verbinding met Adobe IAM rol.

Daarna, ga aan [&#x200B; te werk vormen AWS S3 voor publiek die &#x200B;](./configure-aws-s3-audience-sourcing.md) aantrekken om uw S3 emmertje aan Collaboration te verbinden.

Voor meer informatie over het betrekken van publiek, verwijs naar [&#x200B; Source en beheer publiek &#x200B;](./onboard-audiences.md).
