---
title: Prestaties meten
description: Meet de prestaties van uw campagnes over verschillende kanalen. Leer hoe u verschillende rapporten kunt gebruiken en interpreteren.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: c92b263e-1f96-49f1-841a-ef2e97a4cb9a
source-git-commit: b69d204149f203d1950fd0e28b0858ffca2c1225
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 0%

---

# Prestaties meten

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>De **[!UICONTROL Measure]** werkruimte is slechts beschikbaar als het **2&rbrace; gebruiksgeval van de de meetmethode van de Campagne [ tijdens het verbindingsproces ](../connect/establishing-connections.md#connection-settings) werd toegelaten.** Voor meer informatie over gebruiksgevallen, verwijs naar [ projecten ](./manage-projects.md#project-use-cases) gids beheren.

Leer meer over de beschikbare rapporten in Real-Time CDP Collaboration en begrijp hoe u de prestaties van uw marketingcampagnes op verschillende kanalen kunt meten en analyseren.

## Vereisten

Voordat u de meetrapporten in Real-Time CDP Collaboration kunt openen, hebt u al het volgende:

* [ Verbonden ](/help/guide/connect/establishing-connections.md) met een gewenste adverteerder of uitgever met de **meting van de Campagne** toegelaten gebruiksgeval en begonnen samenwerkend op [ projecten ](/help/guide/collaborate/manage-projects.md)
* Stel een campagne in werking en [ geüploade metingsgegevens ](/help/guide/setup/onboard-measurement-data.md) in Real-Time CDP Collaboration.

<!--

## Create a report {#create-report}

Hidden until functionality is live. At that point, move the contextualhelp from below into this section. 

The syntax rtcdp_collaboration_measurement_create_report is currently implemented in the UI. However, a preference would be to imlement the other contextualhelp ID from below instead, since that explicitly includes campaignID in the syntax. Need to sync up with UI team. More details in CORE-116991.

-->

## Rapporten weergeven {#view-reports}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measurement_create_report_campaignID"
>title="Campagne-id&#39;s"
>abstract="Tijdelijke aanduiding om relevante informatie in de gebruikersinterface toe te voegen over wat de campagne-id&#39;s zijn."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measurement_create_report"
>title="Campagne-id&#39;s"
>abstract="Tijdelijke aanduiding om relevante informatie in de gebruikersinterface toe te voegen over wat de campagne-id&#39;s zijn."

U kunt als volgt de rapporten weergeven die beschikbaar zijn op het tabblad Metingen:

1. Ga naar **[!UICONTROL Collaborate]** > **[!UICONTROL My projects]**.
2. Selecteer **[!UICONTROL View]** voor het gewenste project.
3. Selecteer in het project de tab **[!UICONTROL Measure]** .

Selecteer **[!UICONTROL View full report]** om toegang te krijgen tot de verschillende beschikbare rapporten, die hieronder nader worden beschreven.

![ hoe te om aan het metingslusje in een project te krijgen.](/help/assets/collaborate/measure/measurement.gif)

### Samenvattingsweergave

In de paginaopmaakweergave op het tabblad Meting wordt een campagneresamenvatting weergegeven met een aantal cijfers op hoog niveau waarnaar u kunt verwijzen:

**[!UICONTROL Impressions]**: Het totale aantal keren dat het creatieve bestand is weergegeven.
**[!UICONTROL Unique reach]**: Het aantal individuele identiteiten dat de creatieve persoon heeft gezien.
**[!UICONTROL Total average frequency]**: Het aantal afbeeldingen gedeeld door de unieke identiteiten die zijn bereikt. Dit cijfer wijst erop hoe vaak elke identiteit creatief werd getoond.

![ de summiere mening van de Campagne ](/help/assets/collaborate/measure/campaign-summary.png)

### Metrisch in de loop der tijd {#metrics-over-time}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_measure_metricsovertime"
>title="Metrisch in de loop der tijd"
>abstract="Met de metrische gegevens in de tijdweergave krijgt u inzicht in het totale aantal indrukken dat gedurende de campagne voor uw creatieve project wordt weergegeven. U kunt maximaal twee dimensies selecteren om in het rapport weer te geven."

Met de metrische gegevens in de tijdweergave krijgt u inzicht in het totale aantal indrukken dat gedurende de campagne voor uw creatieve project wordt weergegeven. Merk op dat u een maximum van twee metriek kunt selecteren om in het rapport te tonen en te analyseren.

![ Metriek over tijdmening.](/help/assets/collaborate/measure/metrics-over-time.png)

### Frequentieverdeling {#frequency-distribution}

Gebruik de mening van de frequentieverdeling om de verdeling van te begrijpen hoeveel indrukkingen aan elke unieke gebruiker werden getoond. Met deze weergave kunt u in toekomstige campagnes bepalen vanaf welk punt u het publiek wilt onderdrukken. U kunt bijvoorbeeld profielen onderdrukken die al drie keer creatief zijn geweest.

![ de distributiemening van de Frequentie.](/help/assets/collaborate/measure/frequency-distribution.gif)

### Metrisch per dimensie {#metric-by-dimension}

Analyseer verschillende metriek zoals impressies, viewable beelden, uniek bereik, kosten, en meer in de context van het plaatsingsmiddel. Analyseer welk medium (bijvoorbeeld mobiel streamen, CTV programmatic of andere) de beste resultaten voor uw campagnes geeft.

![ Metrisch door dimensie.](/help/assets/collaborate/measure/metric-by-dimension.png)

### Cumulatieve bereikcurve {#cumulative-reach-curve}

Naarmate de campagne vorderde en het aantal indrukken toenam, begrijpt u of het aantal gebruikers dat u kon bereiken, ook is toegenomen. Een gemeenschappelijk patroon in campagnes is dat na een bepaald punt een plateau wordt bereikt waar creatief wordt getoond aan de zelfde mensen telkens opnieuw. Deze weergave kan u helpen de duur van toekomstige campagnes aan te passen, afhankelijk van het moment dat nieuwe mensen niet meer werden bereikt.

![ Cumulatieve bereikkromme.](/help/assets/collaborate/measure/cumulative-reach-curve.png)

### Impressies door plaatsing {#impressions-by-placement}

Begrijp welk medium indrukkingen veroorzaakt voor uw creatieve projecten. Zo kunt u bepalen waar u uw advertentie wilt investeren in toekomstige campagnes.

![ Impressies door plaatsing.](/help/assets/collaborate/measure/impressions-by-placement.png)

## Volgende stappen

![ ontdekt, activeert, maatregel voor adverteerders.](/help/assets/end-to-end-workflow/discover-activate-measure.png)

In de geest van de conjunctuur in het bovenstaande beeld, gebruik de inzichten u van het bekijken van de rapporten bij het plannen van uw volgende campagne verwierf. Ga als adverteerder, indien nodig, terug om verschillende uitgevers te ontdekken en looppas overlappingen om verschillende soorten publiek voor uw volgende campagnes te ontdekken.
