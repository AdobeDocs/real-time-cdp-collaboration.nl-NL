---
title: Soorten publiek activeren
description: Leer hoe je publiek activeert in Adobe Real-Time CDP Collaboration.
audience: admin, publisher
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
source-git-commit: afe8560a12017c6b993f93cde8636288aa6e4991
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 0%

---

# Soorten publiek activeren

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>De **[!UICONTROL Activate]** werkruimte is slechts beschikbaar als het **2&rbrace; gebruiksgeval van de activering van het publiek** tijdens het verbindingsproces [ werd toegelaten. ](../connect/establishing-connections.md#connection-settings) Voor meer informatie over gebruiksgevallen, verwijs naar [ projecten ](./manage-projects.md#project-use-cases) gids beheren.

Met activering van het publiek kunt u het publiek activeren voor gebruik in campagnes. De activering kan door één van beide samenwerker afhankelijk van de montages van de publiekactivering [ worden gedaan die in de verbinding ](/help/guide/connect/establishing-connections.md#configure-connection-settings) worden gevormd. Nadat u [ het beste publiek voor uw campagne ](./discover.md) ontdekt, activeer het publiek om hen voor gebruik beschikbaar te maken. Wanneer u een publiek activeert, wordt het verzonden naar de pre-gevormde bestemming van uw medewerker, zoals Adobe Experience Platform, waar het voor gebruik in campagnes beschikbaar wordt. Voor meer informatie over vestiging bestemmingen, verwijs naar de [ gids van het bestemmingsoverzicht ](../destinations/overview.md).

## Nieuw publiek activeren {#activate-new-audiences}

Als u het publiek wilt activeren, navigeert u naar het tabblad **[!UICONTROL Activate]** in de projectwerkruimte.

>[!IMPORTANT]
>
>**vóór** u een publiek kunt activeren, moet uw samenwerker **&#x200B;**&#x200B;een bestemming vormen. Wanneer u een publiek activeert, wordt het automatisch verzonden naar de gevormde bestemming van uw medewerker. Als er geen bestemming is ingesteld, kunt u het publiek niet activeren.
>
>![ Activate werkruimte wanneer de medewerker geen gevormde bestemming heeft.](/help/assets/collaborate/activate/no-destination-configured.png)

Selecteer het add pictogram (![ voeg pictogram toe.](/help/assets/icons/plus.png)) of de optie **[!UICONTROL Activate audience]** als er geen vorig publiek is verzonden voor activering.

![ Activate werkruimte in een project zonder toegevoegd publiek.](/help/assets/collaborate/activate/activate-new-audiences.png)

De workflow voor het activeren van soorten publiek wordt geopend. Hier kunt u het publiek selecteren dat u naar uw medewerker wilt verzenden. Gebruik vervolgkeuzelijst om een publiek te selecteren of zoek naar een specifiek publiek. Als u meer informatie over het publiek wilt zien voordat u een selectie maakt, selecteert u **[!UICONTROL Browse audiences]**

![ het de activeringswerkschema van het publiek met dropdown en doorbladert benadrukte publieksopties.](/help/assets/collaborate/activate/audience-activation.png)

In **[!UICONTROL Browse audiences]**, kunt u **[!UICONTROL Identity count]** zien, **[!UICONTROL Overlapping identities]**, en **[!UICONTROL Overlap %]** voor elk publiek.

![ de Browse publieksdialoog die het beschikbare publiek toont.](/help/assets/collaborate/activate/browse-audiences.png)

>[!IMPORTANT]
>
>Wanneer het activeren van publiek waar de veelvoudige gelijke sleutels worden gebruikt, als één (of meer) gelijke sleutel geen overlappingen heeft, geen kijkcijfers van het publiek, of onder drempel daalt, zal de volledige activering ontbreken. Zorg ervoor dat uw publiek voldoende overlap heeft en dat het voldoet aan de minimumdrempel van 1000 id&#39;s voor alle overeenkomende toetsen voordat het wordt geactiveerd.

Selecteer het publiek dat u in campagnes wilt activeren en selecteer vervolgens **[!UICONTROL Save]** . Het publiek wordt nu weergegeven en u ziet de deelvensters **[!UICONTROL Identity count]** , **[!UICONTROL Overlapping identities]** en **[!UICONTROL Overlap %]** voor het geselecteerde publiek.

![ het werkschema van de activering van het Publiek met het geselecteerde getoonde publiek.](/help/assets/collaborate/activate/audience-selected.png)

### Overeenkomstsleutels bewerken {#edit-match-keys}

Vervolgens kunt u de overeenkomende toetsen van de doelgroep bewerken door **[!UICONTROL Edit match keys]** te selecteren in het geselecteerde publiek. Deze opties worden overgenomen van de selecties van de match-toets wanneer de verbinding tussen medewerkers voor het eerst werd ingesteld. U kunt geselecteerde wedstrijdtoetsen verwijderen als deze niet van toepassing zijn op een specifieke campagne, maar u kunt geen nieuwe overeenkomende toetsen toevoegen.

![ het werkschema van de activering van het publiek met Edit benadrukte gelijke sleutels.](/help/assets/collaborate/activate/edit-match-keys.png)

Het dialoogvenster **[!UICONTROL Edit match keys]** wordt geopend, waarin u de overeenkomende toetsen die u niet wilt gebruiken, kunt uitschakelen. Selecteer **[!UICONTROL Save]** om uw wijzigingen op te slaan.

>[!NOTE]
>
>Er moet ten minste één overeenkomende toets zijn geselecteerd. In de huidige versie zijn alleen **[!UICONTROL Hashed email]** overeenkomende toetsen beschikbaar. U kunt deze overeenkomende toets dus niet verwijderen.

![ geef gelijke sleuteldialoog in het de activeringswerkschema van het Onderzoek uit.](/help/assets/collaborate/activate/edit-match-keys-selection.png)

### Vernieuwingsfrequentie voor publiek instellen {#set-audience-refresh-frequency}

Tot slot plaats de gewenste frequentie en de datumwaaier voor het publiek om te verfrissen. In de huidige versie is **[!UICONTROL Once]** de enige ondersteunde frequentieoptie. De **[!UICONTROL Once]** frequentie betekent dat het publiek één keer wordt geactiveerd en niet wordt vernieuwd. De optie **[!UICONTROL Date]** wordt automatisch ingevuld met de huidige datum.

![ het werkschema van de activering van het publiek met de benadrukte sectie van de Frequentie.](/help/assets/collaborate/activate/audience-frequency.png)

Als u tevreden bent met de selecties, selecteert u **[!UICONTROL Activate]** om de workflow te voltooien.

## Het dashboard activeren {#activate-dashboard}

Op het tabblad **[!UICONTROL Activate]** kunt u alle soorten publiek weergeven die naar uw medewerker zijn verzonden, evenals alle soorten publiek die uw medewerker naar uw doel heeft geactiveerd.

![ activeer dashboard die het Verzonden publiek en de Geactiveerde publiekssecties tonen.](/help/assets/collaborate/activate/activate-dashboard.png)

## Verzonden publiek weergeven {#view-sent-audiences}

In de **[!UICONTROL Sent audiences to]** collaboratorsectie worden alle soorten publiek weergegeven die u hebt verzonden. Momenteel, worden het publiek automatisch verzonden naar de gevormde bestemming van uw medewerker nadat u hen hebt verzonden. In de mening van uw medewerker, worden deze publiek getoond in de **[!UICONTROL Activated audiences]** sectie.

Binnen elk verzonden publiek, kunt u de volgende metriek zien:

| Metrisch | Beschrijving |
|---------|----------|
| **[!UICONTROL Name]** | De naam van het publiek. |
| **[!UICONTROL Status]** | De status van het verzonden publiek. |
| **[!UICONTROL Identity count]** | Het aantal identiteiten in het publiek. |
| **[!UICONTROL Overlapping identities]** | Het aantal overlappende identiteiten tussen dit publiek en de totale populatie van profielen in de inventaris van de deelnemer. |
| **[!UICONTROL Created]** | De datum waarop het publiek voor het eerst werd verzonden. |
| **[!UICONTROL Last sent]** | De datum waarop het publiek voor het laatst naar uw medewerker is verzonden. |
| **[!UICONTROL Match keys]** | Geeft de overeenkomende toets aan die voor het publiek wordt gebruikt. |

## Actieve doelgroepen weergeven {#view-activated-audiences}

In de sectie **[!UICONTROL Activated audiences]** ziet u alle soorten publiek die op uw doel zijn geactiveerd.

Binnen elk geactiveerd publiek, kunt u de volgende metriek zien:

| Metrisch | Beschrijving |
|---------|----------|
| **[!UICONTROL Name]** | De naam van het publiek. |
| **[!UICONTROL Status]** | De status van het geactiveerde publiek. |
| **[!UICONTROL Identity count]** | Het aantal identiteiten dat werd geactiveerd, op basis van de overlappende identiteiten toen uw medewerker het publiek verstuurde. |
| **[!UICONTROL Created]** | De datum waarop het publiek werd geactiveerd. |
| **[!UICONTROL Last refreshed]** | De datum waarop het publiek voor het laatst is vernieuwd, op basis van het vernieuwingsschema dat tijdens de activering is gekozen. |
| **[!UICONTROL Destination]** | De bestemming waar het publiek werd geactiveerd aan. |
| **[!UICONTROL Match keys]** | Geeft de overeenkomende toets aan die voor het publiek wordt gebruikt. |

## Verzonden publiek verwijderen {#delete-sent-audiences}

U kunt verzonden soorten publiek verwijderen die u niet meer wilt activeren. Wanneer u een verzonden publiek verwijdert, wordt deze verwijderd uit de sectie **[!UICONTROL Sent audiences to]** en wordt de doelgroep niet meer geactiveerd voor de medewerker.

Om een verzonden publiek te schrappen, selecteer het **[!UICONTROL Delete]** pictogram (![ pictogram van de Schrapping.](/help/assets/icons/delete.png) ) naast het publiek in de **[!UICONTROL Sent audiences to]** -sectie.

![ de optie van de Schrapping in het Verzonden publiek aan sectie.](/help/assets/collaborate/activate/delete-sent-audiences.png)

Er wordt een bevestigingsvenster geopend waarin u wordt gevraagd de verwijdering te bevestigen. Selecteer **[!UICONTROL Delete]** om te bevestigen.

![ de bevestigingsdialoog van de Schrapping.](/help/assets/collaborate/activate/delete-sent-audiences-confirmation.png)

## Volgende stappen {#next-steps}

Na het activeren van publiek en lopende campagnes, werk met Adobe enablement en techniekteam om meetgegevens te uploaden en de overeenkomstige [ metingsrapporten ](/help/guide/collaborate/measure.md) te bekijken.
