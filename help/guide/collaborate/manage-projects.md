---
title: Projecten maken en beheren
description: Leer hoe u projecten maakt en beheert in Adobe Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/nl/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: ae492846-bc0a-4422-86ca-577bcc1fa60c
source-git-commit: 0cf888e36ffc4730fc8de4d8adccae0e0fc2caa8
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 0%

---

# Projecten maken en beheren

{{limited-availability-release-note}}

Projecten vormen de kern van uw workflow in Adobe Real-Time CDP Collaboration. Nadat u verbinding hebt gemaakt met medewerkers, maakt u een project waarmee u overlappende berekeningen voor het publiek kunt uitvoeren en relevante doelgroepen voor campagnes kunt ontdekken.

>[!TIP]
>
>Projecten moeten over het algemeen worden gekoppeld aan één campagne.

![&#x200B; het Collaborate dashboard die alle huidige projecten tonen.](/help/assets/collaborate/manage-view-projects/projects-overview-page.png){zoomable="yes"}

U kunt filters gebruiken om slechts de projecten te bekijken die u met bepaalde medewerkers, zoals hieronder getoond bent begonnen:

![&#x200B; Gefilterde mening van projecten met één enkele medewerker.](/help/assets/collaborate/manage-view-projects/filtered-project-view.png){zoomable="yes"}

## Project maken {#create-project}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_create_project_advertisername_amc"
>title="Naam adverteerder (Amazon Marketing Cloud)"
>abstract="Voor Amazon Marketing Cloud-verbindingen (AMC) vertegenwoordigt dit veld de AMC-instantie waartoe uw Amazon Ads-aanmelding toegang heeft. Er wordt geen naam van een adverteerder weergegeven. Als het vereiste exemplaar niet wordt vermeld, contacteer uw beheerder van Amazon Marketing Cloud om toegang te verzoeken."

Om een project tot stand te brengen, moet u eerst [&#x200B; een verbinding &#x200B;](/help/guide/connect/establishing-connections.md) met een medewerker vestigen. Zodra de verbinding wordt gevestigd, kunt u een project met die medewerker tot stand brengen.

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_projects_advertisername"
>title="Naam adverteerder"
>abstract="Selecteer de naam van de adverteerder in het vervolgkeuzemenu. De opties worden vooraf geconfigureerd door de uitgever in de verbindingsinstellingen om ervoor te zorgen dat ze compatibel zijn met hun systemen."

Navigeer naar **[!UICONTROL Collaborate]** en vervolgens naar **[!UICONTROL My Projects]** . Als dit uw eerste project is, kunt u **[!UICONTROL Create a project]** selecteren. Anders kunt u het toevoegen pictogram selecteren (![&#x200B; voeg pictogram toe.](/help/assets/icons/plus.png)) om op elk moment een nieuw project te maken.

![&#x200B; Uitgezocht plus symbool of creeer een project aan opstelling een nieuw project.](/help/assets/collaborate/manage-view-projects/create-project.png){zoomable="yes"}

Het dialoogvenster **[!UICONTROL Create project]** wordt weergegeven. Selecteer de **[!UICONTROL Collaborator]** waarmee u het project maakt via de vervolgkeuzelijst. Als u een uitgever bent en u adverteerdernamen tijdens uw verbindingsopstelling plaatst, kunt u **[!UICONTROL Advertiser name]** selecteren.

>[!NOTE]
>
> Als u één enkele adverteerdernaam in de verbindingsmontages vormde, verschijnt het door gebrek. Als er geen naam van de adverteerder is ingesteld, wordt de voorinstelling **[!UICONTROL Name]** van de adverteerder geselecteerd als de **[!UICONTROL Advertiser name]** .

![&#x200B; creeer projectdialoog met geselecteerde medewerker en benadrukte adverteerdernaam.](/help/assets/collaborate/manage-view-projects/create-project-advertiser-names.png){zoomable="yes"}

Voeg vervolgens een **[!UICONTROL Project name]** en **[!UICONTROL Description]** toe voor uw project. Selecteer vervolgens een afbeelding die het project vertegenwoordigt. Dit beeld helpt om het project in de pagina van het projectoverzicht te onderscheiden. Als u klaar bent, selecteert u **[!UICONTROL Create]** om het project te maken.

![&#x200B; Vereiste opties aan opstelling een nieuw project &#x200B;](/help/assets/collaborate/manage-view-projects/create-project-required-info.png){zoomable="yes"}

U kunt nu uw nieuwe project, zijn details, en beschikbare die secties bekijken op de gebruiksgevallen tijdens verbindingsopstelling worden geselecteerd.

![&#x200B; de werkruimte van het projectoverzicht.](/help/assets/collaborate/manage-view-projects/project-overview.png){zoomable="yes"}

## Campagne-id beheren {#manage-campaign-id}

A **identiteitskaart van de Campagne** verbindt uw project met een specifieke campagne en wordt vereist om metingsrapporten [&#128279;](./measure.md#create-measurement-report) te produceren. U kunt veelvoudige campagne IDs aan één project toevoegen als u verscheidene campagnes met de zelfde medewerker in werking stelt. Al deze campagnes zijn beschikbaar voor selectie in rapportering.

- **Uitgevers**: Ga of werk Campagne IDs en bijbehorende namen in Collaboration UI vóór het runnen van rapporten binnen.
- **Advertisers**: Vraag uw medewerker (uitgever) om Campagne IDs toe te voegen zoals nodig.

Als u campagne-id&#39;s wilt toevoegen of bijwerken, navigeert u naar de **[!UICONTROL Collaborate]** -werkruimte en selecteert u vervolgens **[!UICONTROL View]** in de relevante projectkaart.

![&#x200B; de Collaborate werkruimte die de optie van de Mening binnen een projectkaart benadrukt.](/help/assets/collaborate/manage-view-projects/view-project.png){zoomable="yes"}

De bijbehorende **[!UICONTROL Project overview]** werkruimte wordt weergegeven met een **[!UICONTROL Campaign ID and name]** -sectie waarin alle campagnes worden weergegeven die aan het project zijn gekoppeld. Selecteer **[!UICONTROL Add]** als u nog geen campagne hebt toegevoegd. Als er al campagnes aanwezig zijn, selecteert u **[!UICONTROL Edit]** om details bij te werken of extra campagnes toe te voegen.

![&#x200B; de werkruimte van het projectoverzicht die identiteitskaart van de Campagne en naamsectie tonen met de Edit benadrukte optie.](/help/assets/collaborate/manage-view-projects/edit-campaign-id.png){zoomable="yes"}

Selecteer **[!UICONTROL Add campaign ID]** in het dialoogvenster **[!UICONTROL Campaign ID and name]** om een nieuwe rij toe te voegen waarin u campagnedetails kunt invoeren.

![&#x200B; identiteitskaart van de Campagne en noem dialoog tonend de lege campagnemijl na het selecteren van Add de optie van campagneidentiteitskaart.](/help/assets/collaborate/manage-view-projects/add-campaign-row.png){zoomable="yes"}

Geef de velden **[!UICONTROL Campaign ID]** en **[!UICONTROL Campaign name]** op en selecteer vervolgens **[!UICONTROL Save]** .

![&#x200B; identiteitskaart van de Campagne en noem dialoog die de nieuwe campagnedetails en sparen benadrukte optie tonen.](/help/assets/collaborate/manage-view-projects/save-campaign-id.png){zoomable="yes"}

Raadpleeg de sectie **[!UICONTROL Campaign ID and name]** voor de meest recente campagnes en wijzigingen. U kunt nu de nieuwe campagne-id&#39;s gebruiken om meetrapporten te genereren.

![&#x200B; de werkruimte van het projectoverzicht die bijgewerkte identiteitskaart van de Campagne en naamsectie tonen.](/help/assets/collaborate/manage-view-projects/view-updated-campaigns.png){zoomable="yes"}
