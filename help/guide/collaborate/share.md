---
title: Soorten publiek delen
description: Leer hoe u publiek kunt delen met uw medewerkers voor reclamecampagnes.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0fdf0598-89c9-452d-a2e3-ce868df0b9d2
source-git-commit: acaaaa1e1fab981d874210639c16e76e48fc3394
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 0%

---

# Soorten publiek delen

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>De **[!UICONTROL Share]** werkruimte is slechts beschikbaar als het **Delen van het Publiek en het 2&rbrace; gebruiksgeval van de activering [ tijdens het verbindingsproces ](../connect/establishing-connections.md#connection-settings) werd toegelaten.** Voor meer informatie over gebruiksgevallen, verwijs naar [ projecten ](./manage-projects.md#project-use-cases) gids beheren.

Als adverteerder leert u hoe u publiek kunt delen met uw uitgevers zodat deze campagnes kunnen voeren. Als uw samenwerking **heeft toegelaten ontdekken publiek** gebruiksgeval, begin door overlappende rapporten in te stellen [ ontdekt lusje ](/help/guide/collaborate/discover.md) om het beste publiek voor het delen te identificeren.

## Nieuw publiek delen

Navigeer naar het tabblad **[!UICONTROL Share]** in uw projectwerkruimte om het delen van het publiek te starten. Slechts **adverteerderorganisaties** kunnen publiek voor campagnes delen. Op dit tabblad kunt u gedeelde doelgroepen controleren en beheren.

Selecteer het **plus symbool (+)**, of de **[!UICONTROL Share audience]** optie als geen vorig publiek is gedeeld, beginnen het publiek delend proces.

![ Standaardmening zonder gedeeld publiek.](/help/assets/collaborate/share/share-new-audiences.png)

Er wordt een nieuw deelvenster weergegeven waarin u het publiek kunt selecteren dat u met uw medewerker wilt delen.

![ deel nieuw publiek werkschema.](/help/assets/collaborate/share/share-audiences-workflow.png)

### Selecteer publiek dat u wilt delen

In het venster van de publieksselectie, kunt u naar specifieke publiek zoeken om te delen door de publieksnaam in de onderzoeksbar in te gaan. Selecteer **[!UICONTROL Browse audiences]** en gebruik de beschikbare sorteeropties om precies het gewenste publiek te zoeken.

![ doorblader publiek mening met geselecteerd publiek.](/help/assets/collaborate/share/browse-audiences-view.png)

### Overeenkomstsleutels bewerken en doelopties instellen

Nadat u het gewenste publiek hebt geselecteerd dat u wilt delen, kunt u nu andere configuratieopties selecteren voor de deelactiviteit.

![ geef gelijke sleutels uit en doel of onderdruk benadrukte selecteur ](/help/assets/collaborate/share/match-keys-and-targeting.png)

Selecteer **[!UICONTROL Edit match keys]** om aan te geven welke overeenkomende toetsen moeten worden gebruikt voor de identiteiten in het publiek. Deze opties worden overgenomen van de instellingen die zijn geselecteerd toen de verbinding tussen deelnemers voor het eerst werd ingesteld. U kunt matrixtoetsen verwijderen die op dat punt zijn geselecteerd als deze niet van toepassing zijn op deze specifieke campagne, maar u kunt op dit punt geen nieuwe overeenkomende toetsen toevoegen.

![ geef gelijke sleutels uit.](/help/assets/collaborate/share/update-match-keys.png)

Geef voor elk publiek aan of u de doelgroep of de doelgroep in de campagne wilt instellen. Onderdrukte profielen maken specifiek geen deel uit van het publiek dat door de uitgever wordt geactiveerd.

### Vernieuwingsfrequentie en interval voor het publiek instellen

Tot slot plaats de gewenste frequentie en de datumwaaier voor het publiek verfrist zich. De momenteel ondersteunde modi voor publieksvernieuwing zijn **[!UICONTROL Once]** en **[!UICONTROL Daily]** .

Wanneer u **[!UICONTROL Once]** selecteert, wordt het publiekslidmaatschap niet vernieuwd tijdens de duur van een campagne. Wanneer u **[!UICONTROL Daily]** selecteert, wordt het publiekslidmaatschap eenmaal per dag vernieuwd tijdens de duur van een campagne.

![ benadrukte de opties van de Frequentie.](/help/assets/collaborate/share/audience-refresh-frequency.png)

Als u tevreden bent met de selecties, selecteert u **[!UICONTROL Share]** om de workflow te voltooien.

>[!SUCCESS]
>
>U ziet nu een nieuwe activiteit voor het delen van publiek op het tabblad **[!UICONTROL Sharing]** . Desgewenst kunt u teruggaan en alle selecties bewerken die u hebt gemaakt.

## Momenteel gedeeld publiek weergeven

Op het tabblad **[!UICONTROL Sharing]** kunt u het publiek weergeven dat momenteel wordt gedeeld door de deelnemers, gegroepeerd in activiteiten voor het delen van het publiek.

![ Overzicht van het delen tabel.](/help/assets/collaborate/share/share-tab-overview.png)

<!--

The banner at the top of the page shows figures across all audience sharing activities. 

![The hero banner in the sharing tab.](/help/assets/collaborate/share/share-hero-banner.png)


|Metric | Description |
|---------|----------|
| **[!UICONTROL Shared audiences]** | Indicates the number of audiences shared between collaborators in this project, across all audience sharing modules. |
| **[!UICONTROL Estimated addressable reach]** | Indicates the approximate number of profiles that you can reach across all the audiences that are currently shared in the project. [TODO: ADD INFORMATION ABOUT HOW THIS IS CALCULATED] |
| **[!UICONTROL Target identities]** | The number of identities across all audiences shared in this project for which you selected to target the profiles. |
| **[!UICONTROL Suppress identities]** | The number of identities across all audiences shared in this project for which you selected to suppress the profiles and thereby not target them in campaigns. |

-->

Binnen elke activiteit die van het publiek deelt, kunt u informatie over elk gedeeld publiek krijgen.

| Metrisch | Beschrijving |
|---------|----------|
| **[!UICONTROL Identity count]** | Hiermee geeft u het aantal profielen voor alle identiteiten aan die aan dit publiek zijn gekoppeld, volgens de meest recente evaluatie van het aantal identiteiten. Deze getallen worden elke 24 uur vernieuwd. |
| **[!UICONTROL Overlapping identities]** | Geeft het aantal overlappende identiteiten tussen de leden van dit publiek aan en de totale populatie van profielen in de inventaris van de deelnemer. |
| **[!UICONTROL Match key breakdown]** | Toont het identiteitsaantal voor elke identiteit die in het publiek wordt gebruikt. Een totaal aantal gebruikers van 500.000 kan bijvoorbeeld bestaan uit 400.000 gebruikers die de gehashte e-mailidentiteit hebben uitgeschakeld en 100.000 gebruikers die een mobiele-id-identiteit hebben afgevinkt. Let op: in het hier beschreven voorbeeld is dezelfde persoon mogelijk twee keer aanwezig in het publiek met zijn e-mail- en mobiele-id-id-id-identiteit. |
| **[!UICONTROL Objective]** | **[!UICONTROL Suppress]** of **[!UICONTROL Target]** . Hiermee geeft u aan of de leden van een publiek doelgroep moeten zijn of moeten worden uitgesloten van campagnes. |

De pagina bevat ook besturingselementen voor **[!UICONTROL Pause sharing]** en **[!UICONTROL Edit audiences]** .

## Soorten publiek bewerken {#edit-audiences}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_share_edit_audiences_usecases"
>title="Gebruiksscenario voor doel of onderdrukken"
>abstract="<p>Selecteer **Doel** als u de profielen in het publiek wilt worden getoond advertenties in de campagne.</p> <p>Selecteer **Onderdruk** als u de profielen in het publiek van het campagneoverseinen wilt uitsluiten.</p>"

Selecteer **[!UICONTROL Edit audiences]** om te wijzigen welk publiek wordt gedeeld in een module voor het delen van publiek en om verschillende configuraties te wijzigen voor de manier waarop het publiek wordt gedeeld.

![ Mening van uitgeeft publiek modaal ](/help/assets/collaborate/share/edit-audiences-modal.png)

<!--

Search for audiences that you want to add to the sharing module. 

For each audience, you can select whether you'd like to target or suppress those profiles in campaigns. 

To remove an audience from the sharing module, select the trash can icon [TODO: add spectrum icon and folder].

Select how often you would like the audience membership to be refreshed and the date range within which you want the membership of the audience to be refreshed. 

TODO: are there any limitations for frequency in the M1 release?

-->

## Volgende stappen

Nadat de uitgever het gedeelde publiek ontvangt, zullen zij [&#128279;](/help/guide/collaborate/activate.md) hen nu activeren in digitale reclamecampagnes.
