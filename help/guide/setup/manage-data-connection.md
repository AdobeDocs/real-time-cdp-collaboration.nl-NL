---
title: Gegevensverbindingen beheren
description: Leer hoe u gegevensverbindingen beheert, zoals match keys, planning, use cases en publiekfiltering in Real-Time CDP Collaboration
audience: administrator, data engineer
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/nl/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: c76259c1a5a684e69e4b5ac8bfdecc9026fe0939
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 0%

---

# Gegevensverbindingen beheren

{{limited-availability-release-note}}

## Overzicht

Gebruik gegevensverbindingen in Real-Time CDP Collaboration om het publiek van verschillende platforms te voorzien. Leer hoe u de sleutels van uw overeenkomst beheert en hoe u het vernieuwen van de gegevens voor uw bestaande gegevensverbindingen plant. Bovendien, zult u publiek door verschillende attributen voor meer korrelige inzichten kunnen filtreren.

## Gegevensverbindingen weergeven

Als u bestaande gegevensverbindingen wilt weergeven, navigeert u naar **[!UICONTROL Setup]** en selecteert u de tab **[!UICONTROL My data connections]** . Al uw huidige gegevensverbinding wordt getoond, tonend een kort overzicht voor elke verbinding. Selecteer **[!UICONTROL View data connection]** voor een volledige weergave van de gegevens van een gegevensverbinding, inclusief de overeenkomende sleutels, planningsdetails en doelgroepen.

![&#x200B; de werkruimte van de Opstelling met Mijn getoonde en benadrukte mening van het lusje van gegevensverbindingen.](/help/assets/setup/manage-data-connection/my-data-connections.png){zoomable="yes"}

### Toetsen afstemmen {#match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_matchkeys"
>title="Toetsen afstemmen"
>abstract="Met Identieke toetsen bepaalt u hoe gegevens uit verschillende bronnen worden vergeleken. De hieronder getoonde sleutels van de gelijke zijn de doelgebieden u uw brongebieden aan in kaart bracht."

De sleutels van de gelijke zijn de doelgebieden u [&#x200B; in kaart bracht uw brongebieden aan &#x200B;](./onboard-audiences.md#map-fields). U kunt de sleutels niet uitgeven die u aanvankelijk voor uw gegevensverbinding selecteerde. Als u overeenkomende toetsen wilt bijwerken, moet u een nieuwe gegevensverbinding maken. Meer over leren hoe de gelijkensleutels werken, zie de [&#x200B; handleiding van de gelijknamensleutels &#x200B;](./onboard-account.md#set-up-match-keys).

![&#x200B; de werkruimte van de gegevensverbindingen van A met de benadrukt de sleutelensectie van de Gelijke.](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### Planning {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="Planning"
>abstract="Bekijk de planningsdetails voor uw gegevensverbinding, en geef indien nodig uit vernieuwt frequentie."

Bekijk en beheer de planningsinstellingen voor uw gegevensverbindingen. Het plannen bepaalt hoe vaak het publiek wordt verfrist.

Nadat een gegevensverbinding is gemaakt, kunt u de vernieuwingsfrequentie rechtstreeks vanuit de sectie **[!UICONTROL Scheduling]** van de werkruimte voor gegevensverbindingen bijwerken.

>[!NOTE]
>
>Bij het aanschaffen van soorten publiek bij Adobe Experience Platform wordt het publiek binnen 24 uur na de totstandbrenging van de gegevensverbinding beschikbaar gesteld. Na de eerste bron worden de publieksgegevens vernieuwd volgens de gedefinieerde frequentie.

Voor meer informatie bij het plannen, zie [&#x200B; het plannen sectie &#x200B;](/help/guide/setup/onboard-audiences.md#schedule) in de gids aan het vormen publiek.

![&#x200B; de werkruimte van de gegevensverbinding van A met de het Plannen benadrukte sectie.](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

#### Planning bewerken {#edit-scheduling}

U kunt de frequentie van een bestaande gegevensverbinding bewerken om beter te bepalen hoe vaak het publiek wordt vernieuwd. Als u het schema wilt bewerken, selecteert u **[!UICONTROL Edit]** in de gegevensverbinding in de planningkaart.

De planning is van invloed op alle soorten publiek die afkomstig zijn van de gegevensverbinding.

Selecteer in het dialoogvenster **[!UICONTROL Scheduling]** het vervolgkeuzemenu waarin u het dialoogvenster **[!UICONTROL Frequency]** wilt bijwerken. Stel de vernieuwingsfrequentie in voor dagelijks gebruik of elke twee tot zes dagen. Als u klaar bent, selecteert u **[!UICONTROL Save]** om de wijzigingen toe te passen.

![&#x200B; de Plannende dialoog, die opties tonen om frequentie en datumwaaier te plaatsen.](../../assets/setup/manage-data-connection/scheduling-dialog.png){zoomable="yes"}

## Gegevensverbinding verwijderen

Als u een gegevensverbinding verwijdert, worden alle onderliggende doelgroepen, bijbehorende instellingen en het gebruik in Collaboration verwijderd. Deze handeling kan niet ongedaan worden gemaakt.

Om een bestaande gegevensverbinding te schrappen, selecteer het schrappingspictogram (![&#x200B; pictogram van de Schrapping &#x200B;](/help/assets/common/delete.svg)) binnen de werkruimte van een individuele gegevensverbinding.

![&#x200B; de werkruimte van de gegevensverbindingen van A met de benadrukte schrappingsoptie.](/help/assets/setup/manage-data-connection/delete-data-connection.png){zoomable="yes"}

Er wordt een bevestigingsvenster weergegeven. Selecteer **[!UICONTROL Delete]** om het verwijderen van de gegevensverbinding te voltooien.

![&#x200B; de dialoog van de de gegevensverbinding van de Schrapping met de benadrukte optie van de Schrapping.](/help/assets/setup/manage-data-connection/delete-data-connection-confirm.png){zoomable="yes"}

## Soorten publiek beheren {#manage-audiences}

Onder aan de werkruimte wordt een lijst met publiek weergegeven dat is gekoppeld aan de gegevensverbinding. In de lijst wordt een kort overzicht van elk publiek weergegeven, inclusief de status, de bron en de toegang tot de verbinding. Selecteer de naam van een publiek als u de categorieën, de verbindingstoegang of de zichtbaarheid van metagegevens van een publiek wilt bewerken. Voor een volledige gids bij het beheren van een publiek, verwijs naar de [&#x200B; mening individuele gids van het publiek &#x200B;](./onboard-audiences.md#view-individual-audiences).

![&#x200B; de werkruimte van de gegevensverbindingen van A met de benadrukte publiek.](/help/assets/setup/manage-data-connection/view-data-connection-manage-audiences.png){zoomable="yes"}

## Volgende stappen

Na het beheren van uw gegevensverbindingen, kunt u [&#x200B; overlappingen &#x200B;](/help/guide/collaborate/discover.md) ontdekken tussen uw publiek en het publiek dat uw medewerker ontdekkbaar heeft gemaakt.
