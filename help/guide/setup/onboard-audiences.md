---
title: Soorten publiek importeren en beheren
description: Meer informatie over het importeren en beheren van soorten publiek in Adobe Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0a5158fa-73d3-4406-af20-2b6c7be9934e
source-git-commit: fda414120decc0c76712616ff85b83febede53e9
workflow-type: tm+mt
source-wordcount: '2852'
ht-degree: 0%

---

# Soorten publiek importeren en beheren

{{limited-availability-release-note}}

Het publiek is specifieke groepen gebruikers of klanten die op diverse attributen worden gesegmenteerd. Hierdoor kunnen adverteerders en uitgevers samenwerken aan gerichte marketing en persoonlijke ervaringen voor effectievere reclamecampagnes.

Gebruik deze pagina als uw doorverwijzing voor het begrijpen van alle relevante metriek die u kunt bekijken met betrekking tot uw publiek, evenals de workflowstappen om een publiek in Adobe Real-Time CDP Collaboration te importeren.

>[!TIP]
>
>Gebruik de informatie in dit scherm om alle informatie te krijgen u over uw publiek nodig hebt, en [ ontdekt en overlapt de schermen ](/help/guide/collaborate/discover.md) om inzicht te krijgen betreffende welke van uw publiek het best voor verschillende campagneretypen zou werken, wanneer vergeleken met uitgeversinventaris.

>[!BEGINSHADEBOX]

Wat u op deze documentatiepagina zult vinden:

* [Soorten publiek importeren in Real-Time CDP Collaboration](#import-audiences)
* [Het dashboard voor soorten publiek weergeven](#view-audiences-dashboard)
* [Individuele doelgroepen weergeven](#view-individual-audiences)

>[!ENDSHADEBOX]

## Soorten publiek importeren in Real-Time CDP Collaboration {#import-audiences}

>[!IMPORTANT]
>
>Om publiek in te voeren, moet uw gebruiker aan een rol worden toegewezen die twee toestemmingen van het Beheer van het Profiel - de Profielen van de Mening en de Segmenten van de Mening bevat. Voor informatie over het toewijzen van de noodzakelijke toestemmingen, verwijs naar de [ gids van de kijkinvoer ](../permissions/overview.md#audience-importation).

Voordat u het publiek met medewerkers kunt activeren en overlappende berekeningen kunt uitvoeren, moet het publiek naar Real-Time CDP Collaboration worden geïmporteerd. Volg de workflowstappen in de onderstaande sectie om het publiek te importeren.

Van het **[!UICONTROL My audiences]** lusje binnen de **[!UICONTROL Stetup]** werkruimte selecteer toevoegen pictogram (![ voeg pictogram toe.](/help/assets/icons/plus.png)) of de **[!UICONTROL Add]optie** en selecteer dan **Publiek**.

![ Mijn publiek werkruimte met de Add optie en de benadrukte optie van Soorten publiek.](/help/assets/setup/add-manage-audiences/add-audiences.png)

### Gegevensverbinding selecteren {#select-data-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_marketing_actions"
>title="Marketingacties"
>abstract="<p>Gebruik marketingacties om te bepalen welke publieksgegevens uit Experience Platform in Real-Time CDP Collaboration moeten worden geïmporteerd. De </strong> marketing actie van Collaboration van 0} Gegevens steunt C4, C5 en C9 de etiketten van het gegevensgebruik. <strong> De </strong> marketing actie van de Wetenschap van 0} Gegevens steunt het C9 etiket van het gegevensgebruik.<strong></p> <p> <ul><li> Met checkbox <em> toegelaten </em>, wordt om het even welk gegeven dat met de etiketten duidelijk is die hierboven in Experience Platform worden geroepen uitgesloten en wordt <strong> niet </strong> gebracht in Real-Time CDP Collaboration.</li><li> Met checkbox <em> gehandicapt </em>, is er geen beperking op gegevens van Experience Platform die in Real-Time CDP Collaboration kunnen worden ingevoerd.</li></ul></p>"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/overview.html" text="Overzicht van labels voor gegevensgebruik"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/reference.html" text="Verklarende woordenlijst met gegevensgebruikslabels"

>[!IMPORTANT]
>
>Nadat u de eerste gegevensverbinding tot stand hebt gebracht en uw eerste publiek hebt geïmporteerd, kunt u meerdere soorten publiek importeren via de bestaande gegevensverbinding. Wanneer het toevoegen van extra publiek, zult u van de [ uitgezochte publiek ](#select-audience) stap beginnen, aangezien alle in de eerste plaats vereiste informatie van de andere stappen van de bestaande verbinding zal worden ingevoerd.

Een gegevensverbinding is de gegevensbron waaruit u publiek importeert in Real-Time CDP Collaboration. Adobe Experience Platform is momenteel de enige ondersteunde gegevensverbinding.

Alle instellingen, zoals de planning die u configureert voor de gegevensverbinding, worden toegepast op alle publiek dat wordt geïmporteerd via deze gegevensverbinding.

>[!TIP]
>
>Er is een aparte workflow waarin u uw gegevensverbindingen kunt weergeven en bewerken. Voor meer informatie, volg [ het leiden gegevensverbindingen ](/help/guide/setup/manage-data-connection.md) gids.

Selecteer **[!UICONTROL Add a new data connection]** en selecteer **[!UICONTROL Next]** om uw gegevensverbinding toe te voegen.

![ Add publiek werkruimte met Add een nieuwe benadrukte optie van de gegevensverbinding.](/help/assets/setup/add-manage-audiences/add-data-connection.png)

#### Gegevensbron selecteren

Vervolgens kiest u de bron voor de gegevensverbinding. De beschikbare bronnen zijn onder meer:

* **Adobe Experience Platform**: Selecteer deze optie om uw publiek van Adobe Experience Platform Real-Time CDP te brengen.
* **Csv- Dossier** (Toekomstige versie): Upload een Csv- dossier dat uw publieksgegevens voor snelle en ongecompliceerde gegevensopname bevat.
* **Amazon Web Services** (Toekomstige versie): Verbind met uw opslag van Amazon S3 om publieksgegevens van uw S3 emmers direct in te voeren.
* **Snowflake** (Toekomstige versie): Gebruik uw gegevenspakhuis van Snowflake om in publieksgegevens foutloos te trekken.

Selecteer de gegevensbron en selecteer vervolgens **[!UICONTROL Next]** .

![ Add publiek werkruimte met de benadrukte optie van Adobe Experience Platform.](/help/assets/setup/add-manage-audiences/select-data-connection-source.png)

#### Sandbox selecteren

Nadat u de gegevensbron hebt geselecteerd, moet u de sandbox selecteren die het publiek bevat dat u wilt importeren. Selecteer de sandbox in de lijst met beschikbare sandboxen en selecteer vervolgens **[!UICONTROL Next]**

![ Add publiek werkruimte met geselecteerde zandbak.](/help/assets/setup/add-manage-audiences/select-sandbox.png)

#### Beleid inzake governance en handhavingsmaatregelen {#governance-policy-and-enforcement-actions}

Vervolgens moet u ervoor zorgen dat de juiste marketingacties zijn ingesteld voor de geïmporteerde gegevens. U moet ook toestemming geven voor het gebruik van uit Real-Time CDP geïmporteerde gegevens voor gegevenssamenwerking.

Gebruik marketingacties om te bepalen welke publieksgegevens uit Experience Platform in Real-Time CDP Collaboration moeten worden geïmporteerd. De **marketing actie van Collaboration van 0} Gegevens steunt C4, C5 en C9 de etiketten van het gegevensgebruik.** De **marketing actie van de Wetenschap van 0} Gegevens steunt het C9 etiket van het gegevensgebruik.**

Lees meer over [ C4, C5, en C9 de etiketten van het gegevensgebruik ](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference#contract){target="_blank"}.

* Met checkbox *toegelaten*, wordt om het even welk gegeven dat met de etiketten duidelijk is die hierboven in Experience Platform worden geroepen uitgesloten en wordt *niet* gebracht in Real-Time CDP Collaboration.
* Met checkbox *gehandicapt*, is er geen beperking op gegevens van Experience Platform die in Real-Time CDP Collaboration kunnen worden ingevoerd.

Meer informatie over labels voor gegevensgebruik vindt u in de documentatie van Experience Platform:

* [ overzicht van de gebruiksetiketten van Gegevens ](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/overview){target="_blank"}
* [ de etiketten van het gebruiksgebruik van Gegevens verklarende woordenlijst ](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference){target="_blank"}

Bovendien zult u uw samenstellingsregels willen selecteren om op gegevens toe te passen die in Real-Time CDP Collaboration worden ingevoerd.

![ Add de werkruimte van het publiek bij de sectie van het beleid van het Bestuur en van de handhavingsacties.](/help/assets/setup/add-manage-audiences/data-collaboration-consent.png)

Nadat u de marketingacties en de regels voor toestemming hebt geselecteerd, selecteert u **[!UICONTROL Next]** om door te gaan naar de volgende stap. Er verschijnt een bevestigingsvenster waarin u wordt gevraagd de voorwaarden te accepteren. Schakel het selectievakje in en selecteer vervolgens **[!UICONTROL OK]** om te bevestigen.

![ het beleid van het Bestuur en de dialoog van de handhavingsacties met checkbox en O.K. benadrukte optie.](/help/assets/setup/add-manage-audiences/data-collaboration-consent-confirmation.png)

### Geef details

Geef vervolgens een naam en een beschrijving voor de gegevensverbinding op. Deze informatie zal u helpen de gegevensverbinding later identificeren.

![ Add publiek werkruimte met de optie om een naam en een beschrijving te verstrekken.](/help/assets/setup/add-manage-audiences/data-connection-details.png)

### Toewijzingsvelden {#map-fields}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_source_fields"
>title="Source-velden"
>abstract="Source-velden zijn naamruimten en kenmerken van uw bestaande Real-Time CDP-implementatie. U kunt deze toewijzen aan doelvelden die zijn gedefinieerd in Real-Time CDP Collaboration."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_target_fields"
>title="Doelvelden"
>abstract="Gehashte e-mails zijn momenteel de enige ondersteunde overeenkomende sleutels."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_apply_transformation"
>title="Transformatie toepassen"
>abstract="Wanneer het invoeren van *niet-gehakt* gebieden van uw bron, gebruik deze optie om Real-Time CDP Collaboration te hebben het hakken toepassen en de gewone gebieden in gehakt gebieden omzetten."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_identity_namespaces"
>title="Identiteitsnaamruimten"
>abstract="Selecteer een naamruimte voor identiteit in de standaard- en aangepaste naamruimten die beschikbaar zijn in uw Experience Platform-organisatie."
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/identity/features/namespaces.html#standard" text="Standaard- en naamruimten in Experience Platform"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_profile_attributes"
>title="Profielkenmerken"
>abstract="Selecteer kenmerken in het Unieschema voor de klasse Profile in Experience Platform. In deze weergave worden de kenmerken weergegeven die aanwezig zijn in het Unieschema en die behoren tot de klasse Individueel profiel XDM."
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/profile/union-schemas/union-schema.html" text="Unieschema in Experience Platform"

Vervolgens selecteert u bronvelden die u wilt toewijzen aan doelvelden in Real-Time CDP Collaboration.

![ Add publiek werkruimte met de optie om brongebieden aan doelgebieden in kaart te brengen.](/help/assets/setup/add-manage-audiences/add-map-fields.png)

>[!TIP]
>
>U kunt meerdere bronvelden toewijzen aan hetzelfde doelveld. Als u bijvoorbeeld e-mailadressen hebt in twee verschillende velden in Experience Platform, kunt u beide aan het doelveld van **[!UICONTROL Hashed email]** toewijzen als twee aparte rijen.

>[!BEGINSHADEBOX]

**[!UICONTROL Source fields]** zijn naamruimten en kenmerken van uw bestaande implementatie van Real-Time CDP. Zo bestaan de identiteiten in de bron waaruit u gegevens importeert. Source-velden worden toegewezen aan de doelvelden die zijn gedefinieerd in Real-Time CDP Collaboration.

**[!UICONTROL Target fields]** geeft aan hoe naar de identiteiten wordt verwezen in Real-Time CDP Collaboration. Gehashte e-mails zijn momenteel de enige ondersteunde overeenkomende sleutels.

Gebruik de **[!UICONTROL Apply transformation]** optie wanneer u *niet-gehakt* gebieden van uw bron invoert. In dit geval past Real-Time CDP Collaboration de hash toe en transformeert het de velden. Het hash-algoritme dat door Adobe wordt gebruikt, is SHA256.

>[!ENDSHADEBOX]

Selecteer het lege bronveld naast het doelveld. Het dialoogvenster **[!UICONTROL Select source field]** wordt weergegeven. Selecteer tussen de opties **[!UICONTROL Identity namespaces]** en **[!UICONTROL Profile attributes]** om het gewenste bronveld te zoeken en selecteer vervolgens het bronveld in de lijst. Gebruik hiervoor de zoekoptie om het gewenste veld te zoeken.

![ de Uitgezochte dialoog van het brongebied met de e-mailgetoonde opties.](/help/assets/setup/add-manage-audiences/select-source-field.png)

Als u meerdere e-mailvelden wilt verwerken, wijst u het bronveld voor niet-gehashte e-mail toe met **[!UICONTROL Apply transformation]** .

![ Add de werkruimte van het publiek met de e-mailbrongebieden die aan het doelgebied worden in kaart gebracht, met Toepassen transformatie die voor één wordt van een knevel voorzien.](/help/assets/setup/add-manage-audiences/apply-transformation.png)

Voeg desgewenst toewijzingsparen toe en selecteer vervolgens **[!UICONTROL Next]** .

### Schema {#schedule}

Stel vervolgens in wanneer het publiek moet worden ingevuld. Het publiek wordt volgens dit schema vernieuwd.

![ Add publiekswerkruimte met de het plannen getoonde opties.](/help/assets/setup/add-manage-audiences/audience-scheduling.png)

>[!IMPORTANT]
>
>Het aanpassen van de frequentie van publieksupdates zal helpen de [ de kredietactiviteit van het Beheer van de Publiek beheren ](/help/guide/setup/my-activity.md#types-of-activities), die per publiek wordt berekend verfrist zich. Het selecteren van een hogere frequentie kan invloed hebben op de versheid van de gegevens beschikbaar voor publiek ontdekt rapporten en publieksactivering.

Selecteer in het vervolgkeuzemenu **[!UICONTROL Frequency]** de frequentie waarmee het publiek zich moet vernieuwen.

![ Add publiek dat werkruimte met open drop-down van de Frequentie plant.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png)

Selecteer vervolgens **[!UICONTROL Date range]** . De begindatum is de datum waarop het publiek begint met het vullen met profielen en de einddatum is wanneer het publiek stopt met vernieuwen.

![ Add publiek dat werkruimte met de getoonde de waaieroptie van de Datum plant.](/help/assets/setup/add-manage-audiences/audience-scheduling-date-range.png)

>[!IMPORTANT]
>
>Na de einddatum in het datumbereik wordt het vernieuwen stopgezet van alle soorten publiek die worden geïmporteerd uit deze gegevensverbinding. Om de verbinding te vernieuwen, ga [ gegevensverbinding beheren ](/help/guide/setup/manage-data-connection.md), en plaats een nieuwe einddatum.

### Soorten publiek selecteren {#select-audience}

Nadat u de publieksbron hebt geselecteerd, kiest u een specifiek publiek dat u wilt opnemen. Gebruik de opties voor zoeken en filteren om het relevante publiek in de gegevensbron te zoeken. Selecteer het gewenste publiek en selecteer vervolgens **[!UICONTROL Next]** .

![ Add publiek werkruimte met een lijst van beschikbaar publiek.](/help/assets/setup/add-manage-audiences/select-audience.png)

### Controleren

Bekijk alle configuraties en instellingen voordat u de publiekstoevoeging voltooit. Controleer of alle gegevens correct zijn en selecteer **[!UICONTROL Complete]** om de gegevensverbinding te voltooien.

![ Add publiek werkruimte met alle uitgezochte getoonde configuraties.](/help/assets/setup/add-manage-audiences/review-connection.png)

## Het dashboard voor soorten publiek weergeven {#view-audiences-dashboard}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_missing_identities"
>title="Ontbrekende identiteiten"
>abstract="Het aantal identiteiten zal beschikbaar zijn nadat de volgende gegevensverbinding na het gevormde programma verfrist zich. De eerste vernieuwing vindt gewoonlijk plaats binnen 24 uur nadat de gegevensverbinding is ingesteld. De voortdurende verfrissingen zullen het gevormde programma volgen. "

Nadat u een publiek hebt geïmporteerd naar Real-Time CDP Collaboration, worden in de werkruimte **[!UICONTROL My audiences]** alle soorten publiek weergegeven die momenteel door uw organisatie in Real-Time CDP Collaboration zijn geïmporteerd.


Elk publiek bevat een overzicht van de volgende informatie:

| Item | Beschrijving |
|----------|---------|
| **[!UICONTROL Identities]** | Geeft het aantal identiteiten aan dat in dit publiek aanwezig is. Als hetzelfde profiel twee of meer identiteiten heeft en deze identiteiten als overeenkomende sleutels in het project worden gebruikt, wordt het profiel twee keer weergegeven in de telling. |
| **[!UICONTROL Status]** | Geeft aan of het publiek actief is en kan worden gebruikt in projecten. Een **[!UICONTROL Pending]** -status geeft aan dat het publiek onlangs is geïmporteerd en dat publieksleden nog niet zijn gevuld. Het geïmporteerde publiek krijgt profielen na de eerste vernieuwing, die zich gewoonlijk binnen 24 uur na het instellen van de gegevensverbinding voordoet. |
| **[!UICONTROL Source]** | Geeft de bron aan waaruit het publiek is geïmporteerd. In de huidige release van Real-Time CDP Collaboration is Adobe Experience Platform de enige ondersteunde bron. |
| **[!UICONTROL Data connection]** | De gegevensverbinding waarvan het publiek afkomstig is. U kunt de naam selecteren om de gegevensverbinding te bekijken. |
| **[!UICONTROL Connection access]** | Bepaalt of het publiek privé of openbaar is. Openbare doelgroepen zijn te vinden in overlappende rapporten en kunnen binnen een project worden geactiveerd. |
| **[!UICONTROL Created]** | Geeft aan wanneer het publiek naar Real-Time CDP Collaboration is geïmporteerd. |
| **[!UICONTROL Last updated]** | Geeft de laatste datum en tijd aan waarop een aspect van het publiek is bijgewerkt. |

![ de Mijn publiekswerkruimte die alle ingevoerde publiek tonen.](/help/assets/setup/add-manage-audiences/audiences-workspace.png)

Om snelle acties op een publiek uit te voeren, selecteer de ellips **...** naast de publieksnaam. De volgende opties zijn beschikbaar:

* Met **[!UICONTROL Edit categories]** kunt u verschillende categorietags toevoegen aan het publiek. Voor meer informatie, verwijs naar de [ categorieën ](#categories) hieronder sectie.
* **[!UICONTROL Delete]** verwijdert het publiek uit de gegevensverbinding.

![ Mijn publiek werkruimte met het open weglatingsmenu en uitgeeft categorieën en benadrukt de opties van de Schrapping.](/help/assets/setup/add-manage-audiences/audiences-ellipsis-menu.png)

## Individuele doelgroepen weergeven {#view-individual-audiences}

Als u meer informatie wilt weergeven en configuraties voor een afzonderlijk publiek wilt bewerken, selecteert u het publiek in de werkruimte van **[!UICONTROL My audiences]** . De publiekswerkruimte bevat gedetailleerde informatie over het geselecteerde publiek, zoals de details, identiteiten, categorieën, toegang tot de verbinding en instellingen voor de zichtbaarheid van metagegevens.

### Details publiek

De volgende informatie wordt voor elk individueel publiek getoond:

| Item | Beschrijving |
|----------|---------|
| **[!UICONTROL Status]** | Geeft aan of het publiek actief is en kan worden gebruikt in projecten. |
| **[!UICONTROL Source]** | Geeft de bron aan waaruit het publiek is geïmporteerd. In de huidige release van Real-Time CDP Collaboration is Adobe Experience Platform de enige ondersteunde bron. |
| **[!UICONTROL Data connection]** | De gegevensverbinding waarvan het publiek afkomstig is. |
| **[!UICONTROL Last updated]** | Geeft de laatste datum en tijd aan waarop het publiek is bijgewerkt. |
| **[!UICONTROL Last updated by]** | Geeft de gebruiker aan die het publiek voor het laatst heeft bijgewerkt. |
| **[!UICONTROL Created]** | Geeft aan wanneer het publiek naar Real-Time CDP Collaboration is geïmporteerd. |
| **[!UICONTROL Created by]** | Geeft de gebruiker aan die het publiek in Real-Time CDP Collaboration heeft geïmporteerd. |

![ de werkruimte van een individueel publiek.](/help/assets/setup/add-manage-audiences/audience-details.png)

Daarnaast zijn de volgende besturingselementen beschikbaar in de publiekswerkruimte:

* **[!UICONTROL Delete]**: verwijder het publiek van uw gegevensverbinding.
* **[!UICONTROL Edit]**: geef de naam of beschrijving van het publiek uit.

![ de werkruimte van een individueel publiek met Edit en benadrukte optie van de Schrapping.](/help/assets/setup/add-manage-audiences/audience-details-edit-delete.png)

Vervolgens kunt u de volgende secties bijwerken in de werkruimte van het publiek:

* [Identiteiten](#identities)
* [Categorieën](#categories)
* [Toegang tot verbinding](#connection-access)
* [Zichtbaarheid metagegevens](#metadata-visibility)

### Identiteiten {#identities}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_identities"
>title="Identiteiten"
>abstract="Een uitsplitsingsweergave van de identiteiten waaruit dit publiek bestaat en een totaal aantal profielen met de respectievelijke identiteiten."

De sectie **[!UICONTROL Identities]** geeft het aantal profielen aan dat in het publiek aanwezig is met een van de identiteiten die u hebt geselecteerd tijdens het importeren van het publiek. De sectie bevat ook een identiteitsspecificatie zodat u kunt zien welke identiteiten het grootste deel van de publiekspopulatie uitmaken.

![ de sectie van Identiteiten van de werkruimte van een individueel publiek.](/help/assets/setup/add-manage-audiences/audience-details-identities.png)

### Categorieën {#categories}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_categories"
>title="Categorieën"
>abstract="Geef uw publiek tags voor eenvoudige organisatie, filteren en ophalen. U kunt een publiek met meerdere categorieën tags toewijzen en vervolgens deze categorietags gebruiken om het gewenste publiek in andere gebieden van het product te filteren."

Voor eenvoudige publieksorganisatie, het filtreren, en het terugwinnen, kunt u uw publiek etiketteren. U kunt een publiek met veelvoudige categorieën etiketteren en dan kunt u deze categorietags gebruiken om uw gewenste publiek in [ te filtreren ontdekken ](/help/guide/collaborate/discover.md) productgebied, wanneer het runnen van publiek overlappende rapporten.

Als u categorieën wilt toevoegen, selecteert u de optie **[!UICONTROL Edit]** in de sectie **[!UICONTROL Categories]** .

![ de sectie van Categorieën van de werkruimte van een individueel publiek.](/help/assets/setup/add-manage-audiences/audience-details-categories.png)

Het dialoogvenster **[!UICONTROL Categories]** wordt weergegeven, zodat u de categorieën kunt selecteren die u aan het publiek wilt toevoegen. Als u een afzonderlijke categorie wilt selecteren, schakelt u het selectievakje naast de categorienaam in.

![ de dialoog van Categorieën met de beschikbare getoonde categorieën.](/help/assets/setup/add-manage-audiences/audience-details-categories-select.png)

### Toegang tot verbinding {#connection-access}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_connection_access"
>title="Toegang tot verbinding"
>abstract="<p>De soorten publiek kunnen van drie types zijn: publiek, privé, en douane.</p><p> Hun beschikbaarheid voor gebruik in projecten met medewerkers verschilt gebaseerd op het plaatsen van de verbindingstoegang. U kunt de verbindingstoegang altijd wijzigen van privé in openbaar, maar u kunt die instelling niet meer wijzigen als een publiek wordt geactiveerd met deelnemers.</p>"

De beschikbaarheid van een publiek voor gebruik in projecten met medewerkers verschilt afhankelijk van de instelling voor de toegang tot de verbinding. In de sectie **[!UICONTROL Connection access]** kunt u aangeven of het publiek privé moet zijn of bruikbaar en te ontdekken moet zijn in verbindingen.

Als u de toegang tot de verbinding van de doelgroep wilt bijwerken, selecteert u de optie **[!UICONTROL Edit]** in de **[!UICONTROL Connection access]** -sectie.

![ de de toegangssectie van de Verbinding van de werkruimte van een individueel publiek.](/help/assets/setup/add-manage-audiences/audience-details-connection-access.png)

Het dialoogvenster **[!UICONTROL Connection access]** wordt weergegeven met drie beschikbare toegangsopties voor de verbinding:

* **[!UICONTROL Private audience]**. Dit publiek is *niet* beschikbaar voor gebruik in overlappende rapporten of voor activering in verbindingen met om het even welke medewerkers. Terwijl het publiek niet voor medewerkers beschikbaar is om te bekijken of te gebruiken, draagt de bevolking van het publiek nog aan de totale bevolking in de **[!UICONTROL All audiences]** mening in de [ vergelijkingspubliekssectie ](/help/guide/collaborate/discover.md#compare-audiences) bij. Wijzig de instelling in Openbaar of Aangepast als u het publiek wilt gebruiken in verbindingen met medewerkers.
* **[!UICONTROL Public audience]**. Deze doelgroepen zijn beschikbaar voor gebruik in overlappende rapporten en voor activering in verbindingen met deelnemers.
* **[!UICONTROL Custom audience]**. Deze soorten publiek zijn alleen beschikbaar voor gebruik in overlappende rapporten en voor activering in opgegeven verbindingen. Terwijl het publiek niet voor medewerkers beschikbaar is om te bekijken of te gebruiken, draagt de bevolking van het publiek nog aan de totale bevolking in de **[!UICONTROL All audiences]** mening in de [ vergelijkingspubliekssectie ](/help/guide/collaborate/discover.md#compare-audiences) bij.

Selecteer de gewenste toegangsoptie voor de verbinding en selecteer vervolgens **[!UICONTROL Save]** om de wijzigingen toe te passen.

![ het de toegangsdialoog van de Verbinding met de beschikbare getoonde opties.](/help/assets/setup/add-manage-audiences/audience-details-connection-access-dialog.png)

>[!IMPORTANT]
>
>Ongeacht de toegangsstatus (openbaar, privé, of douane), draagt de bevolking van om het even welk publiek aan de **[!UICONTROL All audiences]** bevolking in de **[!UICONTROL Compare audiences]** sectie binnen een project bij.<br>

De beschikbaarheid van het publiek voor gebruik in projecten met medewerkers verschilt gebaseerd op het plaatsen van de verbindingstoegang. U kunt de toegang tot de verbinding altijd wijzigen van privé in openbaar, maar u kunt die instelling niet meer wijzigen als een publiek wordt geactiveerd.

### Zichtbaarheid metagegevens {#metadata-visibility}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_metadata_visibility"
>title="Zichtbaarheid metagegevens"
>abstract="<p>Geeft aan welke metagegevens van het publiek zichtbaar zijn voor andere organisaties voordat ze verbinding maken met uw organisatie. </p> <p> **de telling van de Identiteit** controleert of uw partner identiteitscijfers voor uw publiek kan bekijken wanneer het bekijken van overlappende rapporten in de ontdekking tabel. **het publiek overlapt %** controleert of de medewerkers overlappende percentages tussen hun publiek en van u kunnen ontdekken."

>[!NOTE]
>
>Als voor uw medewerker alle soorten publiek zijn ingesteld op Private, is de sectie **[!UICONTROL Relevant audiences]** van een project in de **[!UICONTROL Discover]** -werkruimte leeg. Voor meer informatie, lees [ ontdekt ](/help/guide/collaborate/discover.md#relevant-audiences). hulplijn.

De zichtbaarheid van metagegevens geeft de zichtbaarheid van de metagegevens van een publiek aan bij andere organisaties voordat deze verbinding maken met uw organisatie of binnen verschillende projectweergaven. Als u de zichtbaarheid van de metagegevens van de doelgroep wilt bijwerken, selecteert u de optie **[!UICONTROL Edit]** in de **[!UICONTROL Metadata visibility]** -sectie.

![ de de zichtbaarheidssectie van Meta-gegevens van de werkruimte van een individueel publiek.](/help/assets/setup/add-manage-audiences/audience-details-metadata.png)

Het dialoogvenster **[!UICONTROL Metadata visibility]** wordt weergegeven, zodat u de zichtbaarheidsinstellingen voor het publiek kunt configureren. Er zijn twee montages van de meta-gegevenszichtbaarheid die u voor elk publiek kunt vormen:

**[!UICONTROL Show identity count]**: Dit het plaatsen controleert of uw medewerker identiteitstellingen voor uw publiek kan bekijken wanneer [ het bekijken overlappende rapporten in het ontdekkingslusje ](/help/guide/collaborate/discover.md#discover-overlaps) binnen een project.

**[!UICONTROL Show audience overlap %]**: Wanneer geplaatst aan waar, kunnen de medewerkers [ overlappende percentages ](/help/guide/collaborate/discover.md#compare-audiences) tussen hun publiek en uw publiek ontdekken.

![ het de zichtbaarheidsdialoog van Meta-gegevens met de beschikbare getoonde opties.](/help/assets/setup/add-manage-audiences/audience-details-metadata-dialog.png)

## Volgende stappen

Na het invoeren van publiek, is het tijd om uitgevers te ontdekken om [ ](/help/guide/connect/establishing-connections.md) met te verbinden en te beginnen aan projecten samen te werken.
