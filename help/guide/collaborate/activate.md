---
title: Soorten publiek activeren
description: Leer hoe je publiek activeert in Adobe Real-Time CDP Collaboration.
audience: admin, publisher
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/nl/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: fd82fcbf-ab39-48e0-9438-0a9046693431
source-git-commit: 691161cdc1f9338a470373988fbc0dee9a5be6db
workflow-type: tm+mt
source-wordcount: '752'
ht-degree: 0%

---

# Soorten publiek activeren

{{limited-availability-release-note}}

>[!IMPORTANT]
>
>De **[!UICONTROL Activate]** werkruimte is slechts beschikbaar als het **2&rbrace; gebruiksgeval van de activering van het publiek [ tijdens het verbindingsproces ](../connect/establishing-connections.md#connection-settings) werd toegelaten.** Voor meer informatie over gebruiksgevallen, verwijs naar [ projecten ](./manage-projects.md#project-use-cases) gids beheren.

Door de activering van het publiek kunt u het publiek activeren in campagnes. De activiteiten zijn een samenwerking tussen adverteerders en uitgevers. Na [ ontdekkend het beste publiek voor uw campagne ](./discover.md), kan het publiek dan het gerichte publiek activeren. Het publiek dat wordt geactiveerd wordt verzonden naar de vooraf geconfigureerde bestemming van de uitgever, zoals Adobe Experience Platform, voor gebruik in campagnes. Voor meer informatie over vestigingsbestemming, verwijs naar de [ gids van het bestemmingsoverzicht ](../destinations/overview.md).

>[!IMPORTANT]
>
>Momenteel, wanneer adverteerders publiek activeren, worden zij dan automatisch geactiveerd aan de bestemming de uitgever die voor hun organisatie wordt gevormd. De uitgever **moet** een bestemming *vormen alvorens* adverteerder een publiek activeert. Als geen bestemming wordt gevormd, zal het publiek naar de uitgever worden verzonden, maar niet in om het even welke campagnes kunnen worden geactiveerd.

## Nieuw publiek activeren

Als u het publiek wilt activeren, navigeert u naar het tabblad **[!UICONTROL Activate]** in de projectwerkruimte.

Selecteer het add pictogram (![ voeg pictogram toe.](/help/assets/icons/plus.png)) of de optie **[!UICONTROL Activate audience]** als er geen vorig publiek is verzonden voor activering.

![ Activate werkruimte in een project zonder toegevoegd publiek.](/help/assets/collaborate/activate/activate-new-audiences.png)

De workflow voor het activeren van soorten publiek wordt geopend. Hier kunt u het publiek selecteren dat u naar uw medewerker wilt verzenden. Gebruik vervolgkeuzelijst om een publiek te selecteren of zoek naar een specifiek publiek. Als u meer informatie over het publiek wilt zien voordat u een selectie maakt, selecteert u **[!UICONTROL Browse audiences]**

![ het de activeringswerkschema van het publiek met dropdown en doorbladert benadrukte publieksopties.](/help/assets/collaborate/activate/audience-activation.png)

In **[!UICONTROL Browse audiences]**, kunt u **[!UICONTROL Identity count]** zien, **[!UICONTROL Overlapping identities]**, en **[!UICONTROL Overlap %]** voor elk publiek.

![ de Browse publieksdialoog die het beschikbare publiek toont.](/help/assets/collaborate/activate/browse-audiences.png)

Selecteer het publiek dat u in campagnes wilt activeren en selecteer vervolgens **[!UICONTROL Save]** . Het publiek wordt nu weergegeven en u ziet de deelvensters **[!UICONTROL Identity count]** , **[!UICONTROL Overlapping identities]** en **[!UICONTROL Overlap %]** voor het geselecteerde publiek.

![ het werkschema van de activering van het Publiek met het geselecteerde getoonde publiek.](/help/assets/collaborate/activate/audience-selected.png)

### Overeenkomstsleutels bewerken

Vervolgens kunt u de overeenkomende toetsen van de doelgroep bewerken door **[!UICONTROL Edit match keys]** te selecteren in het geselecteerde publiek. Deze opties worden overgenomen van de selecties van de match-toets wanneer de verbinding tussen medewerkers voor het eerst werd ingesteld. U kunt geselecteerde wedstrijdtoetsen verwijderen als deze niet van toepassing zijn op een specifieke campagne, maar u kunt geen nieuwe overeenkomende toetsen toevoegen.

![ het werkschema van de activering van het publiek met Edit benadrukte gelijke sleutels.](/help/assets/collaborate/activate/edit-match-keys.png)

Het dialoogvenster **[!UICONTROL Edit match keys]** wordt geopend, waarin u de overeenkomende toetsen die u niet wilt gebruiken, kunt uitschakelen. Selecteer **[!UICONTROL Save]** om uw wijzigingen op te slaan.

>[!NOTE]
>
>Er moet ten minste één overeenkomende toets zijn geselecteerd. In de huidige versie zijn alleen **[!UICONTROL Hashed email]** overeenkomende toetsen beschikbaar. U kunt deze overeenkomende toets dus niet verwijderen.

![ geef gelijke sleuteldialoog in het de activeringswerkschema van het Onderzoek uit.](/help/assets/collaborate/activate/edit-match-keys-selection.png)

### Vernieuwingsfrequentie en interval voor het publiek instellen

Tot slot plaats de gewenste frequentie en de datumwaaier voor het publiek om te verfrissen. In de huidige versie is **[!UICONTROL Once]** de enige ondersteunde frequentieoptie. De **[!UICONTROL Once]** frequentie betekent dat het publiek één keer wordt geactiveerd en niet wordt vernieuwd. De optie **[!UICONTROL Date]** wordt automatisch ingevuld met de huidige datum.

![ het werkschema van de activering van het publiek met de benadrukte sectie van de Frequentie.](/help/assets/collaborate/activate/audience-frequency.png)

Als u tevreden bent met de selecties, selecteert u **[!UICONTROL Activate]** om de workflow te voltooien. Het publiek is nu geactiveerd en u kunt dit weergeven op het tabblad **[!UICONTROL Activate]** . Het zal ook beschikbaar zijn aan uw medewerker op hun **[!UICONTROL Activate]** lusje, waar zij het in campagnes kunnen gebruiken.

U kunt de naam van het publiek uitgeven pictogram (![ pictogram van het Potlood uitgeven.](/help/assets/icons/edit.png) ) of deactiveer het publiek door **[!UICONTROL Deactivate]** te selecteren.

![ activeer lusje met het geactiveerde die publiek en Edit en Deactivate benadrukte opties.](/help/assets/collaborate/activate/edit-activate-audience.png)

## Actieve doelgroepen weergeven

Op het tabblad **[!UICONTROL Activate]** kunnen zowel uitgevers als adverteerders het publiek weergeven dat momenteel is geactiveerd. Momenteel, worden het publiek automatisch verzonden naar de gevormde bestemming van de uitgever nadat adverteerder hen activeert.

![ Overzicht van het Activate lusje, tonend een geactiveerd publiek.](/help/assets/collaborate/activate/activate-overview.png)

Binnen elk geactiveerd publiek, kunt u de volgende metriek zien:

| Metrisch | Beschrijving |
|---------|----------|
| **[!UICONTROL Activated identities]** | Geeft het aantal geactiveerde identiteiten in het publiek aan. |
| **[!UICONTROL Overlapping identities]** | Geeft het aantal overlappende identiteiten tussen dit publiek en de totale populatie profielen in de inventaris van de deelnemer aan. |
| **[!UICONTROL Match key breakdown]** | Toont het identiteitsaantal voor elke identiteit die in het publiek wordt gebruikt. Een totaal aantal gebruikers van 500.000 kan bijvoorbeeld bestaan uit 400.000 gebruikers die de gehashte e-mailidentiteit hebben uitgeschakeld en 100.000 gebruikers die een mobiele-id-identiteit hebben afgevinkt. Let op: in het hier beschreven voorbeeld is dezelfde persoon mogelijk twee keer aanwezig in het publiek met zijn e-mail- en mobiele-id-id-id-identiteit. |

## Volgende stappen {#next-steps}

Na het activeren van gegevens en lopende campagnes, werk met Adobe enablement en ingenieursteam om metingsgegevens te uploaden en de overeenkomstige [ metingsrapporten ](/help/guide/collaborate/measure.md) te bekijken.
