---
title: Je activiteiten op het gebied van kredietverbruik volgen
description: Leer hoe u de activiteiten van uw organisatie op het gebied van kredietverbruik in Real-Time CDP Collaboration kunt volgen.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/nl/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: b24d63e7-60f4-4cdb-ab1b-77c284543486
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# Je activiteiten op het gebied van kredietverbruik volgen

{{limited-availability-release-note}}

>[!BEGINSHADEBOX]

**90 dag geen-overlijdende Periode**: De klanten in in in aanmerking komende gebieden profiteren van een periode van 90 dag geen-overouderd die van de datum van beschikbaarheid in hun gebied begint. Gedurende deze periode betalen klanten geen overloopkosten voor het overschrijden van hun kredietrecht.

>[!ENDSHADEBOX]

>[!IMPORTANT]
>
>De tabel van het kredietverbruik wordt voor toezicht naar boven afgerond en naar dag geaggregeerd. De cijfers in het **[!UICONTROL My Activity]** dashboard vertegenwoordigen een *geschat* kredietconsumptie. Het *daadwerkelijke* kredietverbruik dat voor het factureren wordt gebruikt wordt gevolgd in interne systemen en is beschikbaar aan u op verzoek. Neem contact op met uw Adobe-vertegenwoordiger voor deze informatie.

Navigeer naar **[!UICONTROL Setup]** in de hoofdnavigatie en selecteer vervolgens het tabblad **[!UICONTROL My activity]** om uw geschatte activiteiten voor kredietverbruik te openen.

![ Mijn dashboard van de Activiteit die de details van de kredietconsumptie tonen ](/help/assets/setup/my-activity-credits/activity-dashboard.png)

>[!TIP]
>
>De weergave **[!UICONTROL My activity]** bevat geen informatie over gebruikersacties in verschillende delen van de gebruikersinterface van Collaboration. Gebruik de [ controlelogboeken ](/help/guide/setup/audit-logs.md) functionaliteit om die informatie te krijgen.

## Het dashboard voor uw activiteiten begrijpen {#understand-dashboard}

Het activity dashboard geeft een uitgebreide lijst weer van alle kredietverbruikende bewerkingen in uw account. Elke rij vertegenwoordigt een afzonderlijke activiteit en verstrekt zeer belangrijke informatie over het kredietgebruik:

>[!NOTE]
>
>**[!UICONTROL Audience Management]** -activiteiten zijn niet gekoppeld aan een andere deelnemer, zodat de kolommen **[!UICONTROL Connection ID]** en **[!UICONTROL Connection name]** voor deze typen activiteiten een **[!UICONTROL -]** -waarde aangeven.

| Kolom | Beschrijving |
|------------|--------------|
| **[!UICONTROL Date]** | De datum waarop de activiteit plaatsvond, weergegeven in de notatie MM/DD/JJJJ. |
| **[!UICONTROL Connection ID]** | Een unieke id voor elke verbinding die aan een kredietverbruikende activiteit is gekoppeld, weergegeven als een alfanumerieke tekenreeks. |
| **[!UICONTROL Connection name]** | De naam van de medewerker die is gekoppeld aan de verbinding en de kredietverslindende activiteit. |
| **[!UICONTROL Activity]** | Het type van uitgevoerde activiteit, zoals **Activering - het Aanpassen**, **Activering - uitgang**, of **Beheer van het Publiek**. |
| **[!UICONTROL Inputs processed]** | Het totale aantal inputs (bijvoorbeeld id&#39;s of rijen) dat voor de activiteit is verwerkt. |
| **[!UICONTROL Total credits used]** | Het totale aantal kredieten dat door de activiteit wordt verbruikt. |
| **[!UICONTROL My credit share]** | Het gedeelte van je account van de credits die voor de activiteit worden gebruikt. |

{style="table-layout:auto"}

## Soorten activiteiten {#types-of-activities}

In de kolom **[!UICONTROL Activity]** worden verschillende soorten kredietverbruikende bewerkingen weergegeven.

* **[!UICONTROL Audience Management]**: Credits worden gebruikt wanneer het publiek naar Collaboration wordt gedownload. Credits worden verbruikt als een functie van het aantal id&#39;s (in miljoenen) dat binnen Collaboration is geïndexeerd voor alle soorten publiek en de frequentie van die indexering (dagelijks, elke drie dagen of wekelijks). Meer leren, lees [ het aantrekken en het leiden van publiek ](/help/guide/setup/onboard-audiences.md) gids.
* **[!UICONTROL Activation - Matching]** - Credits worden gebruikt als een functie van het aantal id&#39;s dat overeenkomt en klaar is voor activering. Meer leren, lees [ activerend publiek ](/help/guide/collaborate/activate.md) gids.
* **[!UICONTROL Activation - Egress]** - Credits worden gebruikt als functie van het aantal id&#39;s dat naar een doel wordt verzonden. Dit wordt altijd in rekening gebracht aan de medewerker die het publiek ontvangt. Meer leren, lees [ activerend publiek ](/help/guide/collaborate/activate.md) gids.
* **[!UICONTROL Measurement]** - Voer activiteiten uit in Collaboration om prestatierapporten en inzichten van de campagne te genereren. Kredieten worden verbruikt op basis van het aantal rijen in campagnerapporten voor alle campagnes en de rapportagefrequentie (dagelijks, elke drie dagen of wekelijks).

## Uw kredietverbruik beheren {#manage-credit-consumption}

Om uw kredietverbruik effectief te beheren:

1. **begrijp** het kredietverbruik verbonden aan elke activiteit. Controleer de [ het productbeschrijving van Collaboration ](https://helpx.adobe.com/nl/legal/product-descriptions/real-time-customer-data-platform-collaboration.html){target=_blank} voor een lijst van kredieten die per activiteit worden gebruikt.
2. **Monitor regelmatig**: Controleer regelmatig uw activiteitendashboard om gebruikspatronen te begrijpen.
3. **Spoor door verbinding**: Gebruik de verbindingsnaam om te identificeren welke verbindingen de meeste kredieten verbruiken.
