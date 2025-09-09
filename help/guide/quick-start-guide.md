---
title: Real-Time CDP Collaboration Quick Start Guide
description: Leer hoe u in Real-Time CDP Collaboration aan boord van uw organisatie kunt gaan, zoals het instellen van rollen en organisaties, het aantrekken van het publiek, activering en meting. Deze gids helpt samenwerkers verbindingsmontages vormen beginnen hun publiek veilig en efficiënt te gebruiken.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 68e5095e-ece5-4f64-9056-10f3b216cf0c
source-git-commit: 849bae30b4e617a6c49f68b2baedc0ab8a822854
workflow-type: tm+mt
source-wordcount: '1384'
ht-degree: 0%

---

# Real-Time CDP Collaboration-handleiding voor snel starten

{{limited-availability-release-note}}

Ga aan de slag met Real-Time CDP Collaboration door uw organisatie te configureren, publiek te betrekken en activering en meting op basis van privacy mogelijk te maken.

## Vereisten

Voordat u begint, moet u het volgende doen:

- Een actieve Real-Time CDP Collaboration-licentie.
- [ toegang van het Systeem of van de productbeheerder tot Adobe Experience Platform ](./permissions/overview.md).
- [ Toegang provisioned voor eind - gebruikers ](./permissions/manage-user-access.md).
- [ Rollen die voor uw organisatie worden gecreeerd en aan gebruikers ](./permissions/manage-roles.md) worden toegewezen.
- Toegang tot brandingmiddelen, zoals de naam, het logo en de banner van uw organisatie.
- A [ bepaalde gelijke zeer belangrijke strategie ](./setup/onboard-account.md#set-up-match-keys)
- (Optioneel) Als u Experience Platform niet gebruikt voor publieksbeheer, hebt u toegang tot een ondersteunde cloudbron (Amazon S3 of Snowflake).

## Stap 1: Volledige op rollen gebaseerde opstelling {#complete-role-based-setup}

De de toegangsrollen van uw organisatie bepalen wat de gebruikers kunnen zien en doen in Collaboration. Voordat u verdergaat, moet u ervoor zorgen dat op rollen gebaseerde machtigingen op de juiste wijze zijn ingesteld om de juiste toegang en zichtbaarheid in het platform te garanderen.

**Middelen:**

- [Documentatie gebruikerstoegang](./permissions/manage-user-access.md)
- [Documentatie voor rolinstellingen](./permissions/manage-roles.md)


Bekijk deze video voor meer informatie over het toewijzen van producttoegang en -machtigingen voor Collaboration met de Admin Console en Experience Platform.

>[!VIDEO](https://video.tv.adobe.com/v/3452216/?learn=on&enablevpops)

## Stap 2: Een Collaboration-account instellen {#set-up-your-account}

Voordat u publiek kunt maken, moet u uw account configureren in Collaboration. Dit bepaalt hoe u verschijnt en waartoe u toegang hebt in de interface.

Als u niet de noodzakelijke toegang hebt, gelieve terug naar stap 1 te verwijzen of uw beheerder van uw organisatie voor hulp te contacteren die deze opstelling voltooit.

Definieer de rol van uw account in Collaboration, voeg brandingmiddelen toe en configureer matrixtoetsen om het publiek via verbindingen uit te lijnen.

>[!NOTE]
>
>Tijdens het instellen kunt u een of meer accounts maken (zoals een adverteerder en een uitgever). Bepaalde velden, zoals brandingmiddelen en contact via e-mail, kunnen later in de werkruimte van **[!UICONTROL Settings]** worden bijgewerkt.

- **wijs een rol** toe - bepaalt of uw rekening een adverteerder of een uitgever is. Uw rol bepaalt welke mogelijkheden u in Collaboration hebt. Om meer over te leren hoe de rollen het samenwerkingswerkschema beïnvloeden, zie de [ rollen ](./overview/roles.md) gids.
- **Brandende activa** - voeg het volgende aan uw rekening toe:
   - Accountnaam (max. 100 tekens)
   - Beschrijving (max. 1000 tekens)
   - Logo (SVG &lt;20KB, idealiter vierkant)

>[!NOTE]
>
>Neem contact op met uw Adobe-accountvertegenwoordiger als u een uitgeveraccount maakt en deze openbaar wilt maken in de catalogus voor Collaboration-verbindingen. Voor uitgeveraccounts is een aangepaste merkbanner vereist (JPG 2688x1536). Dit bestand kan rechtstreeks met uw vertegenwoordiger worden gedeeld.

- **E-mail van het Contact** - verstrek een bedrijfs-e-mail voor medewerkers aan gebruik nadat een verbinding wordt gevestigd.
- **vorm gelijke sleutels** - selecteer de herkenningstekens die voor publiek aanpassing worden gebruikt.

Meer over aanvankelijke rekeningsopstelling leren, met inbegrip van hoe te om rollen te bepalen, het brandmerken activa te uploaden, en gelijke sleutels te vormen, zie de [ gids van de 0&rbrace; aanvankelijke rekeningsopstelling &lbrace;.](./setup/onboard-account.md#initial-account-setup){target="_blank"}

Bekijk deze video voor een stapsgewijze analyse van een adverteerderopstelling, met inbegrip van rekeningsverwezenlijking, branding, en de configuratie van de gelijkesleutel.

>[!VIDEO](https://video.tv.adobe.com/v/3452264/?learn=on&enablevpops)

## Stap 3: Source-publiek (van Experience Platform of een cloudbron) {#source-audiences}

Zodra uw account is gemaakt en uw branding en match keys zijn geconfigureerd, bent u klaar om het publiek te betrekken. Kies een van de volgende bronmethoden op basis van uw gegevensopslag en bedrijfsbehoeften.

### Optie A: Source van Experience Platform

[ Gebruik Collaboration om een zandbak te verbinden die publiek ](./setup/onboard-audiences.md) bevat. Gebruik deze zelfbedieningsmethode om te verwijzen naar bestaande publiekssegmenten vanuit uw Experience Platform-instantie.

#### Soorten publiek configureren

Configureer hoe doelgroepen worden voorbereid, aangepast en beheerd voor gebruik in verbindingen.

- **Uitgezochte publiek** *(Experience Platform slechts)* - kies publiekssegmenten met gesteunde herkenningstekens.
- **de gelijke van de Kaart sleutels** - richt publieksgebieden met de gevormde gelijke sleutels.
- **pas transformaties** toe - de waarden van de Hash plaintext (bijvoorbeeld, e-mail) indien nodig.
- **vernieuwt het Programma** - bepaalt updatefrequentie (bijvoorbeeld, dagelijks).
- **vorm toestemmingsmontages** - bepaal welke profielen om in verbindingen door een toestemmingswijze te selecteren verkiesbaar zijn: opt-in, opt-out, of niets.

>[!NOTE]
>
>U kunt soorten publiek toevoegen of verwijderen en het vernieuwingsschema direct in Collaboration bijwerken. Als u andere instellingen wilt wijzigen, zoals de toetsen of toestemmingsmodus, moet u de gegevensverbinding verwijderen en opnieuw maken.

>[!IMPORTANT]
>
>**Maximum aantal soorten publiek per samenwerkingsrol:**
>
>- **Advertisers** kan tot 25 publiek bron.
>- **Uitgevers** kunnen tot 250 publiek (elk met een minimum van 1.000 IDs) bron.

>[!IMPORTANT]
>
>**de belangrijkste vereisten van de Gelijke:**
>
>Alle gelijke sleutels moeten **worden in orde gebracht**, **verlaagd**
>&#x200B;>De gehakte gelijke sleutels moeten **SHA256-gehakt** zijn.\
>Als u hashwaarden opgeeft waarin hoofdletters worden gebruikt, zet Collaboration deze automatisch om in kleine letters.\
>Als uw bron **plaintext herkenningstekens** bevat, gebruik de **[!UICONTROL Apply transformation]** optie om het hakken toe te passen. Deze optie is alleen beschikbaar wanneer gebruikers worden aangeschaft bij Experience Platform en wordt niet ondersteund voor bronnen in de cloud.
>
>Voor meer informatie, zie de [ kaartgebieden ](./setup/onboard-audiences.md#map-fields) sectie van de bron en beheer de gids van het publiek.

Bekijk de onderstaande video voor een volledige analyse van hoe u publiek kunt bronnen met Collaboration.

>[!VIDEO](https://video.tv.adobe.com/v/3452217/?learn=on&enablevpops)

Alternatief, zie het document op [ sourcing publiek in Collaboration ](./setup/onboard-audiences.md#source-and-manage-audiences).

### Optie B: Source van Snowflake of Amazon S3

Om een wolkenbron (bijvoorbeeld, [!DNL AWS S3] of [!DNL Snowflake]) te vormen, bereidt uw publieksgegevens voor gebruikend de volgende [ Specificatie PDF van de Publiek ](../assets/quick-start/RTCDP_Collaboration_Audience_Onboarding_Spec_v1.0.pdf). Als de installatie is voltooid of als u vragen hebt, neemt u contact op met uw Adobe-accountvertegenwoordiger om de installatie te voltooien. Deze methode is geen zelfbediening en vereist hulp van Adobe.

>[!IMPORTANT]
>
>Cloudgebaseerde publieksbestanden moeten het vereiste schema volgen dat wordt beschreven in de Audience Specification PDF. Bestanden moeten hashed-id&#39;s (lagere SHA256), vereiste metagegevensvelden zoals `segment_name` en `activation_id` bevatten en ondersteunde indelingen zoals CSV of Parquet gebruiken. Adobe normaliseert de gegevens niet voordat deze worden geactiveerd. TTL wordt afgedwongen gebaseerd op de levensduur van het publiek.
>
>Alle soorten publiek in het geüploade bestand zijn in dit stadium volledig afkomstig. Het [ publiek zicht plaatsen ](/help/guide/setup/onboard-audiences.md#metadata-visibility) bepaalt of uw medewerkers uw publiek kunnen bekijken en door Collaboration UI geleid.

## Stap 4: Het publiek activeren (naar Experience Platform of een cloudbestemming) {#activate-audiences}

Activeer vervolgens het publiek naar uw Experience Platform-exemplaar of naar een cloudbestemming.

### Optie A: activeren naar Experience Platform

Voltooi de volgende stappen die in [ worden geschetst vormen Adobe Experience Platform als bestemmings ](/help/guide/destinations/experience-platform.md) gids.

- **creeer een bestemming** - gebruik UI aan opstelling een bestemming van Experience Platform (zandbak-niveau).
- **de overeenkomende sleutels van de Kaart** - selecteer het herkenningsteken (b.v., `hashedEmail`).
- **bepaalt TTL** - vastgestelde vervaldatum (1-30 dagen).
- **verifieer in het Portaal van het Publiek** - Zodra een medewerker u een publiek verzendt, verifieer dat het in het Portaal van het Publiek onder de oorsprong &quot;[!UICONTROL Real-Time CDP Collaboration] verschijnt.&quot;

### Optie B: activeren naar cloud

Als u een cloudbestemming wilt configureren (bijvoorbeeld [!DNL AWS S3] of [!DNL Snowflake] ), neemt u contact op met uw Adobe-accountvertegenwoordiger om het installatieproces te starten. Afhankelijk van de bestemming van de cloud, moet u gegevens over de bestemming van de cloud opgeven, zoals het bestandspad, de referenties, de locatie van de account enzovoort. Zodra de vereiste informatie is verstrekt, zal Adobe de opstelling van de wolkenbestemming vormen.

De gegevens van het publiek die naar een wolkenbestemming worden verzonden volgen een vooraf bepaald schema. Voor een gedetailleerde beschrijving van de vereiste gebieden en het formaat, download de [ Gids van Audience Activation van Collaboration ](../assets/quick-start/RTCDP_Collaboration_Audience_Activation_Spec_v1.0.pdf).

## Stap 5: De meting instellen (optioneel) {#set-up-measurement}

>[!AVAILABILITY]
>
>Deze eigenschap is in **bèta** en beschikbaar uitsluitend aan klanten in het Beperkte programma van de Beschikbaarheid. Neem contact op met uw Adobe-vertegenwoordiger om toegang aan te vragen.

>[!IMPORTANT]
>
>De **[!UICONTROL Measure]** werkruimte is slechts beschikbaar als **[!UICONTROL Measurement]** gebruiksgeval [ tijdens het verbindingsproces ](./connect/establishing-connections.md#connection-settings) werd toegelaten. Voor meer informatie over gebruiksgevallen, verwijs naar [ projecten ](./collaborate/manage-projects.md#project-use-cases) gids beheren.

Collaboration biedt diverse rapporten om het bereik, de frequentie en de doeltreffendheid van de campagne te analyseren. Hoewel de werkruimte van **[!UICONTROL Measure]** beschikbaar is in de gebruikersinterface, is voor de volledige rapportfunctionaliteit mogelijk backendenactivering vereist.

Leren om metingsrapporten te bekijken en te interpreteren, zie de [ gids van de Meting ](./collaborate/measure.md). Het omvat attributie, campagne summiere metriek, en dashboards zoals bereikcurven en frequentieverdeling.

<!-- 
Commenting out the below information as this workflow is not yet in Beta but will be imminently. A guided measurement configuration workflow will be available in a future release."

### Configure measurement workflow

Collaboration supports two measurement workflows:

- **Attribution using Adobe Experience Platform datasets**
- **Campaign summary using only partner-provided data**

Choose the appropriate workflow below based on your campaign measurement goals.

#### Option A: Attribution using Experience Platform datasets

Use this workflow to measure conversion activity using datasets stored in Experience Platform.

1. **Create a measurement data connection**
   - Select the dataset that contains your conversion events.
   - Map identity fields from your dataset to the match keys used in Collaboration.
   - Manage consent and governance settings.
   - Define one or more conversion events to measure.
   - Review and confirm your setup.

2. **Run a measurement report**
   - Go to the **[!UICONTROL Measure]** workspace within the associated project.
   - Input the report name, date range, and report run date.
   - Select **[!UICONTROL Attribution]** as the report type.
   - Select the defined conversion event(s).
   - Submit the report. It will run on the specified date and populate within 24 hours.

#### Option B: Campaign summary using partner-provided data

Use this workflow to generate campaign summary insights based on advertiser-supplied identifiers (for example, campaign ID).

1. **Set up the connection**
   - In the connection settings, ensure **[!UICONTROL Measurement]** is selected as a use case.
   - Create a project under the connection with **[!UICONTROL Measurement]** as an activity.

2. **Provide campaign context**
   - Input required campaign identifiers (for example, **Campaign ID**) for the partner to reference.
   - Align with your partner on campaign scope and reporting timeline.

3. **Run a measurement report**
   - Navigate to the **[!UICONTROL Measure]** workspace within the project.
   - Input the report name, date range, and report run date.
   - Select **[!UICONTROL Campaign summary]** as the report type.
   - Submit the report. It will run on the selected date and populate within 24 hours. 
-->

## Stap 6: Verbinding maken met deelnemers {#connect-with-collaborators}

Nu de installatie is voltooid, is uw organisatie nu klaar om verbinding te maken met medewerkers door uitnodigingen te verzenden of te accepteren en projectinstellingen ter goedkeuring in te dienen. Dit verbindingsproces omvat het verzenden of ontvangen van uitnodigingen, het controleren en het voorleggen van verbindingsmontages (zoals gebruiksgevallen en kredietconsumptie), en het bevestigen van de verbinding.

Als adverteerder gebruikt u de werkruimte **[!UICONTROL Connect]** in het navigatiemenu links om door beschikbare uitgevers te bladeren. Alternatief, kunnen de medewerkers met elkaar direct door [ privé verbindingsuitnodigingen ](./connect/establishing-connections.md#private-connection-invite){target="_blank"} verbinden.

>[!NOTE]
>
>Momenteel kunnen alleen adverteerders door uitgevers bladeren. Uitgevers kunnen niet door verbindingen met adverteerders bladeren of deze tot stand brengen.

Voor een overzicht van deze stroom, zie [ het vestigen van verbindingsgids ](./connect/establishing-connections.md){target="_blank"}. Voor een visuele analyse van het verbindingsproces, met inbegrip van het doorbladeren van medewerkers en het beheren van verbindingsmontages, bekijk de [ video van de de rekeningsopstelling van de adverteerder ](https://experienceleague.adobe.com/en/docs/platform-learn/tutorials/collaboration/connect-with-publishers){target="_blank"}.

## Volgende stappen

U hebt nu de eerste setup voltooid en uw organisatie geconfigureerd voor veilige samenwerking. Verken vervolgens de volgende bronnen om meer inzicht te krijgen in activering, meting en gegevensbeheer:

- [ documentatie van het de activeringswerkschema van het publiek ](./collaborate/activate.md)
- [ het gebruikscase van de Meting ](./collaborate/measure.md)
- [Aanbevolen werkwijzen voor Collaboration-governance](./setup/onboard-audiences.md#governance-policy-and-enforcement-actions)
