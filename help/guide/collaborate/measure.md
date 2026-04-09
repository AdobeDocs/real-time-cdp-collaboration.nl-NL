---
title: Prestaties meten
description: Meet de prestaties van uw campagnes over verschillende kanalen. Leer hoe u verschillende rapporten kunt gebruiken en interpreteren.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: c92b263e-1f96-49f1-841a-ef2e97a4cb9a
source-git-commit: 0cf888e36ffc4730fc8de4d8adccae0e0fc2caa8
workflow-type: tm+mt
source-wordcount: '1868'
ht-degree: 0%

---

# Prestaties meten

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>De **[!UICONTROL Measure]** werkruimte is slechts beschikbaar als het **2} gebruiksgeval van de Meting {tijdens het verbindingsproces ](../connect/establishing-connections.md#connection-settings) werd toegelaten.**[Voor meer informatie over gebruiksgevallen, verwijs naar [ projecten ](./manage-projects.md#project-use-cases) gids beheren.

Leer meer over de beschikbare rapporten in Adobe Real-Time CDP Collaboration en begrijp hoe u de prestaties van uw marketingcampagnes op verschillende kanalen kunt meten en analyseren.

## Vereisten {#prerequisites}

Voordat u de meetrapporten in Collaboration kunt openen, moet u:

* [ verbindt ](/help/guide/connect/establishing-connections.md) met een medewerker met **toegelaten het gebruiksgeval van de Meting**
* Werk aan minstens één project met uw medewerker samen. Leer hoe te om [ een project ](/help/guide/collaborate/manage-projects.md#create-project) tot stand te brengen.
* Stel uw campagne in werking en zorg a [ identiteitskaart van de Campagne voor de campagne ](../collaborate/manage-projects.md#manage-campaign-id) wordt verstrekt:
   * Als u een uitgever bent, voert u de campagne-id in die is gekoppeld aan de campagne van uw adverteerder.
   * Als u een adverteerder bent, vraagt u dat uw medewerker (uitgever) de campagne-id opgeeft. Dit wordt vereist om [ rapporten in de werkruimte van de Maatregel ](#create-measurement-report) te produceren.
* [ uploadt metingsgegevens ](/help/guide/setup/onboard-measurement-data.md) in Collaboration als u [ tot de rapporten van de Attributie ](#create-attribution-report) wilt leiden.

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

1. Navigeer naar **[!UICONTROL Collaborate]** > **[!UICONTROL My projects]** .
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

### Cumulatieve omzettingen {#cumulative-conversions}

In deze weergave ziet u een gedetailleerde uitsplitsing van de conversiegebeurtenissen die u in tabelvorm wilt meten. De tabel bevat:

* **gebeurtenis van de Omzetting**: Naam van elke omzettingsgebeurtenis u volgt.
* **Aantal van de Omzetting**: Totale telling van omzettingen die voor elke gebeurtenis voorkwamen.
* **Geschatte opbrengst**: Geschatte waarde die aan elke omzettingsgebeurtenis wordt toegeschreven.

Bekijk deze tabel om de doeltreffendheid van uw campagne voor het aansturen van de gewenste acties te evalueren.

![ Cumulatieve omzettingen.](/help/assets/collaborate/measure/cumulative-conversions.png)

### Omzetten naar dag {#conversions-by-day}

Dit diagram geeft een dagelijkse uitsplitsing van conversies voor elke gebeurtenisinstelling wanneer u een Attributierapport maakt. In deze weergave kunt u dagelijkse patronen onthullen, perioden met een hoge of lage conversieactiviteit identificeren en vergelijken hoe verschillende conversiegebeurtenissen in de tijdlijn van de campagne worden uitgevoerd.

![ Omzettingen door dag.](/help/assets/collaborate/measure/conversions-by-day.gif)

## Metingsrapport maken {#create-measurement-report}

In Collaboration kunt u twee hoofdtypen meetrapporten maken:

* **Samenvatting van de Campagne**: Verstrekt high-level metriek zoals bereik, indrukkingen, gemiddelde frequentie, en levering door kanaal, die een snel overzicht van algemene campagneprestaties geven.
* **Attributie**: Meet hoe de campagneblootstelling stroomafwaartse acties zoals omzettingen of aankopen drijft, die u helpen campagnedoeltreffendheid begrijpen.

U kunt het Rapport van het Overzicht van de Campagne op zijn eigen in werking stellen, terwijl het rapport van de Attributie beide rapporttypes vereist samen worden geselecteerd.

### Samenvattingsrapport campagne maken {#create-campaign-summary-report}

Zowel kunnen uitgevers als adverteerders **rapporten van de Samenvatting van de Campagne van 0} produceren om campagneprestaties te evalueren.** Gebruik deze rapporten om inzichten in zeer belangrijke metriek zoals [ bereiken ](#cumulative-reach-curve), [ frequentie ](#frequency-distribution), en [ impressies ](#impressions-by-placement) te bereiken, en te begrijpen hoe uw campagne en zijn algemeen effect werd geleverd.

Om a **Samenvatting van de Campagne** rapport te produceren, navigeer aan de projectwerkruimte van de **[!UICONTROL Collaborator]** werkruimte. Van het **[!UICONTROL Measure]** lusje, selecteer het add pictogram (![ voeg pictogram toe.](/help/assets/icons/plus.png)) en selecteer vervolgens **[!UICONTROL Measure]** .

Als dit uw eerste rapport is, kunt u ook de optie **[!UICONTROL Run report]** selecteren.

![ het lusje van de Maatregel die de het rapportoptie van de Looppas en de optie van de Maatregel benadrukt.](/help/assets/collaborate/measure/run-measure-report.png)

Het scherm **[!UICONTROL Create measurement report]** wordt weergegeven met informatie en invoervelden die zijn gegroepeerd onder de secties **[!UICONTROL Billing details]** , **[!UICONTROL Campaign details]** en **[!UICONTROL Report details]** .

#### Factuurgegevens {#billing-details}

In deze sectie wordt uitgelegd hoe credits worden gebruikt bij het genereren van meetrapporten. De verantwoordelijkheid van het krediet wordt gevestigd tijdens [ verbindingsopstelling ](../connect/establishing-connections.md#credit-split). Alvorens om het even welke rapporten in werking te stellen, zorg ervoor om de montages van de creditsplits en het melden van rollen met uw medewerker te herzien en te bevestigen.

#### Campagnegegevens {#campaign-details}

In de **[!UICONTROL Campaign details]** sectie, selecteer aangewezen **Advertiser identiteitskaart** aan vennoot met uw rapport. Deze adverteerdernamen of IDs werden toegevoegd tijdens [ verbindingsopstelling ](../connect/establishing-connections.md#advertiser-names). Als slechts één naam werd gevormd, verschijnt het door gebrek. Als er geen naam is ingesteld, wordt het veld **[!UICONTROL Advertiser ID (Name)]** uitgeschakeld en voorgevuld met de naam van het adverteerderaccount.

![ het Create scherm van het metingsrapport dat Advertiser identiteitskaart (Naam) gehandicapte optie toont.](/help/assets/collaborate/measure/advertiser-id.png)

Selecteer vervolgens de gewenste campagne in het vervolgkeuzemenu **[!UICONTROL Campaign ID]** . Dit menu maakt een lijst van alle campagne IDs ingegaan door de uitgever voor uw project. Als de campagne u nodig hebt niet beschikbaar is, [ voeg het in UI ](./manage-projects.md#manage-campaign-id) toe alvorens het rapport te produceren.

![ creeer het Create scherm van het metingsrapport dat dropdown menu toont van identiteitskaart van de Campagne uitgevouwen.](/help/assets/collaborate/measure/campaign-id.png)

Geef vervolgens de periode op die door het rapport moet worden gedekt. Selecteer **[!UICONTROL Report date range]** en kies vervolgens de begin- en einddatum in de kalender.

![ het Create scherm van het metingsrapport dat de kalender van de de datumwaaier van het Rapport toont.](/help/assets/collaborate/measure/report-date-range.png)

#### Rapportdetails {#report-details}

**looppas van het Rapport datum**

Kies in de sectie **[!UICONTROL Report details]** de datum waarop het rapport moet worden uitgevoerd. Selecteer **[!UICONTROL Report run date]** en kies de gewenste datum in de kalender.

* Als u de datum van vandaag of een datum in het verleden kiest, loopt het **Samenvatting van de Campagne** rapport weg.
* Als u een toekomstige datum kiest, is het **Samenvatting van de Campagne** rapport gepland om op die dag te lopen.

![ creeer het Create scherm van het metingsrapport dat de Kalender van de looppas van het Rapport toont.](/help/assets/collaborate/measure/report-run-date.png)

**Type van Rapport**

* Als u een adverteerder bent, kunt u het rapporttype van **[!UICONTROL Campaign summary]** van de beschikbare opties selecteren. Alleen adverteerders kunnen attributierapporten genereren.
* Als u een uitgever bent, is het rapporttype van **[!UICONTROL Campaign summary]** vooraf geselecteerd en kan niet worden veranderd. Op dit moment kunnen uitgevers geen toewijzingsrapporten uitvoeren.

![ het Create scherm van het metingsrapport dat de summiere optie van de Campagne als vooraf geselecteerd en onveranderbaar rapporttype toont.](/help/assets/collaborate/measure/cs-report-type.png)

Controleer ten slotte uw instellingen en selecteer **[!UICONTROL Create]** . Het samenvattingsrapport van uw campagne wordt onmiddellijk gegenereerd als de runtime vandaag of eerder is of op de gekozen toekomstige datum. U kunt het geplande rapport vóór de runtime bewerken. Voor geleidelijke instructies, verwijs naar [ uitgeef metingsrapport ] sectie.

Zodra beschikbaar, kunt u uw rapport op elk ogenblik in het **[!UICONTROL Measure]** lusje binnen uw projectwerkruimte bekijken.

![ het Create scherm van het metingsrapport dat de informatie en de Create benadrukte optie toont.](/help/assets/collaborate/measure/cs-review.png)

### Toewijzingsrapport maken {#create-attribution-report}

Als adverteerder, kunt u **rapporten van de Attributie** produceren om te beoordelen hoe uw campagneblootstelling aan zeer belangrijke resultaten zoals sign-ups of aankopen bijdraagt. Gebruik deze rapporten om gebruikersinteractie met uw campagne te begrijpen, te identificeren welke aanraakpunten de meeste impact hebben, en effectievere marketing strategieën te informeren.

>[!IMPORTANT]
>
> U moet [ uw metingsgegevens ](../setup/onboard-measurement-data.md#add-measurement-data) in Collaboration bron alvorens de rapporten van de Attributie te produceren.
>![Het lusje van de Maatregel met de vereisten voor de gegevens van de Meting en de gehandicapte optie van de Maatregel.](/help/assets/collaborate/measure/require-measurement-data.png)

Om een **rapport van de Attributie** te produceren, navigeer aan de projectwerkruimte van de **[!UICONTROL Collaborator]** werkruimte. Van het **[!UICONTROL Measure]** lusje, selecteer het add pictogram (![ voeg pictogram toe.](/help/assets/icons/plus.png)) en selecteer vervolgens **[!UICONTROL Measure]** .

Als dit uw eerste rapport is, kunt u ook de optie **[!UICONTROL Run report]** selecteren.

![ het lusje van de Maatregel die de het rapportoptie van de Looppas en de optie van de Maatregel benadrukt.](/help/assets/collaborate/measure/run-measure-report-attribution.png)

Het scherm **[!UICONTROL Create measurement report]** wordt weergegeven met informatie en invoervelden die zijn gegroepeerd onder de secties **[!UICONTROL Billing details]** , **[!UICONTROL Campaign details]** en **[!UICONTROL Report details]** .

Lees en volg stappen in [ creeer het rapport van de campagneresamenvatting ](#create-campaign-summary-report) sectie om de volgende montages te vormen:

* [ het Factureren details ](#billing-details)
* [Campagnegegevens](#campaign-details)

#### Details rapporteren voor Attributen rapporten {#report-details-attribution}

**looppas van het Rapport datum**

>[!IMPORTANT]
>
> Voor attributierapporten, moet de rapportloopdatum een toekomstige datum zijn, en moet minstens één dag na de einddatum van uw waaier van de rapportdatum plus de volledige duur van het bepaalde raadplegingsvenster voorkomen.
> **looppas van het Rapport datum ≥ rapporteinddatum + raadplegingsvenster + 1**
> 
> Bijvoorbeeld, als uw waaier van de rapportdatum op 15 Juni beëindigt en het raadplegingsvenster 14 dagen is, is de datum van de rapportlooppas 30 Juni of later.

Kies in de sectie **[!UICONTROL Report details]** de datum waarop het rapport moet worden uitgevoerd. Selecteer **[!UICONTROL Report run date]** en kies de gewenste datum in de kalender.

**Type van Rapport**

Als adverteerder kunt u naast **[!UICONTROL Campaign summary]** ook **[!UICONTROL Attribution]** als rapporttype selecteren. Wanneer u het rapport van de Attributie kiest, omvatten uw resultaten zowel standaard de Summiere metriek van de Campagne als gedetailleerde analyse van de Attributie, die een uitvoerige mening van campagneprestaties verstrekken.

![ creeer het Create scherm van het metingsrapport dat zowel de de samenvatting van de Campagne als geselecteerde het rapporttypes van de Attributie benadrukt.](/help/assets/collaborate/measure/attribution-report-type.png)

Wanneer u **[!UICONTROL Attribution]** als rapporttype selecteert, wordt een **[!UICONTROL Attribution]** -configuratiesectie weergegeven met aanvullende vereiste instellingen:

* **venster van de Lookback in dagen**: Bepaalt hoe ver achter het rapport campagnebeelden vóór elke omzetting overweegt. Alleen indrukkingen binnen deze periode komen in aanmerking voor creditering.
* **de gebeurtenissen van de Omzetting**: Specificeert welke omzettingsacties u, bijvoorbeeld, aankopen of sign-ups wilt meten. Deze gebeurtenissen moeten opstelling vooraf zijn wanneer u [ uw metingsgegevens ](../setup/onboard-measurement-data.md#add-conversion-event) in Collaboration bron.

Voer eerst een waarde in voor het veld **[!UICONTROL Lookback window in days]** of pas deze aan met de opties voor verhogen/verlagen.

![ het Create scherm van het metingsrapport dat de waarde voor venster van de Lookback in dagen benadrukt.](/help/assets/collaborate/measure/lookback-window-in-days.png)

Daarna, kies tot **3** omzettingsgebeurtenissen van de beschikbare lijst. Voor meer informatie over een bepaalde gebeurtenis selecteert u het pictogram **[!UICONTROL i]** om de details ervan weer te geven.

![ het Create scherm van het metingsrapport dat de geselecteerde omzettingsgebeurtenissen en de informatie van de gebeurtenis van de Aankoop benadrukt.](/help/assets/collaborate/measure/attribution-conversion-events.png)

Controleer ten slotte uw instellingen en selecteer **[!UICONTROL Create]** om het rapport te plannen. Uw toewijzingsrapport wordt gegenereerd op de opgegeven uitvoeringsdatum. U kunt het geplande rapport vóór de runtime bewerken. Voor geleidelijke instructies, verwijs naar [ uitgeef metingsrapport ] sectie.

Zodra beschikbaar, kunt u uw rapport op elk ogenblik in het **[!UICONTROL Measure]** lusje binnen uw projectwerkruimte bekijken.

![ het Create scherm van het metingsrapport dat de informatie en de Create benadrukte optie toont.](/help/assets/collaborate/measure/attribution-review.png)
