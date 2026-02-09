---
title: Opmerkingen bij de nieuwste Real-Time CDP Collaboration-release
description: Volg de nieuwste releases voor Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 8513c648-1cc1-4544-b86d-2ee3193ab60f
source-git-commit: 8bda52a67f5a2bb733ecb6e28ae027e7092beba4
workflow-type: tm+mt
source-wordcount: '1383'
ht-degree: 2%

---

# Opmerkingen bij de nieuwste Real-Time CDP Collaboration-release

{{limited-availability-release-note}}

**Laatste update**: Januari 2026.

Deze releaseopmerkingen betreffen de functionaliteit die in Adobe Real-Time CDP Collaboration wordt vrijgegeven. Collaboration-releases werken op een doorlopend leveringsmodel, dat een gemiddelde maandelijkse release mogelijk maakt. Deze releaseopmerkingen worden vaak bijgewerkt, dus zorg ervoor dat u ze regelmatig controleert.

## Januari 2026 {#january-2026}

Real-Time CDP Collaboration biedt nu ondersteuning voor het uploaden van CSV-bestanden als een nieuwe methode voor het aanschaffen van soorten publiek en voor nieuwe mobiele sleutels (IDFA en GAID) voor betere overeenkomsten en metingen met het publiek.

**Nieuwe of bijgewerkte functies**

| Functie | Beschrijving |
| ------- | ----------- |
| CSV-upload voor audiobronnen | Upload CSV-bestanden rechtstreeks vanuit de gebruikersinterface naar Collaboration. Ideaal voor het instappen van gegevens van eerste partijen voor samenwerkingsprojecten op korte termijn. Voor meer informatie, zie het [&#x200B; CSV- dossier voor publiek dat gids &#x200B;](../setup/upload-csv-audience-sourcing.md) levert. |
| Ondersteuning voor Key afstemmen op mobiele apparaten | Collaboration biedt nu ondersteuning voor mobiele match-keys, waaronder IDFA en GAID, voor publieksmatching en -metingen. Deze gelijke sleutels worden geselecteerd tijdens rekeningsopstelling en kunnen dan worden gebruikt wanneer het vormen van verbindingsmontages voor nieuwe verbindingen en in stroomafwaartse samenwerkingswerkschema&#39;s. Zie de [&#x200B; gids van de de toetsenopstelling van de Gelijke &#x200B;](../setup/onboard-account.md#set-up-match-keys) voor meer details. |

{style="table-layout:auto"}

## December 2025 {#december-2025}

Real-Time CDP Collaboration is nu beschikbaar aan klanten in **Europa, het Midden-Oosten, en Afrika (EMEA)**. Deze service is automatisch beschikbaar voor Real-Time CDP Prime- en Ultimate-klanten in deze regio&#39;s.

## Augustus 2025 {#august-2025}

Real-Time CDP Collaboration is nu beschikbaar aan klanten in **Canada**. Deze service is automatisch beschikbaar voor Real-Time CDP Prime- en Ultimate-klanten in deze regio&#39;s.

* Collaboration steunt nu de volgende [&#x200B; gelijke sleutels &#x200B;](../setup/onboard-account.md#supported-match-keys):
   * Onderbroken e-mail
   * Onderbroken telefoonnummer
   * CRM-id
   * Loyalty-id
   * Onderbroken IPv4
   * Id van advertentie
* Er zijn nu meerdere match-keys beschikbaar in Collaboration, waardoor je het publiek groter kunt maken en de match-rates kunt verbeteren. De veelvoudige gelijke sleutels kunnen worden gebruikt wanneer het bronpubliek, het vestigen van verbindingen, en het activeren van publiek. Meer leren over het gebruiken van veelvoudige gelijke sleutels, leest de [&#x200B; opstellingssleutels &#x200B;](../setup/onboard-account.md) en [&#x200B; die publiek &#x200B;](../setup/onboard-audiences.md#map-fields) gidsen aantrekken.

>[!IMPORTANT]
>
>Wanneer het activeren van publiek waar de veelvoudige gelijke sleutels worden gebruikt, als één (of meer) gelijke sleutel geen overlappingen heeft, geen kijkcijfers van het publiek, of onder drempel daalt, zal de volledige activering ontbreken. Zorg ervoor dat uw publiek voldoende overlap heeft en dat het voldoet aan de minimumdrempel van 1000 id&#39;s voor alle overeenkomende toetsen voordat het wordt geactiveerd.

* De bestemming van Adobe Experience Platform steunt nu het activeren van publiek met veelvoudige gelijke sleutels. Bovendien, kunt u nu een verbonden sleutel gebruiken wanneer het vormen van de afbeelding van uw bestemming om te specificeren welke gelijke sleutel tijdens activering wordt verzonden. Meer leren, lees de [&#x200B; bestemming van Experience Platform &#x200B;](../destinations/experience-platform.md#linked-keys) gids.
* Medewerkers kunnen nu meerdere soorten publiek tegelijk bewerken. U kunt de metagegevens van het publiek, de toegang tot de verbinding, namen, beschrijvingen en categorieën voor meerdere soorten publiek nu bewerken met het gereedschap voor bulkbewerking. Meer leren over het uitgeven publiek, leest [&#x200B; publiek &#x200B;](../setup/onboard-audiences.md#edit-audiences) gids beheren.

## Juli 2025 {#july-2025}

CDP Collaboration in realtime ondersteunt nu merkgebonden samenwerking. Medewerkers kunnen nu verbindingen maken, ongeacht of ze adverteerders of uitgevers zijn. Dit maakt flexibelere samenwerkingsmogelijkheden mogelijk en stelt merken in staat elkaars gegevens en inzichten te benutten. Meer over de verschillen tussen merk-aan-merk samenwerking en adverteerder-aan-uitgever samenwerking leren, lees de [&#x200B; gids van de 0&rbrace; samenwerkingspatronen &lbrace;.](../overview/collaboration-patterns.md)

* De medewerkers kunnen nu met elkaar verbinden gebruikend [&#x200B; privé verbinding nodigt &#x200B;](../connect/establishing-connections.md#private-connection-invites) uit. Deel de unieke verbindingscode van uw account met een medewerker die deze vervolgens kan gebruiken om rechtstreeks verbinding met u te maken. Dit is een kernkenmerk van merkgebonden samenwerking, waardoor medewerkers naast adverteerders ook verbindingen tot stand kunnen brengen om de map **[!UICONTROL Discover collaborators]** te verkennen.
* [&#x200B; Zelf-serverbestemmingen &#x200B;](../setup/manage-destinations.md) zijn nu beschikbaar aan zowel adverteerders als uitgevers.
* De activering van het publiek is nu beschikbaar voor beide medewerkers in een verbinding, ongeacht hun [&#x200B; rekeningsrol &#x200B;](../overview/roles.md). De activeringsmontages van het publiek worden gevormd terwijl [&#x200B; het vestigen van verbindingen &#x200B;](../connect/establishing-connections.md#configure-connection-settings), toestaand u om te specificeren welke samenwerker publiek kan activeren. Meer over publieksactivering leren, lees [&#x200B; activeer publiek &#x200B;](../collaborate/activate.md) gids.
* De gebruikszaak van **[!UICONTROL Activate]** is opnieuw geconfigureerd ter ondersteuning van de samenwerking tussen merken en merken. Het tabblad **[!UICONTROL Activate]** in een project geeft nu het publiek weer dat naar uw medewerker is verzonden en het publiek dat door uw medewerker naar uw doel is geactiveerd. Meer leren, lees [&#x200B; activeer publiek &#x200B;](../collaborate/activate.md) gids. <br> ![&#x200B; activeer dashboard met het publiek naar en het publiek activeerde secties wordt verzonden die.](/help/assets/release-notes/2025/activate-dashboard.png){zoomable="yes"}
* De scores voor de index van het publiek zijn nu beschikbaar op het tabblad **[!UICONTROL Discover]** van een project. De score van de publieksindex is een maat voor de mate waarin een publiek overeenkomt met het publiek van uw medewerker. Deze score wordt berekend op basis van het aantal onderliggende doelgroepen en de overlappingen. Meer over de scores van de publieksindex leren, lees de [&#x200B; score van de publieksindex &#x200B;](../collaborate/discover.md#audience-index-score) gids.

## Mei 2025 {#may-2025}

* Real-Time CDP Collaboration is nu beschikbaar aan klanten in **Australië** en **Nieuw Zeeland**. Deze service is automatisch beschikbaar voor Real-Time CDP Prime- en Ultimate-klanten in deze regio&#39;s.
* Real-Time CDP Collaboration biedt nu [&#x200B; zelf-serverbestemmingen &#x200B;](../setup/manage-destinations.md) door het **[!UICONTROL My destinations]** lusje in de **[!UICONTROL Setup]** sectie aan. Met doelen kunt u het publiek activeren op externe platforms, zoals advertentienetwerken of platforms voor gegevensbeheer, zodat u uw klanten op verschillende kanalen kunt bereiken. Momenteel worden alleen Adobe Experience Platform-doelen ondersteund. Neem contact op met uw Adobe-vertegenwoordiger als u een andere bestemming wilt configureren. Meer over bestemmingen leren, lees de [&#x200B; gids van het bestemmingsoverzicht &#x200B;](../destinations/overview.md).
   * De bestemmingen voegen ook steun toe om het publiek van Collaboration in het [&#x200B; het publieksportaal van Adobe Experience Platform &#x200B;](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences) te bekijken.
* U kunt de publieksvernieuwingsfrequentie voor bestaande gegevensverbindingen in Collaboration nu bewerken. Op dit moment kunt u ervoor kiezen uw publiek dagelijks of om de twee tot zes dagen te vernieuwen. Meer over leren hoe te om het publiek uit te geven verfrist frequentie, leest [&#x200B; gegevensverbindingen &#x200B;](../setup/manage-data-connection.md#scheduling) gids beheren.
* De splitsingen van het krediet tussen medewerkers worden nu geplaatst voor elk gebruiksgeval dat binnen de verbinding wordt geselecteerd. U kunt verschillende regels voor kredietverbruik instellen voor elk geval van gebruik om beter te kunnen bepalen hoe je crediteringen worden gebruikt. Meer over de functie van de creditspleet leren, lees de [&#x200B; gids van verbindingsmontages &#x200B;](../connect/establishing-connections.md#connection-settings). Om meer over te leren hoe de kredieten worden verbruikt, lees de [&#x200B; gids van de kredietactiviteit &#x200B;](../setup/my-activity.md#types-of-activities). <br> ![&#x200B; het montagesscherm dat van de Verbinding de functionaliteit van de creditsplits toont.](/help/assets/release-notes/2025/credit-split.png){zoomable="yes"}
* Uitgevers kunnen nu namen en id&#39;s van adverteerders instellen voordat ze de verbindingsinstellingen van een adverteerder accepteren. Uitgevers kunnen namen en id&#39;s instellen die worden uitgelijnd op hun interne systemen. Deze namen kunnen verschillen van de namen en id&#39;s van de adverteerder. Meer over het toevoegen van adverteerdernamen en IDs leren, lees de [&#x200B; gids van verbindingsmontages &#x200B;](../connect/establishing-connections.md#connection-settings.md). <br> ![&#x200B; het montagesscherm dat van de Verbinding de uitgever toont die adverteerdernamen en IDs plaatsen.](/help/assets/release-notes/2025/add-advertiser-names-modal.png){zoomable="yes"}

## April 2025 {#april-2025}

* Er is een nieuwe kolom **[!UICONTROL Inputs Processed]** toegevoegd aan de tabel met kredietverbruiksactiviteiten. In deze kolom wordt het totale aantal inputs (bijvoorbeeld id&#39;s of rijen) weergegeven dat voor elke activiteit is verwerkt. [&#x200B; las meer &#x200B;](/help/guide/setup/my-activity.md#inputs-processed). <br> ![&#x200B; Inputs verwerkte kolom die in Mijn activiteitenmening wordt benadrukt.](/help/assets/release-notes/2025/inputs-processed-column.png){zoomable="yes"}
* Er is een nieuwe e-mailoptie voor contact toegevoegd aan het maken van een account. Dit helpt de medewerkers van de partner uit u bereiken zoals nodig tijdens het verbindingsproces. [Meer informatie](../setup/onboard-account.md).

## Maart 2025 {#march-2025}

* Wanneer [&#x200B; het sourcen publiek &#x200B;](/help/guide/setup/onboard-audiences.md) in Collaboration, kunt u een publiek nu plaatsen verfrist frequentie van **elke tot zes dagen** om de [&#x200B; de kredietactiviteit van het Beheer van de Publiek &#x200B;](/help/guide/setup/my-activity.md#types-of-activities) beter te beheren. Voor meer informatie, leest [&#x200B; publiek &#x200B;](https://experienceleague.adobe.com/en/docs/experience-platform/segmentation/ui/audience-portal.md#manage-audiences) gids beheren. <br> ![&#x200B; het scherm dat van het Programma verschillende frequentiedetails voor het bijwerken van publiekslidmaatschap toont.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png " het scherm dat van het Programma verschillende frequentiedetails voor het bijwerken van publiekslidmaatschap toont."){width="250" align="center" zoomable="yes"}
* Wanneer het vestigen van een verbinding met een medewerker, kunt u van vooraf bepaalde **gebruiksgevallen** nu selecteren. De geselecteerde gebruikscase bepaalt welke projectsecties en productfunctionaliteit beschikbaar worden. Voor meer informatie, lees [&#x200B; projecten &#x200B;](/help/guide/collaborate/manage-projects.md#project-use-cases) gids leiden.
   * *Metingen* laat de **sectie van het het projectproject van de Maatregel** toe.
   * *de ontdekking van het publiek* laat **toe ontdekt** projectsectie.
   * *activering van het publiek* laat **toe activeert** projectsecties <br>
* U kunt nu verbindingen verwijderen met deelnemers waarmee u niet meer wilt werken. Leren hoe te om verbindingen te schrappen, lees [&#x200B; schrappend verbindingen &#x200B;](/help/guide/connect/establishing-connections.md#delete-connections) gids.

## Februari 2025 {#february-2025}

Adobe Real-Time CDP Collaboration, dat speciaal is ontworpen om adverteerders en uitgevers in staat te stellen hoogwaardig publiek zonder cookies van derden te detecteren, activeren en meten, is nu in de Verenigde Staten algemeen beschikbaar.

### Aan de slag

1. **Opstelling van de Toegang**: De beheerders van het systeem vormen toegangstoestemmingen voor gebruikers. Meer leren over het vormen van toegangstoestemmingen, leest [&#x200B; gebruikerstoegang &#x200B;](/help/guide/permissions/manage-user-access.md#RTCDP-collaboration-access) gids.
2. **verbind Gegevensbronnen**: Het publiek van Source aan gebruik in Collaboration. Beginnen bronsend publiek, lees de [&#x200B; bron en beheer publiek &#x200B;](/help/guide/setup/onboard-audiences.md) gids.
3. **Vestig Verbindingen**: Begin werkend met vertrouwde op adverteerders of uitgevers. Meer leren over het vormen van verbindingen, lees [&#x200B; het vestigen van verbindingen &#x200B;](/help/guide/connect/establishing-connections.md) gids.
4. **ontdekt en activeert**: Creeer projecten om waardevolle publiek te identificeren in campagnes te activeren. Meer leren over het creëren van projecten, lees [&#x200B; projecten &#x200B;](/help/guide/collaborate/manage-projects.md) gids leiden.

### Beschikbaarheid

* Adobe Real-Time CDP Collaboration is momenteel alleen beschikbaar voor klanten in de VS.
* Deze service is automatisch beschikbaar voor Adobe Real-Time CDP Prime- en Ultimate-klanten

Lees voor meer informatie het volgende:

* [Collaboration-overzicht](/help/guide/home.md)
* [End-to-end workflow](/help/guide/overview/end-to-end-workflow.md)
* [Overzicht van machtigingen](/help/guide/permissions/overview.md)
