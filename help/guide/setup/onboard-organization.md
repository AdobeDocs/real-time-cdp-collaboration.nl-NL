---
title: Ingebouwde en beheerde organisatie
description: Leer hoe u verschillende aspecten van uw organisatie in Real-Time CDP Collaboration kunt opnemen en beheren
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/nl/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: fda414120decc0c76712616ff85b83febede53e9
workflow-type: tm+mt
source-wordcount: '828'
ht-degree: 0%

---

# Aan boord en beheer uw organisatie

{{limited-availability-release-note}}

Leer hoe u uw bedrijf op Real-Time CDP Collaboration kunt inbouwen en verschillende aspecten van uw bedrijf kunt beheren. Deze pagina bevat een overzicht van de stappen die een organisatie moet uitvoeren naar Adobe Real-Time CDP Collaboration, zoals het instellen van de sleutels voor overeenkomsten, de voorkeursidentiteiten en meer opties.

![ de opstellingswerkruimte van de organisatie die zijn huidige montages tonen.](/help/assets/setup/manage-organization/my-organization.png){zoomable="yes"}

## Eerste configuratie van organisatie

U moet eerst uw organisatie en organisatorische details instellen. Als dit uw eerste organisatie is, zult u door het onboarding proces onmiddellijk worden geleid, beginnend met vestiging uw [ rekeningsdetails ](#set-up-details).

Om extra organisaties toe te voegen, navigeer aan **[!UICONTROL Setup]** in het linkerspoor en selecteer het toevoegingspictogram (![ voeg pictogram toe.](/help/assets/icons/plus.png) ) in de rechterbovenhoek. Selecteer vervolgens **[!UICONTROL Account]** .

![ de opstellingswerkruimte met de benadrukte optie van de Rekening.](/help/assets/setup/manage-organization/add-new-account.png){zoomable="yes"}

### Details instellen {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="E-mailadres"
>abstract="Geef een team of op rol gebaseerde e-mail op, bijvoorbeeld `collaboration@yourcompany.com` . Persoonlijke of individuele e-mailadressen mogen niet worden gebruikt."

Als u aan boord van uw organisatie wilt gaan, moet u eerst de organisatiedetails instellen. Hiervoor moet u de volgende informatie toevoegen:

* Voeg een **[!UICONTROL Organization name]** voor uw bedrijf toe.
* Voeg een **[!UICONTROL Description]** over uw bedrijf toe.
* Selecteer de **[!UICONTROL Company role]** . U kunt kiezen tussen **[!UICONTROL Advertiser]** en **[!UICONTROL Publisher]** . Lees het [ werkschemadocument van begin tot eind ](/help/guide/end-to-end-workflow.md) om gelijkenissen en lichte verschillen in werkschema tussen de twee organisatorische roltypes te zien.
* Selecteer de **[!UICONTROL Industry]** voor uw organisatie. Voorbeelden zijn **[!UICONTROL Retail]** , **[!UICONTROL Telecommunications]** of **[!UICONTROL Financial services]** .
* Selecteer de **[!UICONTROL Region]** voor uw organisatie. In de huidige versie van het product is **[!UICONTROL North America]** de standaardselectie met voorinstellingen.
* Voeg een **[!UICONTROL Contact email]** toe voor uw organisatie. Dit moet een team of een op rollen gebaseerd e-mailadres zijn. Persoonlijke e-mailadressen mogen niet worden opgegeven.
* Upload een **[!UICONTROL Logo]** voor uw bedrijf. Op dit moment worden SVG-afbeeldingen ondersteund.
* Selecteer een afbeelding voor de koptekst van uw bedrijf.

>[!NOTE]
>
>Hoewel u de meeste van deze details op elk moment kunt bewerken, zijn de **[!UICONTROL Role]** en **[!UICONTROL Region]** niet bewerkbaar na de eerste setup.

![ de de organisatiewerkruimte van de Opstelling met de getoonde sectie van Details.](/help/assets/setup/manage-organization/add-organization-details.png){zoomable="yes"}

Wanneer u klaar bent, gebruikt u **[!UICONTROL Next]** om door te gaan naar de volgende pagina om de gewenste gelijke sleutels te selecteren uw organisatie zal gebruiken.

### Overeenkomstsleutels instellen {#set-up-match-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_organization_onboarding_matchkeys"
>title="Toetsen afstemmen"
>abstract="Identieke sleutels zijn herkenningstekens die worden gebruikt om leden over publiek van verschillende gegevensbronnen met elkaar in overeenstemming te brengen. Neem alle sleutels op die uw bedrijf kan gebruiken."

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
>Met de sleutels die u tijdens de installatie van de organisatie selecteert, worden de beschikbare overeenkomende sleutels bepaald voor de verbindingen die u met andere organisaties maakt. Terwijl u gelijke sleutels tijdens de verbindingsopstelling kunt verwijderen, kunt u geen nieuwe gelijke sleutels later toevoegen. Het is belangrijk om alle gelijke sleutels te selecteren die u in toekomstige campagnes tijdens de organisatorische opstelling wilt gebruiken.

Identieke sleutels, zoals e-mailadressen, apparaat-id&#39;s of klant-id&#39;s, helpen adverteerders en uitgevers samen door nauwkeurige en privacygerichte gegevenssynchronisatie in te schakelen, waardoor doelgerichtere doelgroepen en meetwaarden mogelijk zijn.

![ dia die de beschikbare herkenningstekens voor de eerste versie van Real-Time CDP Collaboration tonen.](/help/assets/setup/manage-organization/available-identifiers.png)

Selecteer de sleutels die u wilt gebruiken wanneer het in overeenstemming brengen van leden van uitgever en adverteerderpubliek. Neem alle sleutels op die uw bedrijf kan gebruiken. Plan voor de toekomst en selecteer de wedstrijdsleutels die u in toekomstige uitgever-adverteerders campagnes zult gebruiken. Als u extra gelijke sleutels voor uw organisatie moet selecteren, kunt u dat in een recentere tijd ook doen, in [ organisatie ](#edit-organization) werkschema uitgeven.

![ de de organisatiewerkruimte van de Opstelling met de getoonde sleutelensectie van de Gelijke.](/help/assets/setup/manage-organization/add-organization-match-keys.png){zoomable="yes"}

Selecteer maximaal vijf overeenkomende toetsen die u wilt gebruiken. Later kunt u bij het instellen van verbindingen ongewenste overeenkomende toetsen verwijderen, maar geen nieuwe toetsen toevoegen.

De beschikbare sleutels van gelijke in Real-Time CDP Collaboration kunnen van drie types zijn:

* ID&#39;s van eerstehulppersonen
* Apparaat-id&#39;s van eerste partij
* Partner-id&#39;s

De beschikbare match keys voor de eerste release van Real-Time CDP Collaboration zijn:

* Onderbroken e-mail

Als dit gereed is, selecteert u **[!UICONTROL Complete]** om de installatieworkflow van de organisatie te voltooien.

## Organisatie bewerken {#edit-organization}

Nadat u uw organisatie voor het eerst hebt ingesteld, kunt u op elk gewenst moment bepaalde aspecten en details van de organisatie bewerken. Als u uw organisatie wilt bewerken, selecteert u **[!UICONTROL Edit]** in de sectie **[!UICONTROL My organization]** van de **[!UICONTROL Setup]werkruimte** .

![ de werkruimte van de Opstelling met het Mijn benadrukte organisatielusje en geeft optie uit.](/help/assets/setup/manage-organization/edit-organization.png){zoomable="yes"}

U kunt nu de organisatiedetails bewerken, met uitzondering van **[!UICONTROL Role]** en **[!UICONTROL Region]** .

![ de Edit dialoog van organisatiedetails.](/help/assets/setup/manage-organization/editable-options.png){zoomable="yes"}

U kunt ook de sleutels bijwerken die u aanvankelijk selecteerde wanneer het aan boord gaan van uw organisatie. Selecteer **[!UICONTROL Edit]** in de **[!UICONTROL Match keys]** -sectie om extra gewenste overeenkomende toetsen toe te voegen.

![ de werkruimte van de Opstelling met Edit optie die binnen de de sleutelensectie van de Gelijke van de organisatie wordt benadrukt.](/help/assets/setup/manage-organization/edit-match-keys.png){zoomable="yes"}

## Volgende stappen

Na vestiging uw organisatie, bent u bereid om [ publiek ](/help/guide/setup/onboard-audiences.md) in Real-Time CDP Collaboration in te voeren.
