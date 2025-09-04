---
title: Opmerkingen bij de nieuwste Real-Time CDP Collaboration-release
description: Volg de nieuwste releases voor Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 8513c648-1cc1-4544-b86d-2ee3193ab60f
source-git-commit: 738c7bc9f3a482a1c7c92c820b364c577e61dd56
workflow-type: tm+mt
source-wordcount: '1030'
ht-degree: 1%

---

# Opmerkingen bij de nieuwste Real-Time CDP Collaboration-release

{{limited-availability-release-note}}

**Laatste update**: Augustus 2025.

Deze releaseopmerkingen betreffen de functionaliteit die in Adobe Real-Time CDP Collaboration wordt vrijgegeven. Collaboration-releases werken op een doorlopend leveringsmodel, dat een gemiddelde maandelijkse release mogelijk maakt. Deze releaseopmerkingen worden vaak bijgewerkt, dus zorg ervoor dat u ze regelmatig controleert.

## Augustus 2025 {#august-2025}

* Medewerkers kunnen nu meerdere soorten publiek tegelijk bewerken. U kunt de metagegevens van het publiek, de toegang tot de verbinding, namen, beschrijvingen en categorieën voor meerdere soorten publiek nu bewerken met het gereedschap voor bulkbewerking. Meer leren over het uitgeven publiek, leest [ publiek ](../setup/onboard-audiences.md#edit-audiences) gids beheren.

## Juli 2025 {#july-2025}

CDP Collaboration in realtime ondersteunt nu merkgebonden samenwerking. Medewerkers kunnen nu verbindingen maken, ongeacht of ze adverteerders of uitgevers zijn. Dit maakt flexibelere samenwerkingsmogelijkheden mogelijk en stelt merken in staat elkaars gegevens en inzichten te benutten. Meer over de verschillen tussen merk-aan-merk samenwerking en adverteerder-aan-uitgever samenwerking leren, lees de [ gids van de 0&rbrace; samenwerkingspatronen &lbrace;.](../overview/collaboration-patterns.md)

* De medewerkers kunnen nu met elkaar verbinden gebruikend [ privé verbinding nodigt ](../connect/establishing-connections.md#private-connection-invites) uit. Deel de unieke verbindingscode van uw account met een medewerker die deze vervolgens kan gebruiken om rechtstreeks verbinding met u te maken. Dit is een kernkenmerk van merkgebonden samenwerking, waardoor medewerkers naast adverteerders ook verbindingen tot stand kunnen brengen om de map **[!UICONTROL Discover publishers]** te verkennen.
* [ Zelf-serverbestemmingen ](../setup/manage-destinations.md) zijn nu beschikbaar aan zowel adverteerders als uitgevers.
* De activering van het publiek is nu beschikbaar voor beide medewerkers in een verbinding, ongeacht hun [ rekeningsrol ](../overview/roles.md). De activeringsmontages van het publiek worden gevormd terwijl [ het vestigen van verbindingen ](../connect/establishing-connections.md#configure-connection-settings), toestaand u om te specificeren welke samenwerker publiek kan activeren. Meer over publieksactivering leren, lees [ activeer publiek ](../collaborate/activate.md) gids.
* De gebruikszaak van **[!UICONTROL Activate]** is opnieuw geconfigureerd ter ondersteuning van de samenwerking tussen merken en merken. Het tabblad **[!UICONTROL Activate]** in een project geeft nu het publiek weer dat naar uw medewerker is verzonden en het publiek dat door uw medewerker naar uw doel is geactiveerd. Meer leren, lees [ activeer publiek ](../collaborate/activate.md) gids. <br> ![ activeer dashboard met het publiek naar en het publiek activeerde secties wordt verzonden die.](/help/assets/release-notes/2025/activate-dashboard.png){zoomable="yes"}
* De scores voor de index van het publiek zijn nu beschikbaar op het tabblad **[!UICONTROL Discover]** van een project. De score van de publieksindex is een maat voor de mate waarin een publiek overeenkomt met het publiek van uw medewerker. Deze score wordt berekend op basis van het aantal onderliggende doelgroepen en de overlappingen. Meer over de scores van de publieksindex leren, lees de [ score van de publieksindex ](../collaborate/discover.md#audience-index-score) gids.

## Mei 2025 {#may-2025}

* Real-Time CDP Collaboration is nu beschikbaar aan klanten in **Australië** en **Nieuw Zeeland**. Deze service is automatisch beschikbaar voor Real-Time CDP Prime- en Ultimate-klanten in deze regio&#39;s.
* Real-Time CDP Collaboration biedt nu [ zelf-serverbestemmingen ](../setup/manage-destinations.md) door het **[!UICONTROL My destinations]** lusje in de **[!UICONTROL Setup]** sectie aan. Met doelen kunt u het publiek activeren op externe platforms, zoals advertentienetwerken of platforms voor gegevensbeheer, zodat u uw klanten op verschillende kanalen kunt bereiken. Momenteel worden alleen Adobe Experience Platform-doelen ondersteund. Neem contact op met uw Adobe-vertegenwoordiger als u een andere bestemming wilt configureren. Meer over bestemmingen leren, lees de [ gids van het bestemmingsoverzicht ](../destinations/overview.md).
   * De bestemmingen voegen ook steun toe om het publiek van Collaboration in het [ het publieksportaal van Adobe Experience Platform ](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences) te bekijken.
* U kunt de publieksvernieuwingsfrequentie voor bestaande gegevensverbindingen in Collaboration nu bewerken. Op dit moment kunt u ervoor kiezen uw publiek dagelijks of om de twee tot zes dagen te vernieuwen. Meer over leren hoe te om het publiek uit te geven verfrist frequentie, leest [ gegevensverbindingen ](../setup/manage-data-connection.md#scheduling) gids beheren.
* De splitsingen van het krediet tussen medewerkers worden nu geplaatst voor elk gebruiksgeval dat binnen de verbinding wordt geselecteerd. U kunt verschillende regels voor kredietverbruik instellen voor elk geval van gebruik om beter te kunnen bepalen hoe je crediteringen worden gebruikt. Meer over de functie van de creditspleet leren, lees de [ gids van verbindingsmontages ](../connect/establishing-connections.md#connection-settings). Om meer over te leren hoe de kredieten worden verbruikt, lees de [ gids van de kredietactiviteit ](../setup/my-activity.md#types-of-activities). <br> ![ het montagesscherm dat van de Verbinding de functionaliteit van de creditsplits toont.](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* Uitgevers kunnen nu namen en id&#39;s van adverteerders instellen voordat ze de verbindingsinstellingen van een adverteerder accepteren. Uitgevers kunnen namen en id&#39;s instellen die worden uitgelijnd op hun interne systemen. Deze namen kunnen verschillen van de namen en id&#39;s van de adverteerder. Meer over het toevoegen van adverteerdernamen en IDs leren, lees de [ gids van verbindingsmontages ](../connect/establishing-connections.md#connection-settings.md). <br> ![ het montagesscherm dat van de Verbinding de uitgever toont die adverteerdernamen en IDs plaatsen.](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## April 2025 {#april-2025}

* Er is een nieuwe kolom **[!UICONTROL Inputs Processed]** toegevoegd aan de tabel met kredietverbruiksactiviteiten. In deze kolom wordt het totale aantal inputs (bijvoorbeeld id&#39;s of rijen) weergegeven dat voor elke activiteit is verwerkt. [ las meer ](/help/guide/setup/my-activity.md#inputs-processed). <br> ![ Inputs verwerkte kolom die in Mijn activiteitenmening wordt benadrukt.](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* Er is een nieuwe e-mailoptie voor contact toegevoegd aan het maken van een account. Dit helpt de medewerkers van de partner uit u bereiken zoals nodig tijdens het verbindingsproces. [Meer informatie](../setup/onboard-account.md).

## Maart 2025 {#march-2025}

* Wanneer [ het sourcen publiek ](/help/guide/setup/onboard-audiences.md) in Collaboration, kunt u een publiek nu plaatsen verfrist frequentie van **elke tot zes dagen** om de [ de kredietactiviteit van het Beheer van de Publiek ](/help/guide/setup/my-activity.md#types-of-activities) beter te beheren. Voor meer informatie, leest [ publiek ](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences) gids beheren. <br> ![ het scherm dat van het Programma verschillende frequentiedetails voor het bijwerken van publiekslidmaatschap toont.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png " het scherm dat van het Programma verschillende frequentiedetails voor het bijwerken van publiekslidmaatschap toont."){width="250" align="center" zoomable="yes"}
* Wanneer het vestigen van een verbinding met een medewerker, kunt u van vooraf bepaalde **gebruiksgevallen** nu selecteren. De geselecteerde gebruikscase bepaalt welke projectsecties en productfunctionaliteit beschikbaar worden. Voor meer informatie, lees [ projecten ](/help/guide/collaborate/manage-projects.md#project-use-cases) gids leiden.
   * *Metingen* laat de **sectie van het het projectproject van de Maatregel** toe.
   * *de ontdekking van het publiek* laat **toe ontdekt** projectsectie.
   * *activering van het publiek* laat **toe activeert** projectsecties <br>
* U kunt nu verbindingen verwijderen met deelnemers waarmee u niet meer wilt werken. Leren hoe te om verbindingen te schrappen, lees [ schrappend verbindingen ](/help/guide/connect/establishing-connections.md#delete-connections) gids.

## Februari 2025 {#february-2025}

Adobe Real-Time CDP Collaboration, dat speciaal is ontworpen om adverteerders en uitgevers in staat te stellen hoogwaardig publiek zonder cookies van derden te detecteren, activeren en meten, is nu in de Verenigde Staten algemeen beschikbaar.

### Aan de slag

1. **Opstelling van de Toegang**: De beheerders van het systeem vormen toegangstoestemmingen voor gebruikers. Meer leren over het vormen van toegangstoestemmingen, leest [ gebruikerstoegang ](/help/guide/permissions/manage-user-access.md#RTCDP-collaboration-access) gids.
2. **verbind Gegevensbronnen**: Het publiek van Source aan gebruik in Collaboration. Beginnen bronsend publiek, lees de [ bron en beheer publiek ](/help/guide/setup/onboard-audiences.md) gids.
3. **Vestig Verbindingen**: Begin werkend met vertrouwde op adverteerders of uitgevers. Meer leren over het vormen van verbindingen, lees [ het vestigen van verbindingen ](/help/guide/connect/establishing-connections.md) gids.
4. **ontdekt en activeert**: Creeer projecten om waardevolle publiek te identificeren in campagnes te activeren. Meer leren over het creëren van projecten, lees [ projecten ](/help/guide/collaborate/manage-projects.md) gids leiden.

### Beschikbaarheid

* Adobe Real-Time CDP Collaboration is momenteel alleen beschikbaar voor klanten in de VS.
* Deze service is automatisch beschikbaar voor Adobe Real-Time CDP Prime- en Ultimate-klanten

Lees voor meer informatie het volgende:

* [Collaboration-overzicht](/help/guide/home.md)
* [End-to-end workflow](/help/guide/overview/end-to-end-workflow.md)
* [Overzicht van machtigingen](/help/guide/permissions/overview.md)
