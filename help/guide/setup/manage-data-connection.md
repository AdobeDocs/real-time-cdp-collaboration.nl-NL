---
title: Gegevensverbindingen beheren
description: Leer hoe u gegevensverbindingen beheert, zoals match keys, planning, use cases en publiekfiltering in Real-Time CDP Collaboration
audience: administrator, data engineer
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/nl/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: d142d3ed-f56a-4150-a885-571728a73ac8
source-git-commit: 46d2596bd0ccdc5da32067493968945c61f8acc4
workflow-type: tm+mt
source-wordcount: '1092'
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

De sleutels van de gelijke zijn de doelgebieden u [&#x200B; in kaart bracht uw brongebieden aan &#x200B;](./onboard-audiences.md#map-fields). Meer over leren hoe de gelijkensleutels werken, zie de [&#x200B; handleiding van de gelijknamensleutels &#x200B;](./onboard-account.md#set-up-match-keys).

![&#x200B; de werkruimte van de gegevensverbindingen van A met de benadrukt de sleutelensectie van de Gelijke.](/help/assets/setup/manage-data-connection/view-data-connection-match-keys.png){zoomable="yes"}

### Planning {#scheduling}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_manage_dataconnections_scheduling"
>title="Planning"
>abstract="Bekijk de planningsdetails voor uw gegevensverbinding, en geef de configuraties indien nodig uit."

Bekijk en beheer de planningsinstellingen voor uw gegevensverbindingen. Het plannen bepaalt hoe vaak het publiek wordt verfrist.

Nadat een gegevensverbinding is gemaakt, kunt u de vernieuwingsfrequentie, de begindatum en de einddatum rechtstreeks bijwerken vanuit de sectie **[!UICONTROL Scheduling]** van de werkruimte voor gegevensverbindingen.

>[!NOTE]
>
>Bij het aanschaffen van soorten publiek bij Adobe Experience Platform wordt het publiek binnen 24 uur na de totstandbrenging van de gegevensverbinding beschikbaar gesteld. Na de eerste bron worden de publieksgegevens vernieuwd volgens de gedefinieerde frequentie.

Voor meer informatie bij het plannen, zie [&#x200B; het plannen sectie &#x200B;](/help/guide/setup/onboard-audiences.md#schedule) in de gids aan het vormen publiek.

![&#x200B; de werkruimte van de gegevensverbinding van A met de het Plannen benadrukte sectie.](/help/assets/setup/manage-data-connection/view-data-connection-scheduling.png){zoomable="yes"}

## Gegevensverbinding bewerken {#edit-data-connection}

Lees de volgende secties om te leren hoe te om de gelijke sleutels en het plannen montages van een bestaande gegevensverbinding bij te werken.

### Overeenkomstsleutels bewerken {#edit-match-keys}

>[!IMPORTANT]
>
>Let op het volgende voordat u de overeenkomende toetsen voor een gegevensverbinding bewerkt:
>
>* Alleen overeenkomende sleutels die zijn geconfigureerd voor uw account kunnen worden gebruikt voor gegevensverbindingen.
>* Op dit moment kunt u aanvullende overeenkomende toetsen toevoegen aan een gegevensverbinding, maar als een overeenkomende toets eenmaal is ingeschakeld, kan deze niet worden verwijderd.

Selecteer **[!UICONTROL Edit]** in de sectie **[!UICONTROL Match keys]** .

![&#x200B; de de sleutelensectie van de Gelijke met Edit benadrukte optie.](/help/assets/setup/manage-data-connection/edit-match-keys.png){zoomable="yes"}

Er wordt een bevestigingsdialoogvenster weergegeven waarin wordt uitgelegd dat wijzigingen in de gegevensverbinding van toepassing zijn op alle bijbehorende doelgroepen. Selecteer **[!UICONTROL OK]** om te bevestigen. Je kunt deze bevestiging later overslaan.

![&#x200B; dialoog die van de Bevestiging toont dat om het even welke veranderingen in de gegevensverbinding op alle bijbehorende publiek van toepassing zullen zijn.](/help/assets/setup/manage-data-connection/confirm-data-connection-changes.png){zoomable="yes"}

In het dialoogvenster **[!UICONTROL Match keys]** kunt u de bestaande toewijzingen tussen bronvelden en de bijbehorende doelvelden (overeenkomende toetsen) weergeven. U kunt een gelijke sleutel uitgeven door het in kaart gebrachte brongebied bij te werken, of extra rijen van het toewijzingsgebied toe te voegen om nieuwe gelijke sleutels te bevolken.

![&#x200B; de de sleuteldialoog van de Gelijke die de bestaande afbeeldingen tussen brongebieden en de overeenkomstige doelgebieden tonen.](/help/assets/setup/manage-data-connection/match-keys-dialog.png){zoomable="yes"}

#### Overeenkomstsleutels toevoegen {#add-match-keys}

Selecteer **[!UICONTROL Add field]** om een nieuwe veldrij toe te voegen.

![&#x200B; na het selecteren van voegt gebied toe, toont de de sleuteldialoog van de Gelijke een leeg nieuw toewijzingsgebied klaar voor input.](/help/assets/setup/manage-data-connection/add-new-field.png){zoomable="yes"}

Selecteer vervolgens het lege bronveld. Het dialoogvenster **[!UICONTROL Select source field]** wordt weergegeven met de opties **[!UICONTROL Identity namespaces]** en **[!UICONTROL Profile attributes]** . U kunt de lijst filteren en het gewenste bronveld zoeken met de zoekoptie.

Kies het gewenste bronveld, gevolgd door **[!UICONTROL Select]** .

![&#x200B; de Uitgezochte geselecteerde dialoog van het brongebied met de geselecteerde optie GAID.](/help/assets/setup/manage-data-connection/select-source-field.png){zoomable="yes"}

In het dialoogvenster **[!UICONTROL Match keys]** gebruikt u het vervolgkeuzemenu om het nieuwe bronveld toe te wijzen aan een doelveld. Alle beschikbare doelgebieden zijn de gelijke sleutels die voor uw rekening van de Medewerker worden gevormd. Als u niet het doelgebied ziet u nodig hebt, [&#x200B; geeft de de overeenkomstensleutels van uw rekening uit &#x200B;](./onboard-account.md#edit-match-keys) om het toe te voegen.

Gebruik de optie **[!UICONTROL Apply transformation]** als u een niet-gehasht veld wilt betrekken bij een gehasht doelveld, bijvoorbeeld wanneer u een bronveld voor normale tekst toewijst aan het doelveld van **[!UICONTROL Hashed email]** .

![&#x200B; dropdown menu dat alle beschikbare doelgebieden toont om met het nieuwe brongebied in kaart te brengen.](/help/assets/setup/manage-data-connection/select-target-field.png){zoomable="yes"}

Nadat u de toewijzingsvelden hebt gemaakt, controleert u de updates en selecteert u **[!UICONTROL Confirm]** om de wijzigingen toe te passen.

![&#x200B; de dialoog van de sleutels van de Gelijke die de bijgewerkte gebiedstoewijzing met de bevestig benadrukte optie toont.](/help/assets/setup/manage-data-connection/review-and-confirm.png){zoomable="yes"}

Een bevestigingsvenster bevestigt dat de overeenkomende toetsen zijn bijgewerkt.

### Planning bewerken {#edit-scheduling}

Nadat een gegevensverbinding is gemaakt, kunt u de vernieuwingsfrequentie, de begindatum en de einddatum rechtstreeks bijwerken vanuit de sectie **[!UICONTROL Scheduling]** van de werkruimte voor gegevensverbindingen.

U kunt de frequentie van een bestaande gegevensverbinding bewerken om beter te bepalen hoe vaak het publiek wordt vernieuwd. Als u het schema wilt bewerken, selecteert u **[!UICONTROL Edit]** in de gegevensverbinding in de planningkaart.

![&#x200B; de Plannende sectie met de Edit benadrukte optie.](/help/assets/setup/manage-data-connection/edit-scheduling.png){zoomable="yes"}

Er wordt een bevestigingsdialoogvenster weergegeven waarin wordt uitgelegd dat wijzigingen in de gegevensverbinding van toepassing zijn op alle bijbehorende doelgroepen. Selecteer **[!UICONTROL OK]** om te bevestigen. Je kunt deze bevestiging later overslaan.

![&#x200B; dialoog die van de Bevestiging toont dat om het even welke veranderingen in de gegevensverbinding op alle bijbehorende publiek van toepassing zullen zijn.](/help/assets/setup/manage-data-connection/confirm-data-connection-changes.png){zoomable="yes"}

Selecteer in het dialoogvenster **[!UICONTROL Scheduling]** het vervolgkeuzemenu waarin u het dialoogvenster **[!UICONTROL Frequency]** wilt bijwerken. Stel de vernieuwingsfrequentie in voor dagelijks gebruik of elke twee tot zes dagen.

![&#x200B; het Plannen dialoog met dropdown van de Frequentie die wordt uitgebreid om publiek te tonen verfrist frequentieopties.](../../assets/setup/manage-data-connection/edit-frequency.png){zoomable="yes"}

Selecteer vervolgens **[!UICONTROL Date range]** als u de periode wilt bijwerken waarin het publiek wordt gevuld en vernieuwd.

![&#x200B; de Plannende dialoog die het de waaiervervolgkeuzemenu toont van de Datum uitgevouwen om het begin en einddatum voor publiekspopulatie uit te geven en te verfrissen.](../../assets/setup/manage-data-connection/edit-date-range.png){zoomable="yes"}

Als u klaar bent, controleert u de updates en selecteert u **[!UICONTROL Save]** om de wijzigingen toe te passen.

![&#x200B; de Plannende dialoog die de updates en sparen optie benadrukt.](../../assets/setup/manage-data-connection/scheduling-dialog.png){zoomable="yes"}

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
