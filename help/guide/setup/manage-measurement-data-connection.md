---
title: Gegevensverbindingen voor metingen beheren
description: Leer hoe u gegevensverbindingen voor metingen beheert, inclusief details en sleutels in Real-Time CDP Collaboration
audience: administrator, data engineer
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/nl/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 494277f421606eda62b74c254f1fdd29b22e3473
workflow-type: tm+mt
source-wordcount: '1270'
ht-degree: 0%

---

# Gegevensverbindingen voor metingen beheren

{{limited-availability-release-note}}

## Overzicht

Gebruik verbindingen met meetgegevens in Real-Time CDP Collaboration om uw conversiegegevens van verschillende platforms te verkrijgen. Leer hoe u details kunt beheren en sleutels kunt afstemmen voor uw bestaande gegevensverbindingen.

## Gegevensverbindingen voor metingen weergeven {#view-measurement-data-connections}

U kunt details voor om het even welke bestaande verbinding van metingsgegevens bekijken, met inbegrip van hoe uw omzettingsgegevens worden gedownload, die sleutels in gebruik zijn, en alle omzettingsgebeurtenissen verbonden aan de verbinding.

Navigeer vanuit de werkruimte **[!UICONTROL Setup]** naar het tabblad **[!UICONTROL My data connections]** . Alle huidige verbindingen met meetgegevens worden onder de sectie **[!UICONTROL Measurement]** weergegeven in een tabel- of rasterweergave. Selecteer **[!UICONTROL View data connection]** op de relevante verbindingskaart, of selecteer de naam van de gegevensverbinding wanneer in lijstmening om zijn werkruimte te openen en alle details te bekijken.

![&#x200B; het Mijn lusje van gegevensverbindingen die een kaart van de meetgegevensverbinding en de optie van de de gegevensverbinding van de Mening benadrukken.](/help/assets/setup/manage-measurement-data-connection/view-measurement-data-connection.png){zoomable="yes"}

### Verbindingsgegevens meetgegevens {#measurement-data-connection-details}

In deze sectie kunt u de volgende details van de gegevensverbinding zien:

| Veld | Beschrijving |
|-------------------|-------------|
| Status | De huidige status van de gegevensverbinding voor metingen, bijvoorbeeld **[!UICONTROL Active]** . |
| Source | Het platform of systeem dat de meetgegevens voor deze verbinding levert. |
| Sandbox | De naam van de sandbox waarin de gegevensverbinding voor metingen is geconfigureerd. |
| Gegevensset | De naam van de gegevensset die wordt gebruikt voor het ophalen van meetgegevens in de verbinding. |
| Laatst bijgewerkt | Het tijdstempel van de meest recente update van de gegevensverbinding voor metingen. |
| Laatst bijgewerkt op | De gebruiker die de gegevensverbinding voor de meting als laatste heeft gewijzigd. |
| Gemaakt | De tijdstempel op het moment dat de gegevensverbinding voor de meting is gemaakt. |
| Gemaakt door | De gebruiker die oorspronkelijk de gegevensverbinding voor de meting heeft gemaakt. |

{style="table-layout:auto"}

### Toetsen afstemmen {#match-keys}

De sleutels van de gelijke zijn de doelgebieden u uw brongebieden aan in kaart bracht wanneer u [&#x200B; uw metingsgegevens &#x200B;](./onboard-measurement-data.md) bron. Meer over leren hoe de gelijkensleutels werken, zie de [&#x200B; handleiding van de gelijknamensleutels &#x200B;](./onboard-account.md#set-up-match-keys).

![&#x200B; de verbindingswerkruimte van de metingsgegevens van A met de benadrukt de sleutelensectie van de Gelijke.](/help/assets/setup/manage-measurement-data-connection/view-match-keys.png){zoomable="yes"}

### Conversiegebeurtenissen {#conversion-events}

Onder aan de werkruimte wordt een lijst weergegeven met conversiegebeurtenissen die zijn gekoppeld aan de gegevensverbinding. De lijst bevat een kort overzicht van elke gebeurtenis, inclusief de status, het conversietype en de bron. U kunt de gebeurtenisnaam selecteren om zijn configuraties te bekijken en uit te geven, of de omzettingsgebeurtenis met de schrappingsoptie te verwijderen (![&#x200B; pictogram van de Schrapping &#x200B;](/help/assets/common/delete.svg)). Voor een volledige gids bij het beheren van een omzettingsgebeurtenis, verwijs naar [&#x200B; en beheer meetgegevens &#x200B;](./onboard-measurement-data.md) gids.

![&#x200B; de verbindingswerkruimte van de metingsgegevens van A met de benadrukte sectie van omzettingsgebeurtenissen.](/help/assets/setup/manage-measurement-data-connection/view-conversion-events.png){zoomable="yes"}

## Verbinding met meetgegevens bewerken {#edit-measurement-data-connection}

U kunt op elk gewenst moment de details bijwerken en de sleutels van een bestaande verbinding met meetgegevens afstemmen om ervoor te zorgen dat de rapportage en analyse correct blijven. Navigeer eerst naar het tabblad **[!UICONTROL My data connections]** en selecteer de gegevensverbinding voor metingen die u wilt bewerken. Hiermee opent u de werkruimte voor gegevensverbinding, waarin u de onderstaande stappen kunt volgen om de benodigde wijzigingen aan te brengen.

### Naam en beschrijving bewerken {#edit-name-and-description}

Om de naam en de beschrijving van de gegevensverbinding bij te werken, uitgezocht geef pictogram uit (![&#x200B; geef pictogram &#x200B;](/help/assets/icons/edit.png)) naast de huidige verbindingsnaam uit.

![&#x200B; de werkruimte van de de verbinding van metingsgegevens die het Edit pictogram naast de naam van de gegevensverbinding benadrukken.](/help/assets/setup/manage-measurement-data-connection/edit-name-description.png){zoomable="yes"}

Werk in het dialoogvenster **[!UICONTROL Edit data connection]** de velden bij met de gewenste waarden en selecteer vervolgens **[!UICONTROL Save]** om de wijzigingen toe te passen.

![&#x200B; de Edit dialoog van de gegevensverbinding met sparen benadrukte optie.](/help/assets/setup/manage-measurement-data-connection/edit-name-description-dialog.png){zoomable="yes"}

Er verschijnt een bevestigingsvenster om te bevestigen dat de gegevens zijn bijgewerkt.

### Overeenkomstsleutels bewerken {#edit-match-keys}

>[!IMPORTANT]
>
>Let op het volgende voordat u de overeenkomende toetsen voor een gegevensverbinding bewerkt:
>
>* Alleen overeenkomende sleutels die zijn geconfigureerd voor uw account kunnen worden gebruikt voor gegevensverbindingen.
>* Op dit moment kunt u aanvullende overeenkomende toetsen toevoegen aan een gegevensverbinding, maar als een overeenkomende toets eenmaal is ingeschakeld, kan deze niet worden verwijderd.

Selecteer **[!UICONTROL Edit]** in het deelvenster **[!UICONTROL Match keys]** van de werkruimte voor gegevensverbinding.

![&#x200B; de de sleutelensectie van de Gelijke met Edit benadrukte optie.](/help/assets/setup/manage-measurement-data-connection/edit-match-keys.png){zoomable="yes"}

Er wordt een bevestigingsvenster weergegeven waarin wordt uitgelegd dat wijzigingen in de gegevensverbinding van toepassing zijn op alle bijbehorende conversies. Selecteer **[!UICONTROL OK]** om te bevestigen. Je kunt deze bevestiging later overslaan.

![&#x200B; dialoog die van de Bevestiging toont dat om het even welke veranderingen in de gegevensverbinding op alle bijbehorende omzettingen van toepassing zullen zijn.](/help/assets/setup/manage-measurement-data-connection/confirm-data-connection-changes.png){zoomable="yes"}

In het dialoogvenster **[!UICONTROL Match keys]** kunt u verrijkingsinstellingen bekijken en de huidige toewijzingen tussen uw bronvelden en de doelvelden (overeenkomende toetsen) bekijken.

![&#x200B; de de sleuteldialoog van de Gelijke die de verrijkingsmontages en bestaande afbeeldingen tussen brongebieden en de overeenkomstige doelgebieden tonen.](/help/assets/setup/manage-measurement-data-connection/edit-match-keys-dialog.png){zoomable="yes"}

#### Verrijking {#enrichment}

Als de verrijking niet werd toegelaten toen u [&#x200B; uw metingsgegevens &#x200B;](./onboard-measurement-data.md) kocht, hebt u de optie om uw gebeurtenisdataset met attributen van het Profiel van de Klant in real time te verrijken. Wanneer verrijking is ingeschakeld voor meetgegevens, kan deze niet worden uitgeschakeld. U kunt de toetsen voor verrijkingssamenvoeging desgewenst nog steeds bijwerken.

Wanneer u verrijking inschakelt in het dialoogvenster **[!UICONTROL Match keys]** , wordt de interface uitgebreid om meer configuratieopties weer te geven onder de sectie **[!UICONTROL Enrich your event data with IDs from profiles]** .

Selecteer de optie **[!UICONTROL Source field join key]** .

![&#x200B; de de sleuteldialoog van de Gelijke met het gebied van Source sluit zich bij zeer belangrijke benadrukte optie aan.](../../assets/setup/manage-measurement-data-connection/enrich-event-data.png){zoomable="yes"}

Kies in het dialoogvenster **[!UICONTROL Source field join key]** het bronveld, gevolgd door **[!UICONTROL Select]** .

![&#x200B; het gebied van Source sluit zich aan bij zeer belangrijke dialoog die het geselecteerde brongebied en de Volgende optie benadrukt.](../../assets/setup/manage-measurement-data-connection/source-field-join-key-dialog.png){zoomable="yes"}

Selecteer vervolgens de optie **[!UICONTROL Profile join key]** . Selecteer in het dialoogvenster **[!UICONTROL Profile join key]** het profielveld in de lijst. U kunt de optie Zoeken gebruiken om het gewenste veld te zoeken. Kies vervolgens **[!UICONTROL Select]** om te bevestigen.

![&#x200B; het Profiel sluit zich bij zeer belangrijk dialoog die het geselecteerde profielgebied en de Uitgezochte optie benadrukt.](../../assets/setup/manage-measurement-data-connection/profile-join-key-dialog.png){zoomable="yes"}

#### Toewijzing bewerken {#edit-mapping}

Als u een bestaande overeenkomende sleutel wilt bewerken, werkt u het bijbehorende bronveld en doelveld bij in het dialoogvenster **[!UICONTROL Match keys]** . Selecteer **[!UICONTROL Add field]** als u een nieuwe overeenkomende sleutel wilt opnemen. Zo ontstaat een lege rij waarin u aanvullende toewijzingen kunt definiëren tussen bron- en doelvelden.

![&#x200B; na het selecteren van voegt gebied toe, toont de de sleuteldialoog van de Gelijke een lege nieuwe toewijzingsrij klaar voor input.](/help/assets/setup/manage-measurement-data-connection/add-new-field.png){zoomable="yes"}

Selecteer vervolgens het lege bronveld. Het dialoogvenster **[!UICONTROL Select source field]** wordt weergegeven met een lijst beschikbare bronvelden die zijn gegroepeerd onder opties zoals **[!UICONTROL Identity namespaces]** en **[!UICONTROL Profile attributes]** . U kunt de lijst filteren en het gewenste bronveld zoeken met de zoekoptie.

Kies het gewenste bronveld, gevolgd door **[!UICONTROL Select]** .

![&#x200B; de Uitgezochte dialoog van het brongebied die de optie van het Onderzoek, het Van de bron Telefoon gebied, en de Uitgezochte optie benadrukt.](/help/assets/setup/manage-measurement-data-connection/select-source-field.png){zoomable="yes"}

In het dialoogvenster **[!UICONTROL Match keys]** gebruikt u het vervolgkeuzemenu om het nieuwe bronveld toe te wijzen aan een doelveld. Alle beschikbare doelgebieden zijn de gelijke sleutels die voor uw rekening van de Medewerker worden gevormd. Als u niet het doelgebied ziet u nodig hebt, [&#x200B; geeft de de overeenkomstensleutels van uw rekening uit &#x200B;](./onboard-account.md#edit-match-keys) om het toe te voegen.

Gebruik de optie **[!UICONTROL Apply transformation]** als u een niet-gehasht veld wilt betrekken bij een gehasht doelveld, bijvoorbeeld wanneer u een bronveld voor een onbewerkte tekst toewijst aan het doelveld van **[!UICONTROL Hashed phone]** .

![&#x200B; dropdown menu dat alle beschikbare doelgebieden toont om met het nieuwe brongebied in kaart te brengen.](/help/assets/setup/manage-measurement-data-connection/target-field-dropdown.png){zoomable="yes"}

Nadat u de toewijzingsvelden hebt gemaakt, controleert u de updates en selecteert u **[!UICONTROL Confirm]** om de wijzigingen toe te passen.

![&#x200B; de dialoog van de sleutels van de Gelijke die de bijgewerkte gebiedstoewijzing met de bevestig benadrukte optie toont.](/help/assets/setup/manage-measurement-data-connection/confirm-edit-match-keys.png){zoomable="yes"}

Een bevestigingsvenster bevestigt dat de overeenkomende toetsen zijn bijgewerkt.

## Gegevensverbinding verwijderen

Als u een gegevensverbinding verwijdert, worden alle onderliggende conversies, bijbehorende instellingen en het gebruik in Collaboration verwijderd. Deze handeling kan niet ongedaan worden gemaakt.

Om een bestaande gegevensverbinding te schrappen, selecteer het schrappingspictogram (![&#x200B; pictogram van de Schrapping &#x200B;](/help/assets/common/delete.svg)) binnen de werkruimte van een individuele gegevensverbinding.

![&#x200B; de werkruimte van de gegevensverbindingen van A met de benadrukte schrappingsoptie.](/help/assets/setup/manage-measurement-data-connection/delete-measurement-data-connection.png){zoomable="yes"}

Er wordt een bevestigingsvenster weergegeven. Selecteer **[!UICONTROL Delete]** om het verwijderen van de gegevensverbinding te voltooien.

![&#x200B; de dialoog van de de gegevensverbinding van de Schrapping met de benadrukte optie van de Schrapping.](/help/assets/setup/manage-measurement-data-connection/delete-measurement-data-connection-confirm.png){zoomable="yes"}

Een bevestigingsvenster bevestigt dat de gegevensverbinding is verwijderd.

## Volgende stappen {#next-steps}

Nadat u de verbindingen met meetgegevens hebt beheerd, kunt u:

* Voeg desgewenst meer conversiegebeurtenissen toe die zijn gekoppeld aan uw gegevensverbinding. Voor gedetailleerde stappen, lees [&#x200B; toevoegt en beheert metingsgegevens &#x200B;](./onboard-measurement-data.md) documentatie.
* Genereer maatrapporten om inzicht te krijgen in de prestaties en impact van uw campagne. Voor meer informatie over beschikbare rapporttypes en hoe te om hen tot stand te brengen, zie de [&#x200B; gids van de meetprestaties &#x200B;](/help/guide/collaborate/measure.md).
