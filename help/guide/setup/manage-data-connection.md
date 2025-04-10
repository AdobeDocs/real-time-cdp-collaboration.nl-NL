---
title: Gegevensverbindingen beheren
description: Leer hoe u gegevensverbindingen beheert, zoals match keys, planning, use cases en publiekfiltering in Real-Time CDP Collaboration
audience: administrator, data engineer
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: acaaaa1e1fab981d874210639c16e76e48fc3394
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Gegevensverbindingen beheren

{{limited-availability-release-note}}

## Overzicht

Gegevensverbindingen gebruiken in Real-Time CDP Collaboration om doelgroepen uit verschillende bronnen te importeren. Meer informatie over het beheren van vergelijkingscodes en het plannen van gegevensimport voor uw bestaande gegevensverbindingen. Bovendien kunt u doelgroepen filteren op verschillende kenmerken voor gedetailleerdere inzichten.

Voordat u uw gegevensverbindingen hier beheert, moet u ze in eerste instantie instellen tijdens de workflow](./onboard-audiences.md) voor het onboarden van het [publiek. Dit zorgt ervoor dat de juiste gegevensbronnen worden aangesloten voor gebruik in Real-Time CDP Collaboration.

## Dataverbindingen bekijken

>[!IMPORTANT]
>
>Het verwijderen van een gegevensverbinding wordt momenteel niet ondersteund in de gebruikersinterface van Real-Time CDP Collaboration. Om een gegevensverbinding te schrappen, te bereiken gelieve uit aan uw vertegenwoordiger van Adobe of [ een kaartje van de klantensteun ](https://experienceleague.adobe.com/home?lang=en&amp;support-tab=open-ticket#support){target="_blank"} tot stand te brengen.

Als u bestaande gegevensverbindingen wilt weergeven, navigeert u naar **[!UICONTROL Setup]** > **[!UICONTROL My audiences]** en selecteert u **[!UICONTROL Manage data connections]** .

![ de werkruimte van de Opstelling met Manage benadrukte gegevensverbindingen.](/help/assets/setup/manage-data-connection/manage-data-connection-highlighted.png){zoomable="yes"}

Dit brengt een mening van al uw momenteel opstellings gegevensverbindingen, met informatie over het aantal publiek in elk van hen, de bron van de gegevensverbinding, en meer. Selecteer deze optie **[!UICONTROL View data connection]** om informatie weer te geven over de vergelijkingssleutels, de planning en de doelgroepen die deel uitmaken van deze gegevensverbinding.

![Werkruimte voor gegevensverbindingen beheren met een verbinding Gegevensverbindingen weergeven gemarkeerd. ](/help/assets/setup/manage-data-connection/view-data-connection-highlighted.png){zoomable="yes"}

### Match sleutels {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="Match sleutels"
>abstract="Vergelijkingssleutels bepalen hoe gegevens uit verschillende bronnen worden gematcht. Kies de matchcodes die het meest relevant zijn voor uw gebruiksscenario&#39;s en privacyrichtlijnen."

Overeenkomstcodes zijn ID&#39;s die worden gebruikt om leden uit verschillende doelgroepen uit verschillende gegevensbronnen met elkaar in contact te brengen. Beschikbare match-sleutels zijn onder meer:

- **Gehashte e-mail**

U kunt de overeenkomende toetsen die in deze gegevensverbinding worden gebruikt, niet bewerken.

![ de werkruimte van de gegevensverbindingen van A met de benadrukt de sleutelensectie van de Gelijke.](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### Planning {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="Plannen"
>abstract="In deze weergave worden de planningsopties weergegeven die u in eerste instantie hebt geselecteerd voor uw gegevensverbinding."

U kunt de planningsopties die u in eerste instantie voor uw gegevensverbinding hebt geselecteerd, niet bewerken. Bekijk voor meer informatie over planningsopties de [sectie](/help/guide/setup/onboard-audiences.md#schedule) Planning in het werkstroomdocument voor het importeren van doelgroepen.

![Een werkruimte voor gegevensverbindingen waarin de sectie Planning is gemarkeerd.](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

## Doelgroepen beheren {#manage-audiences}

Wanneer u de lijst met doelgroepen via uw gegevensverbinding bekijkt, kunt u ervoor kiezen om de doelgroepen weer te geven, hun categorieën te bewerken of ze uit de gegevensverbinding te verwijderen.

![Een werkruimte voor gegevensverbindingen met de doelgroepen gemarkeerd.](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## Volgende stappen

Na het beheren van uw gegevensverbindingen, kunt u [ overlappingen ](/help/guide/collaborate/discover.md) ontdekken tussen uw publiek en het publiek dat uw medewerker ontdekkbaar heeft gemaakt.
