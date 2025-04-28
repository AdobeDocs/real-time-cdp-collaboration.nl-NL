---
title: Je activiteiten op het gebied van kredietverbruik volgen
description: Leer hoe u de activiteiten van uw organisatie op het gebied van kredietverbruik in Real-Time CDP Collaboration kunt volgen.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b24d63e7-60f4-4cdb-ab1b-77c284543486
source-git-commit: 3aec9806d2ea920d656bb0981f22ba31fd8ae3ee
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Je activiteiten op het gebied van kredietverbruik volgen

{{limited-availability-release-note}}

Gebruik het tabblad **[!UICONTROL My Activity]** om het geschatte kredietverbruik van uw organisatie voor alle samenwerkingsactiviteiten te controleren en te volgen. Deze functie biedt gedetailleerd inzicht in hoe credits worden gebruikt voor verschillende verbindingen en activiteiten, waardoor u uw bronnen effectief kunt beheren.

>[!IMPORTANT]
>
>De tabel van het kredietverbruik wordt voor toezicht naar boven afgerond en naar dag geaggregeerd. De cijfers in het **[!UICONTROL My Activity]** dashboard vertegenwoordigen een *geschat* kredietconsumptie. Het *daadwerkelijke* kredietverbruik dat voor het factureren wordt gebruikt wordt gevolgd in interne systemen en is beschikbaar aan u op verzoek. Neem contact op met uw Adobe-vertegenwoordiger voor deze informatie.

Navigeer naar **[!UICONTROL Setup]** in de hoofdnavigatie en selecteer vervolgens het tabblad **[!UICONTROL My activity]** om uw geschatte activiteiten voor kredietverbruik te openen.

![ Mijn dashboard van de Activiteit die de details van de kredietconsumptie tonen ](/help/assets/setup/my-activity-credits/activity-dashboard.png)

>[!TIP]
>
>De weergave **[!UICONTROL My activity]** bevat geen informatie over gebruikersacties in verschillende delen van de Collaboration CDP-gebruikersinterface in real-time. Gebruik de [ controlelogboeken ](/help/guide/setup/audit-logs.md) functionaliteit om die informatie te krijgen.

## Het dashboard voor uw activiteiten begrijpen {#understand-dashboard}

Het activity dashboard geeft een uitgebreide lijst weer van alle kredietverbruikende bewerkingen binnen uw organisatie. Elke rij vertegenwoordigt een afzonderlijke activiteit en verstrekt zeer belangrijke informatie over het kredietgebruik:

>[!NOTE]
>
>**[!UICONTROL Audience Management]** -activiteiten zijn niet gekoppeld aan een andere deelnemer, zodat de kolommen **[!UICONTROL Connection ID]** en **[!UICONTROL Connection name]** voor deze typen activiteiten een **[!UICONTROL N/A]** -waarde aangeven.

| Kolom | Beschrijving |
|------------|--------------|
| **[!UICONTROL Date]** | De datum waarop de activiteit plaatsvond, weergegeven in de notatie MM/DD/JJJJ. |
| **[!UICONTROL Connection ID]** | Een unieke id voor elke verbinding die aan een kredietverbruikende activiteit is gekoppeld, weergegeven als een alfanumerieke tekenreeks. |
| **[!UICONTROL Connection name]** | De naam van de medewerker die is gekoppeld aan de verbinding en de kredietverslindende activiteit. |
| **[!UICONTROL Activity]** | Het type van uitgevoerde activiteit, zoals **Activering - het Delen**, **Activering - uitgang**, of **beheer van het Publiek**. |
| **[!UICONTROL Inputs processed]** | Het totale aantal inputs (bijvoorbeeld id&#39;s of rijen) dat voor de activiteit is verwerkt. |
| **[!UICONTROL Total credits used]** | Het totale aantal kredieten dat door de activiteit wordt verbruikt. |
| **[!UICONTROL My credit share]** | Het gedeelte van de credits van uw organisatie dat wordt gebruikt voor de activiteit. |

{style="table-layout:auto"}

## Soorten activiteiten {#types-of-activities}

In de kolom **[!UICONTROL Activity]** worden verschillende soorten kredietverbruikende bewerkingen weergegeven.

* **[!UICONTROL Audience Management]**: Credits worden gebruikt wanneer soorten publiek worden geïmporteerd in Real-Time CDP Collaboration. Credits worden verbruikt als een functie van het aantal id&#39;s (in miljoenen) dat binnen Real-Time CDP Collaboration is geïndexeerd voor alle doelgroepen, en de frequentie van die indexering (dagelijks, elke drie dagen of wekelijks) gedurende de factureringsperiode. Lees meer over [ het invoeren en het leiden van publiek ](/help/guide/setup/onboard-audiences.md).
* **[!UICONTROL Activation - Sharing]** - Credits worden verbruikt als een functie van het aantal id&#39;s dat gedurende de factureringsperiode vanuit Real-Time CDP Collaboration is geactiveerd. Lees meer over [ delend ](/help/guide/collaborate/share.md) en [ activerend publiek ](/help/guide/collaborate/activate.md) in Real-Time CDP Collaboration.
* **[!UICONTROL Activation - Egress]** - Credits worden verbruikt als een functie van het aantal id&#39;s dat gedurende de factureringsperiode vanuit Real-Time CDP Collaboration is geactiveerd. Lees meer over [ delend ](/help/guide/collaborate/share.md) en [ activerend publiek ](/help/guide/collaborate/activate.md) in Real-Time CDP Collaboration.
* **[!UICONTROL Audience Overlaps]** - Kredieten worden gebruikt wanneer het analyseren van publiek overlapt gebruikend gegevensschetsen. De schetsen van gegevens zijn vereenvoudigde samenvattingen van publieksgegevens die helpen bepalen hoe gelijkaardig twee publiek terwijl het handhaven van gegevensprivacy is. Lees meer over [ publiek overlapt in ontdekt lusje ](/help/guide/collaborate/discover.md).
* **[!UICONTROL Audience Measurement]** - Voer activiteiten uit in Real-Time CDP Collaboration om prestatierapporten en inzichten van de campagne te genereren. Kredieten worden verbruikt op basis van het aantal rijen in campagnerapporten voor alle campagnes en de rapportagefrequentie (dagelijks, elke drie dagen of wekelijks).


<!--

**[!UICONTROL Audience Overlaps]** – Credits are consumed as a function of the number of matched IDs across 2 or more shared audiences throughout the billing period. Read more about [audience overlaps in the discover tab](/help/guide/collaborate/discover.md).

Collaboration Measurement – Credits are consumed as a function of the number of rows existing in campaign reports across all campaigns, and the frequency of that reporting (daily, every three days, or weekly).

-->


## Uw kredietverbruik beheren {#manage-credit-consumption}

Om uw kredietverbruik effectief te beheren:

1. **begrijp** het kredietverbruik verbonden aan elke activiteit. Controleer de [ het productbeschrijving van Real-Time CDP Collaboration ](https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html){target=_blank} voor een lijst van samenwerkingskredieten die per activiteit worden gebruikt.
2. **Monitor regelmatig**: Controleer regelmatig uw activiteitendashboard om gebruikspatronen te begrijpen.
3. **Spoor door verbinding**: Gebruik de verbindingsnaam om te identificeren welke partnerschappen de meeste kredieten verbruiken.

<!--

## Pagination and navigation

The activity list is paginated to improve performance and readability. Use the navigation controls at the bottom of the table to move between pages and adjust how many records you can view at once.

-->
