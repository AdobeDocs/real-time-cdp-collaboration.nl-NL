---
title: Uw account configureren en beheren
description: Leer hoe u verschillende aspecten van uw account in Real-Time CDP Collaboration kunt configureren en beheren
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/nl/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: 608706d00124372ac59209478ab551a3a6ce0226
workflow-type: tm+mt
source-wordcount: '909'
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

<!-- Move the above popover to new section for invite on this page when its created -->

Als u wilt beginnen met het configureren van uw account, moet u eerst de accountgegevens instellen. Hiervoor moet u de volgende informatie toevoegen:

* Voeg een **[!UICONTROL Account name]** toe die duidelijk uw merk vertegenwoordigt.
* Voeg een **[!UICONTROL Description]** over uw merk toe. Dit is optioneel, maar het helpt andere medewerkers uw merk beter te begrijpen.
* Selecteer de **[!UICONTROL Role]** . U kunt kiezen tussen **[!UICONTROL Advertiser]** en **[!UICONTROL Publisher]** . Lees het [ werkschemadocument van begin tot eind ](/help/guide/end-to-end-workflow.md) om gelijkenissen en lichte verschillen in werkschema tussen de twee organisatorische roltypes te zien.
<!-- The above will need to be updated when I update things for B2B -->
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
>abstract="Identieke sleutels zijn herkenningstekens die worden gebruikt om leden over publiek van verschillende gegevensbronnen met elkaar in overeenstemming te brengen. Neem alle sleutels op waarmee uw merk kan werken."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_peopleIDs"
>title="ID&#39;s van eerstehulppersonen"
>abstract="Id&#39;s van eerstehulppersonen, zoals gehashte e-mailadressen of telefoonnummers, zijn rechtstreeks verbonden met een afzonderlijk profiel. Momenteel ondersteunde id&#39;s zijn gehashte e-mails en telefoonnummers."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_deviceIDs"
>title="Apparaat-id&#39;s van eerste partij"
>abstract="Apparaat-id&#39;s van de eerste partij, zoals ECID- of IP-adressen, zijn rechtstreeks verbonden met apparaten, die kunnen worden gedeeld tussen verschillende personen. IPv4 is de enige apparaat-id van de eerste partij die momenteel wordt ondersteund."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_partnerIDs"
>title="Ondersteunde partner-id&#39;s"
>abstract="Identiteitskaart van de partner verbonden aan profielen breidt het bereik tot een bepaald profiel uit."

>[!IMPORTANT]
>
>De sleutels die u tijdens de opstelling van de rekening selecteert zullen de beschikbare gelijke sleutels voor de verbindingen bepalen die u met andere medewerkers creeert. Terwijl u gelijke sleutels tijdens de verbindingsopstelling kunt verwijderen, kunt u geen nieuwe gelijke sleutels toevoegen. Het is belangrijk om **alle** gelijke sleutels te selecteren die u van plan bent in toekomstige campagnes tijdens de rekeningsopstelling te gebruiken.

De sleutels van de gelijke, zoals e-mailadressen, apparaat IDs, of klant IDs, helpen medewerkers samenwerken door nauwkeurige en privacy-centric gegevenssynchronisatie toe te laten, die voor nauwkeurigere publiek het richten en meting toestaat.

![ dia die de beschikbare herkenningstekens voor de eerste versie van Collaboration tonen.](/help/assets/setup/manage-account/available-identifiers.png)

<!-- Eventually replace this image above to match branding better. -->

Selecteer de sleutels die u wilt gebruiken om de profielen van het publiek met elkaar in overeenstemming te brengen. Neem alle overeenkomende toetsen op die u kunt gebruiken. Plan de toekomst en selecteer de sleutels van de gelijke die u in toekomstige campagnes zult gebruiken. Als u extra gelijke sleutels voor uw rekening in een recentere tijd moet selecteren, kunt u dit in het [ uitgeven rekening ](#edit-account) werkschema doen.

Selecteer maximaal vijf overeenkomende toetsen die u wilt gebruiken. Later kunt u bij het instellen van verbindingen ongewenste overeenkomende toetsen verwijderen, maar geen nieuwe toetsen toevoegen.

Er zijn drie typen beschikbare overeenstemmingssleutels:

* ID&#39;s van eerstehulppersonen
* Apparaat-id&#39;s van eerste partij
* Partner-id&#39;s

>[!IMPORTANT]
>
>Momenteel wordt hashed-e-mail de enige ondersteunde overeenkomende sleutel.

Als dit gereed is, selecteert u **[!UICONTROL Complete]** om de installatieworkflow van de organisatie te voltooien.

![ de de organisatiewerkruimte van de Opstelling met de getoonde sleutelensectie van de Gelijke.](/help/assets/setup/manage-account/add-account-match-keys.png){zoomable="yes"}

## Account bewerken {#edit-account}

Nadat u uw account hebt ingesteld, kunt u op elk gewenst moment bepaalde aspecten en details van het account bewerken. Als u uw account wilt bewerken, selecteert u **[!UICONTROL Edit]** in de sectie **[!UICONTROL My account]** van de **[!UICONTROL Setup]werkruimte** .

![ de werkruimte van de Opstelling met het Mijn benadrukte rekeningslusje en geeft optie uit.](/help/assets/setup/manage-account/edit-account.png){zoomable="yes"}

U kunt nu uw accountgegevens bewerken, met uitzondering van de extensie **[!UICONTROL Role]** . De regio wordt automatisch ingesteld op basis van uw Adobe Experience Cloud-account en kan op geen enkel moment worden gewijzigd.

![ de Edit dialoog van de rekeningsdetails.](/help/assets/setup/manage-account/editable-options.png){zoomable="yes"}

U kunt ook de sleutels bijwerken die u aanvankelijk selecteerde wanneer het aan boord gaan van uw organisatie. Selecteer **[!UICONTROL Edit]** in de **[!UICONTROL Match keys]** -sectie om extra gewenste overeenkomende toetsen toe te voegen.

![ de werkruimte van de Opstelling met Edit optie die binnen de de sleutelensectie van de Gelijke van de rekening wordt benadrukt.](/help/assets/setup/manage-account/edit-match-keys.png){zoomable="yes"}

## Volgende stappen

Na vestiging zijn uw rekeningen, u klaar aan [ bronpubliek ](/help/guide/setup/onboard-audiences.md) in Real-Time CDP Collaboration.
