---
title: Opmerkingen bij de nieuwste Real-Time CDP Collaboration-release
description: Volg de nieuwste releases voor Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 8513c648-1cc1-4544-b86d-2ee3193ab60f
source-git-commit: 92e347e3258817a983d8eaed9cf2b962b3443cbc
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 3%

---

# Opmerkingen bij de nieuwste Real-Time CDP Collaboration-release

{{limited-availability-release-note}}

**Laatste update**: April, 2025.

Deze releaseopmerkingen betreffen de functionaliteit die in Real-Time Customer Data Platform Collaboration wordt vrijgegeven. Real-Time CDP Collaboration-releases werken op een doorlopend leveringsmodel, dat een gemiddelde maandelijkse release mogelijk maakt. Deze releaseopmerkingen worden vaak bijgewerkt, dus zorg ervoor dat u ze regelmatig controleert.

## Mei 2025 {#may-2025}

* Real-Time CDP Collaboration is nu beschikbaar aan klanten in **Australië** en **Nieuw Zeeland**. Deze service is automatisch beschikbaar voor Real-Time CDP Prime- en Ultimate-klanten in deze regio&#39;s.
* Real-Time CDP Collaboration biedt nu [ zelf-dient bestemmingen ](../setup/manage-destinations.md) door het Mijn bestemmingslusje in de sectie van de Opstelling aan. Met doelen kunt u het publiek activeren op externe platforms, zoals advertentienetwerken of platforms voor gegevensbeheer, zodat u uw klanten op verschillende kanalen kunt bereiken. Momenteel worden alleen Adobe Experience Platform-doelen ondersteund. Neem contact op met uw Adobe-vertegenwoordiger als u een andere bestemming wilt configureren. Meer over bestemmingen leren, lees de [ gids van het bestemmingsoverzicht ](../destinations/overview.md).

   * De bestemmingen voegen ook steun toe om het publiek van Real-Time CDP Collaboration in het [ het publieksportaal van Adobe Experience Platform ](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences.) te bekijken.

* U kunt de publieksvernieuwingsfrequentie voor bestaande gegevensverbindingen in Real-Time CDP Collaboration nu bewerken. Op dit moment kunt u ervoor kiezen uw publiek dagelijks of om de twee tot zes dagen te vernieuwen. Meer over leren hoe te om het publiek uit te geven verfrist frequentie, leest [ gegevensverbindingen ](../setup/manage-data-connection.md#scheduling) gids beheren.
* De splitsingen van het krediet tussen medewerkers worden nu geplaatst voor elk gebruiksgeval dat binnen de verbinding wordt geselecteerd. U kunt verschillende regels voor kredietverbruik instellen voor elk geval van gebruik om beter te kunnen bepalen hoe je crediteringen worden gebruikt. Meer over de functie van de creditspleet leren, lees de [ gids van verbindingsmontages ](../connect/establishing-connections.md#connection-settings). Om meer over te leren hoe de kredieten worden verbruikt, lees de [ gids van de kredietactiviteit ](../setup/my-activity.md#types-of-activities). <br> ![ het montagesscherm dat van de Verbinding de functionaliteit van de creditsplits toont.](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* Uitgevers kunnen nu namen en id&#39;s van adverteerders instellen voordat ze de verbindingsinstellingen van een adverteerder accepteren. Uitgevers kunnen namen en id&#39;s instellen die worden uitgelijnd op hun interne systemen. Deze namen kunnen verschillen van de namen en id&#39;s van de adverteerder. Meer over het toevoegen van adverteerdernamen en IDs leren, lees de [ gids van verbindingsmontages ](../connect/establishing-connections.md#connection-settings.md). <br> ![ het montagesscherm dat van de Verbinding de uitgever toont die adverteerdernamen en IDs plaatsen.](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## April 2025 {#april-2025}

* Er is een nieuwe kolom **[!UICONTROL Inputs Processed]** toegevoegd aan de tabel met kredietverbruiksactiviteiten. In deze kolom wordt het totale aantal inputs (bijvoorbeeld id&#39;s of rijen) weergegeven dat voor elke activiteit is verwerkt. [ las meer ](/help/guide/setup/my-activity.md#inputs-processed). <br> ![ Inputs verwerkte kolom die in Mijn activiteitenmening wordt benadrukt.](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* Er is een nieuwe e-mailoptie voor contact toegevoegd aan het maken van een account. Dit helpt de medewerkers van de partner uit u bereiken zoals nodig tijdens het verbindingsproces. [Meer informatie](../setup/onboard-organization.md).

## Maart 2025 {#march-2025}

* Wanneer [ invoerend publiek ](/help/guide/setup/onboard-audiences.md) in Real-Time CDP Collaboration, kunt u een publiek nu plaatsen verfrist frequentie van **elke tot zes dagen** om de [ de kredietactiviteit van het Beheer van de Publiek ](/help/guide/setup/my-activity.md#types-of-activities) beter te beheren. [ las meer ](/help/guide/setup/onboard-audiences.md#schedule). <br> ![ het scherm dat van het Programma verschillende frequentiedetails voor het bijwerken van publiekslidmaatschap toont.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png " het scherm dat van het Programma verschillende frequentiedetails voor het bijwerken van publiekslidmaatschap toont."){width="250" align="center" zoomable="yes"}
* Wanneer het vestigen van een verbinding met een medewerker, kunt u van vooraf bepaalde **gebruiksgevallen** nu selecteren. De geselecteerde gebruikscase bepaalt welke projectsecties en productfunctionaliteit beschikbaar worden. [Meer informatie](/help/guide/collaborate/manage-projects.md#project-use-cases).
   * *de meting van de Campagne* laat de **** projectsectie van de Maatregel toe.
   * *de ontdekking van het publiek* laat **toe ontdekt** projectsectie.
   * *activering van het publiek* laat **toe activeert** projectsecties <br>
* U kunt nu verbindingen verwijderen met deelnemers waarmee u niet meer wilt werken. [Meer informatie](/help/guide/connect/establishing-connections.md#delete-connections).


## Februari 2025 - Algemene beschikbaarheid voor klanten in de VS {#february-2025-ga}

Real-Time CDP Collaboration, dat speciaal is ontworpen om adverteerders en uitgevers in staat te stellen hoogwaardig publiek zonder cookies van derden te detecteren, activeren en meten, is nu in de Verenigde Staten algemeen beschikbaar.

### Aan de slag

1. **Opstelling van de Toegang**: De beheerders van het systeem vormen toegangstoestemmingen voor gebruikers. [Meer informatie](/help/guide/permissions/manage-user-access.md#RTCDP-collaboration-access).
2. **verbind Gegevensbronnen**: De kijkcijfers van de invoer aan gebruik in Real-Time CDP Collaboration. [Meer informatie](/help/guide/setup/onboard-audiences.md).
3. **Vestig de Verbindingen van de Partner**: Begin met het samenwerken met vertrouwde merken of uitgevers. [Meer informatie](/help/guide/connect/establishing-connections.md).
4. **ontdekt en activeert**: Creeer projecten om waardevolle publiekssegmenten te identificeren en in campagnes te activeren. [Meer informatie](/help/guide/collaborate/manage-projects.md).

### Beschikbaarheid

* Real-Time CDP Collaboration is momenteel alleen beschikbaar voor klanten in de VS.
* Deze service is automatisch beschikbaar voor Real-Time CDP Prime- en Ultimate-klanten

Lees voor meer informatie:

* [Real-Time CDP Collaboration-overzicht](/help/guide/home.md)
* [End-to-end workflow](/help/guide/end-to-end-workflow.md)
* [Overzicht van machtigingen](/help/guide/permissions/overview.md)
