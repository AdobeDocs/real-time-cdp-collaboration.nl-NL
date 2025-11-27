---
title: Vorm  [!DNL Amazon S3]  voor de Bron van het Publiek
description: Leer hoe te om uw  [!DNL Amazon S3]  opslag als zelfbediening gegevensbron te vormen en te verbinden om publieksgegevens in Real-Time CDP Collaboration in te voeren.
source-git-commit: 7a2bfb524d77d42690f3abe848a59aae5b16b667
workflow-type: tm+mt
source-wordcount: '1513'
ht-degree: 0%

---

# [!DNL Amazon S3] configureren voor publiekssourcing

Leer hoe u de [!DNL Amazon S3] -opslag in de gebruikersinterface van Adobe Real-Time CDP Collaboration configureert en koppelt aan brongegevens voor activering en overlappende analyse.

>[!IMPORTANT]
>
>Voordat u deze handleiding kunt volgen, moet u de stappen voor het autoriseren van de Adobe IAM-rol binnen uw AWS-account hebben voltooid.\
>Zie **[vormen de toestemmingen van AWS voor publiek die](./configure-aws-permissions-audience-sourcing.md)** gids voor geleidelijke opstellingsinstructies opzoeken.

## Overzicht {#overview}

Met deze workflow kunt u soorten publiek van eerste bedrijven rechtstreeks vanuit [!DNL Amazon S3] aanschaffen en beheren. Na configuratie, produceert Collaboration automatisch publiek van uw S3 emmertje en stelt hen ter beschikking voor inzichten en activering.

Voor soorten publiek die via S3 worden aangekocht, gelden dezelfde regels inzake governance en gegevensverwerking als voor het publiek uit Adobe Experience Platform.

## Vereisten {#prerequisites}

Controleer voordat u de S3-gegevensverbinding configureert het volgende:

* U hebt toegang tot een actieve **[!DNL Amazon S3]emmer** bevattende publieksdossiers die aan de **[Specificatie van de Bron van de Publiek (v1.1)](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.1.pdf)** in overeenstemming zijn.
* U hebt een **rol IAM** in AWS gecreeerd die de toestemming van Adobe verleent om tot uw emmer toegang te hebben gebruikend de **veronderstelde rol** methode (niet toegang/geheime sleutels). Zie **[de toestemmingen van AWS voor publieksbron](./configure-aws-permissions-audience-sourcing.md)** voor gedetailleerde instructies vormen. De rol IAM moet de volgende toestemmingen omvatten:

   * `ListBucket`
   * `GetBucketLocation`
   * `GetObject`

* U kunt de volgende waarden gebruiken:

   * **IAM de naam van het Middel van de rolAmazon (ARN)**
   * **S3 emmernaam**
   * **weg van de Omslag** (de folderprefix die uw publieksdossiers bevatten)

>[!NOTE]
>
>De dossiers van het publiek moeten in de **weg van de wortelomslag** van uw gemachtigd S3 emmertje worden gevestigd. Submappenstructuren worden niet ondersteund.

## Uw [!DNL Amazon S3] verbinding configureren {#configure-aws-s3-connection}

Van het **[!UICONTROL My audiences]** lusje binnen de **[!UICONTROL Setup]** werkruimte, selecteer het add pictogram (![&#x200B; voeg pictogram toe.](/help/assets/icons/plus.png) ) en selecteer vervolgens **[!UICONTROL Audience]** .

Als dit uw eerste publiek is, kunt u ook de optie **[!UICONTROL Add]** selecteren.

![&#x200B; Mijn publiek tabel in de werkruimte van de Opstelling met toevoegen pictogram en voegt getoonde publieksoptie toe.](../../assets/setup/add-manage-audiences/add-audiences.png)

De workflow voor het toevoegen van publiek wordt weergegeven. Selecteer **[!UICONTROL Add a new data connection]** en selecteer vervolgens **[!UICONTROL Next]** .

![&#x200B; Add publiek werkruimte met Add een nieuwe benadrukte optie van de gegevensverbinding.](../../assets/setup/add-manage-audiences/add-data-connection.png){zoomable="yes"}

### [!DNL Amazon S3] selecteren als gegevensverbinding {#select-aws-s3}

Selecteer **[!UICONTROL Amazon S3]** als gegevensverbinding, gevolgd door **[!UICONTROL Next]** .

![&#x200B; het selectiescherm van de gegevensverbinding met [!DNL Amazon S3] beschikbaar als selecteerbare optie.](../../assets/setup/aws-audience-sourcing/select-s3-data-connection.png)

### Vereisten voor het bestand van het publiek bekijken {#review-audience-requirements}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_audience_sourcing_specifications"
>title="Uw gegevens voorbereiden voor instaptoegang"
>abstract="Lees de handleiding Audience Sourcing Specification voor het opmaken en structureren van publieksgegevens van Amazon S3 voor Collaboration."
>additional-url="https://www.adobe.com/go/rtcdp-collaboration-audience-sourcing" text="Zie de handleiding"

Er wordt een dialoogvenster weergegeven waarin wordt uitgelegd hoe uw publieksbestanden moeten worden gestructureerd. Gebruik de koppeling naar de **[[!UICONTROL Audience Sourcing Specification]](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.1.pdf)** voor informatie over het opmaken en structureren van publieksgegevens in [!DNL Amazon S3] voor Collaboration, zodat deze correct worden gelezen.

>[!IMPORTANT]
>
>U moet Adobe als [!DNL Amazon S3] -gebruiker hebben geautoriseerd, zodat Adobe gegevens van uw [!DNL Amazon S3] -opslagruimte kan ophalen voor verwerking.

Uw publieksbestanden moeten voldoen aan de specificaties voor Audience Sourcing. De sleutels van de gelijke worden automatisch in kaart gebracht gebaseerd op het vereiste formaat.

Belangrijkste overwegingen zijn:

* De dossiers moeten in formaat CSV zijn, gebruikend komma&#39;s als afbakening en pijpleidingen (`|`) voor veelvoudige waarden.
* Als u meerdere bestanden uploadt, moet u ervoor zorgen dat alle bestanden identieke kolommen bevatten.
* Elke publieksrecord moet een `AUDIENCE_ID` en ten minste een overeenkomende toets bevatten, zoals `HASHED_EMAIL_SHA_256` , `HASHED_PHONE_SHA_256` , `HASHED_IPV4_SHA_256` , `CRM_ID` , `LOYALTY_ID` of `ADFIXUS_ID` .
* De gegevens worden elke 1 tot 6 dagen vernieuwd op basis van uw keuze tijdens de installatie van de bron in Collaboration.

![&#x200B; Bereid Uw Gegevens voor om dialoog met een verbinding aan de Specificaties van de Bron van het Publiek te bron.](../../assets/setup/aws-audience-sourcing/prepare-data-sourcing-dialog.png)

### Verifieer uw S3 verbinding {#authenticate-s3-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_sources_s3_folderpath"
>title="Padindeling van map"
>abstract="Voer het mappad (voorvoegsel) in het [!DNL Amazon S3] -emmertje in waar de bestanden voor uw publiek zijn opgeslagen. <br><ul><li>Begin geen wegen met een voorwaartse schuine streep (/).</li><li>Voeg een slash aan het einde van het pad in.</li><ul><br> Geldig voorbeeld: `base/path/`<br> Ongeldig voorbeeld: `/base/path`"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_audience_sharing_amazon_s3"
>title="publiek toevoegen voor Amazon S3"
>abstract="Als u verbinding wilt maken met uw Amazon S3-opslag, moet u de Adobe-servicegebruiker machtigen om uw publieksgegevens op te halen voor verwerking. Volg de stappen in Experience League om Adobe toegang te verlenen tot uw Amazon S3-opslag."

Geef vervolgens uw [!DNL Amazon S3] -gegevens op om uw S3-emmertje aan te sluiten op Collaboration.

Volg de stappen die in **[worden geschetst vormen de toestemmingen van AWS voor publiek die](./configure-aws-permissions-audience-sourcing.md)** aantrekken om de toegang van Adobe tot uw te verlenen
[!DNL Amazon S3] -opslag. Voer de waarden in de volgende UI-velden in nadat deze zijn voltooid:

* IAM-rol
* S3 Emmernaam
* Mappad

![&#x200B; de [!DNL Amazon S3] verbindingsvorm met gebieden voor rol IAM, de Naam van het Emmertje S3, en de Weg van de Omslag.](../../assets/setup/aws-audience-sourcing/s3-authentication-credentials-form.png)

### Bevestig bevestiging van toestemming {#confirm-consent}

U moet dan erkennen dat de opt-outs voor toestemming zijn geschrapt alvorens te werk te gaan. Schakel het bevestigingsvak, gevolgd door **[!UICONTROL OK]** , in om te bevestigen.

![&#x200B; de dialoog van de toestemmings opt-out erkenning die bevestiging vereist alvorens te werk te gaan.](../../assets/setup/aws-audience-sourcing/consent-optout-acknowledgment.png)

### Verificatieresultaten valideren {#validate-authentication}

Na het verbinden, bevestigt het systeem uw geloofsbrieven en toont één van de volgende berichten:

| Status | Bericht | Beschrijving |
|---| ---|---|
| **Succes** | **[!UICONTROL Authentication successful]** | Uw verbinding met [!DNL Amazon S3] is tot stand gebracht. |
| **Ontbroken** | **[!UICONTROL Authentication failed]** | Controleer uw gegevens en probeer het opnieuw. |
| **Ontkende Toegang** | **[!UICONTROL Access denied]** | Uw referenties hebben niet de vereiste machtigingen om toegang te krijgen tot dit [!DNL Amazon S3] emmertje. Controleer de toegangsinstellingen of neem contact op met de beheerder. |
| **Ongeldig dossierformaat** | **[!UICONTROL Invalid file format]** | De publieksgegevens komen niet overeen met de verwachte structuur. Controleer of uw bestanden voldoen aan de specificaties voor Audience Sourcing. |
| **Geen publieksdossiers gevonden** | **[!UICONTROL No audience files found]** | Bevestig dat de bestanden voor uw publiek aanwezig zijn in het opgegeven mappad en dat het pad toegankelijk is. |
| **Interne fout** | **[!UICONTROL An internal error has occurred]** | Probeer het opnieuw. Neem contact op met de klantenondersteuning als het probleem zich blijft voordoen. |


### Verbindingsgegevens opgeven {#provide-connection-details}

Voer een beschrijvende naam en een optionele beschrijving in voor uw S3-gegevensverbinding. Voer uw waarden in de volgende UI-velden in:

* **[!UICONTROL Data connection name]** (vereist)
* **[!UICONTROL Data connection description]** (optioneel)

![&#x200B; de details van de gegevensverbinding met gebieden voor verbindingsnaam en beschrijving.](../../assets/setup/aws-audience-sourcing/s3-connection-name-description.png)

### Automatisch toegewezen identiteitsvelden controleren {#auto-mapped-fields}

Het scherm **[!UICONTROL Mapping]** is alleen-lezen. U kunt geen transformaties toevoegen, verwijderen of toepassen. Collaboration wijst bronidentiteitsvelden van uw publieksbestanden automatisch toe aan doelvelden op basis van de Specificatie Audience Sourcing.

Bevestig de toegewezen velden visueel en selecteer **[!UICONTROL Next]** om door te gaan.

![&#x200B; het scherm van de gebiedstoewijzing die auto-in kaart gebrachte bron en gebieden van de doelidentiteit tonen.](../../assets/setup/aws-audience-sourcing/s3-field-mapping-auto-mapped.png)

### Vernieuwingsfrequentie en datumbereik plannen {#schedule-refresh}

De weergave **[!UICONTROL Schedule]** wordt weergegeven. Gebruik het vervolgkeuzemenu om een vernieuwingsfrequentie tussen één en zes dagen te selecteren en stel vervolgens het actieve datumbereik in. Gebruik het kalenderpictogram om begin- en einddatums op te geven.

>[!IMPORTANT]
>
>Als u uw Collaboration-credits effectief wilt beheren, stelt u de vernieuwingsfrequentie in zodat deze overeenkomt met de updatefrequentie van de onderliggende S3-gegevens of deze overschrijdt. Het minimaal ondersteunde vernieuwingsinterval is één keer per zes dagen.

![&#x200B; het scherm van de planningsmontages met verfrist frequentieopties en configuratie van de datumwaaier.](../../assets/setup/aws-audience-sourcing/s3-schedule-refresh-frequency.png)

### De verbinding controleren en voltooien {#review-and-complete}

Tot slot herzie uw configuratiemontages in het summiere scherm. Deze weergave bevat een overzicht van de volgende secties:

* **[!UICONTROL Data connection]**: Toont de rol IAM, S3 emmernaam, en omslagweg u vormde.
* **[!UICONTROL Details]**: geeft de naam en de optionele beschrijving van de gegevensverbinding weer, zodat u deze later kunt herkennen.
* **[!UICONTROL Mapping]**: geeft een overzicht van hoe de bronvelden uit uw geüploade publieksbestanden (bijvoorbeeld `HASHED_EMAIL` ) worden toegewezen aan doelvelden die worden gebruikt in Collaboration (bijvoorbeeld email met hashing).
* **[!UICONTROL Schedule]**: vat samen hoe vaak de verbinding publieksgegevens en het actieve datumbereik voor het sourcen vernieuwt.

Selecteer het potloodpictogram als u een sectie wilt bewerken. Selecteer **[!UICONTROL Complete]** om alle secties te bevestigen.

![&#x200B; het overzichtsscherm die gegevensverbinding, details, afbeelding, en planningssecties tonen.](../../assets/setup/aws-audience-sourcing/s3-connection-review-summary.png)

Er wordt een dialoogvenster weergegeven waarin wordt bevestigd dat de gegevensverbinding is gemaakt en dat de doelgroep bezig is met het aanschaffen van de verbinding.

## Bronpubliek bekijken {#review-sourced-audiences}

Na voltooiing van de configuratie, begint Collaboration publiek van uw S3 emmertje te betrekken. Soorten publiek dat via een [!DNL Amazon S3] emmertje is aangeschaft, worden op het tabblad **[!UICONTROL My Audiences]** weergegeven en hebben dezelfde functionaliteit en informatie als publiek dat vanuit Experience Platform is aangeschaft.

Als de doelgroep bezig is met het aanschaffen van een advertentie, verschijnt er een banner boven aan het scherm. Individuele doelgroepen worden alleen weergegeven nadat de bron is voltooid.

![&#x200B; het lusje van het publiek dat dat het bron lopend voor [!DNL Amazon S3] publiek toont.](../../assets/setup/aws-audience-sourcing/s3-audiences-sourcing-in-progress.png)

Zodra het publiek S3 wordt gedownload, wordt uw lijst van beschikbare doelgroepen verstrekt in een lijst of kaartmening.

>[!TIP]
>
>De de broningstijd van het publiek varieert gebaseerd op de grootte van uw S3 gegevens en verfrist frequentie u vormde. De grotere datasets of minder vaak verfrissen programma&#39;s kunnen langer duren om in de **[!UICONTROL My audiences]** werkruimte te verschijnen.

![&#x200B; het lusje van het publiek dat een lijst toont van een lijst van bronpubliek.](../../assets/setup/aws-audience-sourcing/s3-audiences-list-view.png)

Selecteer in de rasterweergave of tabelweergave een rij-item of **[!UICONTROL View audience]** om een overzicht van een specifiek publiek weer te geven. De status, bron en naam van de gegevensverbinding van het publiek worden weergegeven, samen met gedetailleerde deelvensters voor:

**[!UICONTROL Identities]**: geeft het totale aantal identiteiten en de verdeling weer zodra gegevens beschikbaar zijn.
**[!UICONTROL Categories]**: geeft alle tags weer die worden gebruikt voor het organiseren of filteren van het publiek.
**[!UICONTROL Connection access]**: Geeft aan of het publiek privé, openbaar of gedeeld is met specifieke deelnemers.
**[!UICONTROL Metadata visibility]**: bepaalt welke publieksinformatie (zoals het aantal identiteiten, het overlappingspercentage en de index) zichtbaar is voor deelnemers.

Gebruik deze mening om publieksconfiguratie en zichtbaarheidsmontages te bevestigen alvorens het publiek in samenwerkingsprojecten te gebruiken.

Zie de [&#x200B; documentatie van het publiek van de Mening dashboard &#x200B;](https://experienceleague.adobe.com/en/docs/real-time-cdp-collaboration/using/setup/onboard-audiences#view-audiences-dashboard) om meer te leren.

## De S3-gegevensverbinding weergeven {#view-s3-connection}

De zojuist toegevoegde [!DNL Amazon S3] verbinding is direct beschikbaar op het tabblad **[!UICONTROL My data connections]** . De publieksbron wordt weergegeven als [!UICONTROL Amazon S3] .

Uw S3 gegevensverbinding omvat de zelfde functionaliteit en de details zoals andere verbindingen van publieksgegevens, behalve dat kunt u geen publiek direct van deze mening toevoegen of uitgeven.

>[!NOTE]
>
>[!DNL Amazon S3] -gegevensverbindingen kunnen niet worden bewerkt. U kunt instellingen zoals de vernieuwingsfrequentie niet wijzigen als de verbinding eenmaal is gemaakt. Als u de configuratie wilt bijwerken, moet u de bestaande verbinding verwijderen en een nieuwe maken.

![&#x200B; het Mijn lusje van gegevensverbindingen die de [!DNL Amazon S3] gegevensverbinding met het bronstatusinformatie tonen.](../../assets/setup/aws-audience-sourcing/s3-data-connections-tab.png)

## Volgende stappen {#next-steps}

U hebt uw [!DNL Amazon S3] -opslag nu geconfigureerd en verbonden als gegevensbron in Collaboration. Door deze workflow te voltooien, hebt u beveiligde sourcing van gegevens voor het eerste publiek mogelijk gemaakt voor activering en overlappende analyse.

Nadat de sourcing is voltooid, worden uw publiek weergegeven in de **[!UICONTROL My audiences]** -werkruimte, klaar voor samenwerking en activering. Voor gedetailleerde beheersopties, zie de [&#x200B; bron en beheer publieksdocumentatie &#x200B;](./onboard-audiences.md).
