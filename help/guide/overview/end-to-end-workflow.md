---
title: Volledige workflow
description: Begrijp de end-to-end workflow van het gebruiken van Real-Time CDP Collaboration op basis van uw samenwerkingspatroon.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/nl/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 90f9341e-5dd7-4521-a602-edb0263838c5
source-git-commit: 8745d6d8da389b552af3da6612bf693230dfb538
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 0%

---

# Volledige workflow

{{limited-availability-release-note}}

In Adobe Real-Time CDP Collaboration varieert de end-to-end workflow op basis van het samenwerkingspatroon dat u kiest. In de workflow worden de stappen beschreven die nodig zijn voor het opzetten en uitvoeren van een samenwerkingsproject, van het maken van accounts en het aantrekken van publiek tot het maken van verbindingen en het maken van projecten. Kennis van deze workflow is essentieel voor het effectief benutten van de mogelijkheden van het platform om uw marketingdoelstellingen te bereiken.

## Aan de slag

Voordat u begint, moet u ervoor zorgen dat u een goed inzicht hebt in deze belangrijke concepten:

- **patronen van Collaboration**: Deze patronen bepalen hoe de medewerkers samenwerken. Er zijn twee verschillende patronen: [ adverteerder-aan-uitgever ](./collaboration-patterns.md#advertiser-to-publisher) en [ merk-aan-merk ](./collaboration-patterns.md#brand-to-brand).
- **de rollen van de Rekening**: De rollen van de rekening bepalen uw mogelijkheden binnen het platform. Zij zouden aan de doelstellingen van uw organisatie, merk, en doelstellingen moeten richten. Er zijn twee rekeningsrollen: [ adverteerder ](./roles.md#advertiser) en [ uitgever ](./roles.md#publisher).
- **gevallen van het Gebruik**: De gevallen van het gebruik bepalen de manieren u hefboomwerking Collaboration kunt om uw marketing doelstellingen te bereiken. Er zijn drie gevallen van het samenwerkingsgebruik: [ ontdekt ](./use-cases.md#discover), [ activeert ](./use-cases.md#activate), en [ Maatregel ](./use-cases.md#measure).

Deze gids zal drie mock medewerkers gebruiken om het werkschema van begin tot eind te illustreren:

- **[!UICONTROL Luma]**: Een merk voor atletische kleding. Zij zijn een adverteerder die een specifiek publiek wil bereiken via gerichte marketingcampagnes.
- **[!UICONTROL TV Tube]** : een provider van digitale streaming. Zij zijn een uitgever die publieksgegevens voor gebruik door adverteerders verstrekt.
- **[!UICONTROL Fit Apparel]**: Een ander merk voor atletische kleding. Het zijn een tweede adverteerder die wil samenwerken om publieksgegevens en inzichten voor verhoogde marketing inspanningen te delen.

## Workflow voor adverteerders naar uitgevers {#advertiser-to-publisher-workflow}

[!UICONTROL Luma] , een atletisch detailhandelsbedrijf, wil een verbinding maken met [!UICONTROL TV Tube] , een aanbieder van digitale streaming, om een specifiek publiek te bereiken via gerichte marketingcampagnes.

Om te beginnen, [!UICONTROL Luma] moet [ een rekening ](../setup/onboard-account.md) met de adverteerderrol creëren, terwijl [!UICONTROL TV Tube] tot een rekening met de uitgeversrol leidt.

Na het vestigen van hun rekeningen, zowel [!UICONTROL Luma] als [!UICONTROL TV Tube] moeten [ een gegevensverbinding en bronpubliek ](../setup/onboard-audiences.md) tot stand brengen. Slechts [!UICONTROL TV Tube] zal publiek voor marketing campagnes activeren, zodat moeten zij [ een bestemming ](../setup/manage-destinations.md) vormen.

Zodra beide medewerkers hun rekeningsopstelling hebben, zijn zij klaar om [ van een verbinding ](../connect/establishing-connections.md) binnen het platform te vormen. [!UICONTROL Luma] gebruikt [ ontdekt uitgevers ](../connect/discover-publishers.md) eigenschap om [!UICONTROL TV Tube] te vinden en een verbindingsverzoek in werking te stellen. Nadat [!UICONTROL TV Tube] de verbindingsaanvraag heeft geaccepteerd, configureert [!UICONTROL Luma] de verbindingsinstellingen om te bepalen hoe de samenwerking verloopt. [!UICONTROL TV Tube] accepteert het verbindingsverzoek om een veilige koppeling tussen de twee merken tot stand te brengen.

Nadat de verbinding wordt gevestigd, [!UICONTROL Luma] [ leidt tot een project ](../collaborate/manage-projects.md) om van hun samenwerking met [!UICONTROL TV Tube] af te schoppen. Tijdens de projectopstelling, kiezen zij de gevallen van het samenwerkingsgebruik die hun doelstellingen het best passen: [ ontdekt ](../collaborate/discover.md), [ activeert ](../collaborate/activate.md), en [ Maatregel ](../collaborate/measure.md).

[!UICONTROL Luma] hefboomwerkingen [ ontdekken ](../collaborate/discover.md) gebruiksgeval om inzichten in [!UICONTROL TV Tube] het publieksgegevens van de publiek te bereiken. Zodra [!UICONTROL Luma] de segmenten van het doelpubliek heeft geïdentificeerd, activeren zij [&#128279;](../collaborate/activate.md) deze publiek.

Na het activeren van het publiek, [!UICONTROL TV Tube] looppas gerichte marketing campagnes en uploadt gegevens aan [ Meetlat ](../collaborate/measure.md) de resultaten om de doeltreffendheid van hun campagne te evalueren.

## Brand-to-brand workflow {#brand-to-brand-workflow}

[!UICONTROL Fit Apparel] , een atletisch merkmerk, wil samenwerken met [!UICONTROL Luma] , een ander atletisch merkmerk, om publieksgegevens en inzichten voor verhoogde marketing te delen.

Na het vestigen van hun rekeningen, zowel [!UICONTROL Fit Apparel] als [!UICONTROL Luma] moeten [ een gegevensverbinding en bronpubliek ](../setup/onboard-audiences.md) tot stand brengen. Zowel [!UICONTROL Fit Apparel] als [!UICONTROL Luma] zullen publiek voor marketing campagnes activeren, zodat moeten zij allebei een bestemming [ vormen.](../setup/manage-destinations.md)

Na het betrekken van hun publiek, [!UICONTROL Fit Apparel] en [!UICONTROL Luma] [ vorm een verbinding ](../connect/establishing-connections.md) binnen het platform om publieksgegevens veilig te delen. Om dit te doen, moeten zij gebruik maken van de [ privé verbindings uitnodigen ](../connect/establishing-connections.md#private-connection-invite) eigenschap. [!UICONTROL Luma] deelt hun verbindingscode met [!UICONTROL Fit Apparel], die het dan gebruikt om een verbindingsverzoek in werking te stellen. Nadat [!UICONTROL Luma] de verbindingsaanvraag heeft geaccepteerd, configureert [!UICONTROL Fit Apparel] de verbindingsinstellingen om te bepalen hoe ze zullen samenwerken. In de configuratie, [!UICONTROL Fit Apparel] specificeert dat beide medewerkers publiek voor marketing campagnes kunnen activeren. Om de verbinding te voltooien, accepteert [!UICONTROL Luma] het verzoek om een veilige koppeling tot stand te brengen tussen de twee merken.

Nadat de verbinding wordt gevestigd, [!UICONTROL Fit Apparel] [ leidt tot een project ](../collaborate/manage-projects.md) om van hun samenwerking met [!UICONTROL Luma] af te schoppen. Tijdens de projectopstelling, kiezen zij de gevallen van het samenwerkingsgebruik die hun doelstellingen het best passen: [ ontdekt ](../collaborate/discover.md), [ activeert ](../collaborate/activate.md), en [ Maatregel ](../collaborate/measure.md).

[!UICONTROL Fit Apparel] en [!UICONTROL Luma] kunnen zowel [ gebruiken ontdekken ](../collaborate/discover.md) gebruiksgeval om inzichten in elkaars publieksgegevens te bereiken. Zodra zij waardevolle publiekssegmenten hebben geïdentificeerd, activeren zij [&#128279;](../collaborate/activate.md) hun gekozen publiek voor marketing campagnes.

Tot slot na het uitvoeren van hun campagnes, uploaden beide merken gegevens aan [ Meetlat ](../collaborate/measure.md) de resultaten en evalueren de doeltreffendheid van hun samenwerking.
