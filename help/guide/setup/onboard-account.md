---
title: Uw account configureren en beheren
description: Leer hoe u verschillende aspecten van uw account in Real-Time CDP Collaboration kunt configureren en beheren
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: 0dead396657c97cec47ddd64c8ec3c349f541a8f
workflow-type: tm+mt
source-wordcount: '1297'
ht-degree: 0%

---

# Uw account configureren en beheren

{{limited-availability-release-note}}

Leer hoe u uw account in Real-Time CDP Collaboration instelt als voorbereiding op verbindingen met andere medewerkers. Deze handleiding behandelt de eerste installatie van uw account, zoals het toevoegen van accountgegevens, het selecteren van sleutels en het beheren van de instellingen van uw account.

![ de opstellingswerkruimte die een gevormde rekening tonen.](/help/assets/setup/manage-account/my-account.png){zoomable="yes"}

## Uw account instellen {#set-up-account}

Wanneer u voor het eerst Collaboration opent, wordt u gevraagd uw account in te stellen. Dit is een eenmalig proces waarmee u uw accountgegevens kunt configureren en toetsen kunt afstemmen. Als dit de eerste rekening van uw organisatie is, zult u door het onboarding proces onmiddellijk worden geleid, beginnend met vestiging uw [ rekeningsdetails ](#set-up-details).

Om extra organisaties toe te voegen, navigeer aan **[!UICONTROL Setup]** in het linkerspoor en selecteer het toevoegingspictogram (![ voeg pictogram toe.](/help/assets/icons/plus.png) ) in de rechterbovenhoek. Selecteer vervolgens **[!UICONTROL Account]** .

![ de opstellingswerkruimte met de Mijn benadrukte de rekeningslusje en optie van de Rekening.](/help/assets/setup/manage-account/add-new-account.png){zoomable="yes"}

### Details instellen {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="E-mailadres"
>abstract="Gelieve te verstrekken een team of op rol-gebaseerde e-mail, zoals **collaboration@yourcompany.com**. Persoonlijke of individuele e-mailadressen mogen niet worden gebruikt."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_connect_code"
>title="Verbindingscode"
>abstract="De verbindingscode is een unieke id voor uw account. Het wordt gebruikt om verbindingen met andere medewerkers in Real-Time CDP Collaboration tot stand te brengen."

Als u wilt beginnen met het configureren van uw account, moet u eerst de accountgegevens instellen. Hiervoor moet u de volgende informatie toevoegen:

* Voeg een **[!UICONTROL Account name]** toe die duidelijk uw merk vertegenwoordigt.
* Voeg een **[!UICONTROL Description]** over uw merk toe. Dit is optioneel, maar het helpt andere medewerkers uw merk beter te begrijpen.
* Selecteer de **[!UICONTROL Role]** . U kunt kiezen tussen **[!UICONTROL Advertiser]** en **[!UICONTROL Publisher]** . Lees de [ rollen ](/help/guide/overview/roles.md) gids om gelijkenissen en lichte verschillen in werkschema tussen de twee types van rekeningsrol te zien.
* Selecteer de **[!UICONTROL Industry]** voor uw account. Voorbeelden zijn **[!UICONTROL Retail]** , **[!UICONTROL Telecommunications]** of **[!UICONTROL Financial services]** .
* **[!UICONTROL Region]** wordt automatisch ingesteld op basis van uw Adobe Experience Cloud-account. Dit kan op geen enkel moment worden gewijzigd.
* Voeg een **[!UICONTROL Contact email]** voor uw account toe. Dit moet een team of een op rollen gebaseerd e-mailadres zijn. Persoonlijke e-mailadressen mogen niet worden opgegeven.
* Upload een **[!UICONTROL Logo]** voor uw account. Op dit moment worden SVG-afbeeldingen ondersteund. Dit is optioneel, maar het uploaden van een logo helpt uw merk in de Collaboration-interface visueel weer te geven
* Selecteer een afbeelding voor de koptekst van uw account.

>[!NOTE]
>
>U kunt de meeste van deze details op elk gewenst moment bewerken, maar de **[!UICONTROL Role]** kan na de eerste installatie niet meer worden bewerkt. Wanneer u klaar bent, gebruikt u **[!UICONTROL Next]** om door te gaan naar de volgende pagina om de gewenste gelijke sleutels te selecteren uw organisatie zal gebruiken.

![ de de rekeningswerkruimte van de Opstelling met de getoonde sectie van Details en de Volgende benadrukte optie.](/help/assets/setup/manage-account/add-account-details.png){zoomable="yes"}

### Overeenkomstsleutels instellen {#set-up-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_matchkeys"
>title="Toetsen afstemmen"
>abstract="Identieke sleutels zijn herkenningstekens die worden gebruikt om publieksprofielen van verschillende gegevensbronnen met elkaar in overeenstemming te brengen. Neem alle sleutels op waarmee uw merk kan werken."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_setup_match_keys"
>title="match keys"
>abstract=""

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_peopleIDs"
>title="ID&#39;s van eerstehulppersonen"
>abstract="Id&#39;s van eerstehulppersonen, zoals gehashte e-mailadressen, gehashte telefoonnummers of CRM-id&#39;s, zijn rechtstreeks verbonden met een afzonderlijk profiel."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_deviceIDs"
>title="Apparaat-id&#39;s van eerste partij"
>abstract="Apparaat-id&#39;s van de eerste partij, zoals ECID- of IP-adressen, zijn rechtstreeks verbonden met apparaten, die kunnen worden gedeeld tussen verschillende personen. IPv4 is de enige apparaat-id van de eerste partij die momenteel wordt ondersteund."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_partnerIDs"
>title="Ondersteunde partner-id&#39;s"
>abstract="Identiteitskaart van de partner is herkenningstekens die door externe partners voor publieksverzoening worden verstrekt. Identiteitskaart van de partner wordt niet direct verbonden met een individueel profiel."

![ Gesteunde gelijke sleutels.](/help/assets/setup/manage-account/match-keys.png){zoomable="yes"}

>[!IMPORTANT]
>
>De sleutels die u tijdens de opstelling van de rekening selecteert zullen de beschikbare gelijke sleutels binnen uw verbindingen bepalen. Terwijl u [ ongewenste gelijke sleutels ](../connect/establishing-connections.md#connection-settings) tijdens de verbindingsopstelling kunt verwijderen, passen geen sleutels kunnen worden toegevoegd nadat een verbinding is gevestigd. Het is belangrijk dat u **alle** gelijke sleutels selecteert die u van plan bent in toekomstige campagnes tijdens de rekeningsopstelling te gebruiken.

Met Identieke sleutels kunnen medewerkers samenwerken door nauwkeurige en privacygerichte gegevenssynchronisatie in te schakelen, waardoor doelgerichtere doelgroepen en meetwaarden mogelijk zijn. Welke sleutels beschikbaar zijn in toekomstige verbindingen, wordt bepaald door de toetsen die tijdens het instellen van de account zijn geselecteerd. Zij worden ook gebruikt aan [ kaartgebieden ](./onboard-audiences.md#map-fields) van uw gegevensverbinding aan de doelgebieden in Collaboration wanneer het betrekken van publiek.

Selecteer de sleutels die u wilt gebruiken om de profielen van het publiek met elkaar in overeenstemming te brengen. Plan de toekomst en neem alle sleutels op waarmee u kunt werken en waarmee u kunt anticiperen in toekomstige campagnes. Als u extra gelijke sleutels voor uw rekening in een recentere tijd moet selecteren, kunt u dit in het [ uitgeven rekening ](#edit-account) werkschema doen. Eventuele na de eerste installatie toegevoegde sleutels zijn echter niet beschikbaar voor gebruik in bestaande verbindingen.

#### Ondersteunde match keys {#supported-match-keys}

Collaboration ondersteunt drie typen sleutels: id&#39;s voor eerste mensen, id&#39;s voor eerste apparaten en id&#39;s voor partners. Alle gelijke sleutels moeten aan de volgende vereisten voldoen:

* De sleutels van de gelijke moeten **worden in orde gebracht**, **lager gecaste**
* De gehakte gelijke sleutels moeten **SHA256-gehakt** zijn.
* Als u hashwaarden opgeeft waarin hoofdletters worden gebruikt, zet Collaboration deze automatisch om in kleine letters.
* Als uw bron **plaintext herkenningstekens** bevat, gebruik de **[!UICONTROL Apply transformation]** optie tijdens uw [ opstelling van de gegevensverbinding ](./manage-data-connection.md#match-keys) om het hakken toe te passen. Deze optie is alleen beschikbaar wanneer gebruikers worden aangeschaft bij Experience Platform en wordt niet ondersteund voor bronnen in de cloud.

##### ID&#39;s van eerstehulppersonen

ID&#39;s van eersteklas personen zijn rechtstreeks verbonden met een afzonderlijk profiel. Momenteel ondersteunde id&#39;s zijn:

* **[!UICONTROL Hashed email]**
* **[!UICONTROL Hashed phone]**
* **[!UICONTROL CRM IDs]**
* **[!UICONTROL Loyalty IDs]**
<!-- * **[!UICONTROL Custom ID]**: Custom identifiers -->

##### Apparaat-id&#39;s van eerste partij

Apparaat-id&#39;s van de eerste partij zijn id&#39;s die zijn verbonden met een specifiek apparaat. Momenteel ondersteunde id&#39;s zijn:

* **[!UICONTROL Hashed IPv4]**: onderbroken IPv4-adressen

##### Partner-id&#39;s

Identiteitskaart van de partner is herkenningstekens die door externe partners voor publieksverzoening worden verstrekt. Momenteel ondersteunde id&#39;s zijn:

* **[!UICONTROL Adfixus ID]**

>[!NOTE]
>
>Adobe-integratie met [!DNL Adfixus] wijst de unieke [!UICONTROL Adfixus IDs] voor elke account toe aan een algemene Adobe-gecodeerde indeling. Deze toewijzingen worden gebruikt om overlappingen tussen deelnemers te identificeren. Wanneer u een publiek activeert met **[!UICONTROL Adfixus ID]** , worden de oorspronkelijke id&#39;s gebruikt. De Adobe-gecodeerde indeling verlaat Collaboration nooit.

Als u **[!UICONTROL Adfixus ID]** selecteert, moet u de bijbehorende id opgeven van uw externe partner in de sectie **[!UICONTROL Account credentials]** . Deze optie zal slechts beschikbaar zijn *na* het van een knevel voorzien **[!UICONTROL Adfixus ID]**. Voer uw Adfixus-id in het veld **[!UICONTROL Account ID]** in, waarbij u zeker weet dat u de waarde nogmaals controleert op nauwkeurigheid.

![ de de sleuteldialoog van de Gelijke met identiteitskaart Adfixus schakelde en benadrukte sectie van de geloofsbrieven van de Rekening aan.](/help/assets/setup/manage-account/adfixus-settings.png){zoomable="yes"}

Nadat u alle gewenste overeenkomende toetsen hebt geselecteerd, selecteert u **[!UICONTROL Complete]** om de workflow voor het instellen van de account te voltooien.

![ de de rekeningswerkruimte van de Opstelling met de getoonde sleutelensectie van de Gelijke.](/help/assets/setup/manage-account/add-account-match-keys.png){zoomable="yes"}

## Account bewerken {#edit-account}

Nadat u uw account hebt ingesteld, kunt u op elk gewenst moment de details en de sleutels bewerken.

### Details bewerken {#edit-details}

U kunt de meeste details van uw account op elk gewenst moment bewerken, met uitzondering van de **[!UICONTROL Role]** . Het gebied wordt automatisch ingesteld op basis van uw Adobe Experience Cloud-account en kan niet worden gewijzigd.

Als u uw account wilt bewerken, selecteert u **[!UICONTROL Edit]** in het gedeelte **[!UICONTROL My account]** van de **[!UICONTROL Setup]** -werkruimte.

![ de werkruimte van de Opstelling met het Mijn benadrukte rekeningslusje en geeft optie uit.](/help/assets/setup/manage-account/edit-account.png){zoomable="yes"}

U kunt nu uw accountgegevens bewerken. Werk de velden bij die u wilt wijzigen en selecteer vervolgens **[!UICONTROL Save]** om de wijzigingen te bevestigen.

![ de Edit dialoog van de rekeningsdetails.](/help/assets/setup/manage-account/editable-options.png){zoomable="yes"}

### Overeenkomstsleutels bewerken {#edit-match-keys}

>[!IMPORTANT]
>
>Het bewerken van match keys heeft geen invloed op je bestaande verbindingen. Zodra een verbinding is gevestigd, zijn de gelijke sleutels die u tijdens de verbindingsopstelling selecteert vast. Het is belangrijk dat u **alle** gelijke sleutels selecteert die u van plan bent in toekomstige campagnes tijdens de rekeningsopstelling te gebruiken.

U kunt ook de sleutels bijwerken die u aanvankelijk selecteerde toen het creëren van uw rekening. Deze gelijke sleutels zullen de gelijke sleutels bepalen beschikbaar aan toekomstige verbindingen.

Selecteer **[!UICONTROL Edit]** in de sectie **[!UICONTROL Match keys]** .

![ de werkruimte van de Opstelling met Edit optie die binnen de de sleutelensectie van de Gelijke van de rekening wordt benadrukt.](/help/assets/setup/manage-account/edit-match-keys.png){zoomable="yes"}

Het dialoogvenster **[!UICONTROL Match keys]** wordt weergegeven. Schakel eventuele overeenkomende toetsen in of uit of werk de **[!UICONTROL Account ID]** for your [!UICONTROL Adfixus ID's] bij en selecteer **[!UICONTROL Save]** om de wijzigingen te bevestigen.

>[!IMPORTANT]
>
>Het veranderen van uw [!UICONTROL Adfixus ID] zal a [ gegevensschets ](../glossary.md#sketches) niet teweegbrengen voor uw bestaande gegevensverbindingen gebruikend de gelijke sleutel verfrissen. Zodra uw gegevens zijn geschetst, zullen om het even welke veranderingen in uw [!UICONTROL Adfixus ID] niet worden weerspiegeld tot uw volgende publiek zich na uw [ schema van de gegevensverbinding ](./manage-data-connection.md#scheduling) montages verfrist. Als u wijzigingen moet aanbrengen voordat u verdergaat, kunt u de gegevensverbinding verwijderen en opnieuw maken.

![ de dialoog van de sleutels van de Gelijke met sparen benadrukte optie.](/help/assets/setup/manage-account/match-key-dialog.png){zoomable="yes"}

## Volgende stappen

Na vestiging zijn uw rekeningen, u klaar aan [ bronpubliek ](/help/guide/setup/onboard-audiences.md) in Real-Time CDP Collaboration.
