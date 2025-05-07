---
title: Ingebouwde en beheerde organisatie
description: Leer hoe u verschillende aspecten van uw organisatie in Real-Time CDP Collaboration kunt opnemen en beheren
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: a95e932a-9681-48f2-bf34-6fe5a50597d7
source-git-commit: 27faef284a07be114ea0a9a7beeae75ec6265d53
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# Ingebouwde en beheerde organisatie

{{limited-availability-release-note}}

Leer hoe u uw bedrijf op Real-Time CDP Collaboration kunt inbouwen en verschillende aspecten van uw bedrijf kunt beheren. Deze pagina bevat een overzicht van de stappen die een organisatie moet uitvoeren naar Adobe Real-Time CDP Collaboration, zoals het instellen van de sleutels voor overeenkomsten, de voorkeursidentiteiten en meer opties.

![ pagina van de Opstelling ](/help/assets/setup/manage-organization/my-organization.png){zoomable="yes"}

## Eerste configuratie van organisatie

U moet eerst uw organisatie en organisatorische details instellen. Navigeer naar **[!UICONTROL Setup]** in het linkerspoor, selecteer **+** symbool in de hogere juiste hoek, en selecteer **[!UICONTROL Account]**.

>[!TIP]
>
>Nadat u een initiële account hebt ingesteld om mee te werken, kunt u dezelfde workflow gebruiken om extra accounts in dezelfde organisatie in te stellen.

![ Uitgezochte Rekening om nieuwe organisatie aan Real-Time CDP Collaboration toe te voegen ](/help/assets/setup/manage-organization/add-new-account.png){zoomable="yes"}

De workflow voor het instellen van uw organisatie bestaat uit de volgende twee pagina&#39;s:

* [Details instellen](#set-up-details)
* [ de opstellings gelijke sleutels ](#set-up-match-keys)

>[!IMPORTANT]
>
>Om het even welk *gelijke sleutels* die u op het organisatieniveau selecteert zal dan aan het [ projectniveau ](/help/guide/collaborate/manage-projects.md) in de samenwerking tussen adverteerders en uitgevers trickle. Op het projectniveau, kunt u om het even welke gelijknamensleutels dan verwijderen, maar u bent *niet* in staat om extra degenen toe te voegen die niet op het organisatieniveau in dit scherm werden geselecteerd.

### Details instellen {#set-up-details}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_setup_contact_email"
>title="E-mailadres"
>abstract="Geef een team of op rol gebaseerde e-mail op, bijvoorbeeld `collaboration@yourcompany.com` . Persoonlijke of individuele e-mailadressen mogen niet worden gebruikt."

![ de details en gebruikscasestappen aan opstelling een organisatie ](/help/assets/setup/manage-organization/add-organization-details.png){zoomable="yes"}

1. Voeg een **[!UICONTROL Organization name]** voor uw bedrijf toe.
2. Voeg een **[!UICONTROL Description]** over uw bedrijf toe.
3. Selecteer de **[!UICONTROL Company role]** . U kunt kiezen tussen **[!UICONTROL Advertiser]** en **[!UICONTROL Publisher]** . Lees het [ werkschemadocument van begin tot eind ](/help/guide/end-to-end-workflow.md) om gelijkenissen en lichte verschillen in werkschema tussen de twee organisatorische roltypes te zien.
4. Selecteer de **[!UICONTROL Industry]** voor uw organisatie. Voorbeelden zijn **[!UICONTROL Retail]** , **[!UICONTROL Telecommunications]** of **[!UICONTROL Financial services]** .
5. Selecteer de **[!UICONTROL Region]** voor uw organisatie. In de huidige versie van het product is **[!UICONTROL North America]** de standaardselectie met voorinstellingen.
6. Voeg een **[!UICONTROL Contact email]** toe voor uw organisatie. Dit moet een team of een op rollen gebaseerd e-mailadres zijn. Persoonlijke e-mailadressen mogen niet worden opgegeven.
7. Upload een **[!UICONTROL Logo]** voor uw bedrijf. Op dit moment worden SVG-afbeeldingen ondersteund.
8. Selecteer een afbeelding voor de koptekst van uw bedrijf.

Als u tevreden bent met de selectie, gebruikt u **[!UICONTROL Next]** om door te gaan naar de volgende pagina en de gewenste match keys te selecteren die uw organisatie moet gebruiken.

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

Identieke sleutels, zoals e-mailadressen, apparaat-id&#39;s of klant-id&#39;s, helpen adverteerders en uitgevers samen door nauwkeurige en privacygerichte gegevenssynchronisatie in te schakelen, waardoor doelgerichtere doelgroepen en meetwaarden mogelijk zijn.

![ dia die de beschikbare herkenningstekens voor de eerste versie van Real-Time CDP Collaboration tonen.](/help/assets/setup/manage-organization/available-identifiers.png)

Selecteer de sleutels die u wilt gebruiken wanneer het in overeenstemming brengen van leden van uitgever en adverteerderpubliek. Neem alle sleutels op die uw bedrijf kan gebruiken. Plan voor de toekomst en selecteer de wedstrijdsleutels die u in toekomstige uitgever-adverteerders campagnes zult gebruiken. Als u extra gelijke sleutels voor uw organisatie moet selecteren, kunt u dat in een recentere tijd ook doen, in [ organisatie ](#edit-organization) werkschema uitgeven.

![ de stap van de de toetsenselectie van de Gelijke.](/help/assets/setup/manage-organization/add-organization-match-keys.png){zoomable="yes"}

Selecteer maximaal vijf overeenkomende toetsen die u wilt gebruiken. Later kunt u bij het instellen van verbindingen ongewenste overeenkomende toetsen verwijderen, maar geen nieuwe toetsen toevoegen.

De beschikbare sleutels van gelijke in Real-Time CDP Collaboration kunnen van drie types zijn:

* ID&#39;s van eerstehulppersonen
* Apparaat-id&#39;s van eerste partij
* Partner-id&#39;s

De beschikbare match keys voor de eerste release van Real-Time CDP Collaboration zijn:

* Onderbroken e-mail

<!--

not available in the Limited GA release

* Hashed phone
* IPv4

-->

Als dit gereed is, selecteert u **[!UICONTROL Complete]** om de installatieworkflow van de organisatie te voltooien.

## Organisatie bewerken {#edit-organization}

Nadat u uw organisatie voor het eerst hebt ingesteld, kunt u op elk gewenst moment bepaalde aspecten en details van de organisatie bewerken. Als u uw organisatie wilt bewerken, selecteert u **[!UICONTROL Edit]** in de **[!UICONTROL My organization]** -weergave.

![ uitgezocht geef organisatiecontrole uit.](/help/assets/setup/manage-organization/edit-organization.png){zoomable="yes"}

U kunt nu de organisatienaam, beschrijving, logo en afbeelding van het organisatieprofiel bijwerken.

![ Bewerkbare opties voor organisaties.](/help/assets/setup/manage-organization/editable-options.png){zoomable="yes"}

U kunt ook de overeenkomende sleutels bijwerken die u in eerste instantie hebt geselecteerd bij het instappen van uw organisatie, evenals de minimumdrempel voor identiteiten die overeenkomen met overeenkomende sleutels die zichtbaar en bruikbaar zijn in de overlappingen van het publiek en andere productgebieden. Selecteer **[!UICONTROL Edit]** op het tabblad **[!UICONTROL Match keys]** om extra gewenste overeenkomstsleutels toe te voegen of om identiteitsdrempels bij te werken.

![ geef gelijke sleutels ](/help/assets/setup/manage-organization/edit-match-keys.png){zoomable="yes"} uit

## Volgende stappen

Na vestiging uw organisatie, bent u bereid om [ publiek ](/help/guide/setup/onboard-audiences.md) in Real-Time CDP Collaboration in te voeren.
