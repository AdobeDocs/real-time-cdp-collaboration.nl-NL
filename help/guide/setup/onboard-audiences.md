---
title: Source en publiek beheren
description: Leer hoe u het publiek in Adobe Real-Time CDP Collaboration kunt aanschaffen en beheren
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0a5158fa-73d3-4406-af20-2b6c7be9934e
source-git-commit: f14b5d2f49f20f229c4f474c31e22c008827a09b
workflow-type: tm+mt
source-wordcount: '3357'
ht-degree: 0%

---

# Source en publiek beheren

{{limited-availability-release-note}}

Het publiek is specifieke groepen gebruikers of klanten die op diverse attributen worden gesegmenteerd. Hierdoor kunnen deelnemers samenwerken aan gerichte marketing en persoonlijke ervaringen voor effectievere reclamecampagnes. In deze handleiding wordt uitgelegd hoe u het publiek naar Real-Time CDP Collaboration kunt sturen, hoe u het dashboard voor het publiek kunt bekijken en hoe u het individuele publiek kunt beheren.

## Source-publiek naar Collaboration {#source-audiences}

>[!IMPORTANT]
>
>Voor het bronpubliek moet uw gebruiker worden toegewezen aan een rol die twee bevoegdheden voor profielbeheer bevat - **[!UICONTROL View Profiles]** en **[!UICONTROL View Segments]** . Voor informatie over het toewijzen van de noodzakelijke toestemmingen, verwijs naar de [&#x200B; publiek die &#x200B;](../permissions/overview.md#audience-sourcing) gids in toestemmingen terugwinnen.

Voordat u het publiek met medewerkers kunt activeren en overlappende berekeningen kunt uitvoeren, moet het publiek naar Collaboration zijn gedownload. Volg de workflowstappen in de onderstaande sectie om het publiek te bereiken.

Van het **[!UICONTROL My audiences]** lusje binnen de **[!UICONTROL Setup]** werkruimte, selecteer het add pictogram (![&#x200B; voeg pictogram toe.](/help/assets/icons/plus.png) ) en selecteer vervolgens **[!UICONTROL Audience]** . Als dit uw eerste publiek is, kunt u de **[!UICONTROL Add]optie** ook selecteren.

![&#x200B; Mijn publiek werkruimte met de Add optie en de benadrukte optie van Soorten publiek.](/help/assets/setup/add-manage-audiences/add-audiences.png){zoomable="yes"}

### Gegevensverbinding selecteren {#select-data-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_marketing_actions"
>title="Marketingacties"
>abstract="<p>Gebruik marketingacties om te bepalen welke publieksgegevens uit Experience Platform in Real-Time CDP Collaboration moeten worden geïmporteerd. De <strong> marketing actie van Collaboration van 0&rbrace; Gegevens steunt C4, C5 en C9 de etiketten van het gegevensgebruik. </strong> De <strong> marketing actie van de Wetenschap van 0&rbrace; Gegevens steunt het C9 etiket van het gegevensgebruik.</strong></p> <p> <ul><li> Met checkbox <em> toegelaten </em>, wordt om het even welk gegeven dat met de etiketten duidelijk is die hierboven in Experience Platform worden geroepen uitgesloten en wordt <strong> niet </strong> gebracht in Real-Time CDP Collaboration.</li><li> Met checkbox <em> gehandicapt </em>, is er geen beperking op gegevens van Experience Platform die in Real-Time CDP Collaboration kunnen worden betreden.</li></ul></p>"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/overview.html" text="Overzicht van labels voor gegevensgebruik"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/reference.html" text="Verklarende woordenlijst met gegevensgebruikslabels"

>[!IMPORTANT]
>
>Nadat u de eerste gegevensverbinding tot stand hebt gebracht en uw eerste publiek hebt opgehaald, kunt u meerdere soorten publiek vervolgens betrekken via de bestaande gegevensverbinding. Wanneer het toevoegen van extra publiek, zult u van de [&#x200B; uitgezochte publieksstap &#x200B;](#select-audiences) beginnen, aangezien de gegevensverbinding reeds is gevestigd.

Een gegevensverbinding is de bron van gegevens van waar u publiek aantrekt. Adobe Experience Platform is momenteel de enige ondersteunde gegevensverbinding.

Alle instellingen die u configureert voor de gegevensverbinding worden toegepast op alle soorten publiek die afkomstig zijn van deze gegevensverbinding.

>[!TIP]
>
>Er is een aparte workflow waarin u uw gegevensverbindingen kunt weergeven en bewerken. Voor meer informatie, volg [&#x200B; het leiden gegevensverbindingen &#x200B;](/help/guide/setup/manage-data-connection.md) gids.

Selecteer **[!UICONTROL Add a new data connection]** en selecteer **[!UICONTROL Next]** om uw gegevensverbinding toe te voegen.

![&#x200B; Add publiek werkruimte met Add een nieuwe benadrukte optie van de gegevensverbinding.](/help/assets/setup/add-manage-audiences/add-data-connection.png){zoomable="yes"}

#### Gegevensbron selecteren

Vervolgens kiest u de bron voor de gegevensverbinding. De beschikbare bronnen zijn onder meer:

* **Adobe Experience Platform**: Selecteer deze optie om uw publiek van Adobe Experience Platform te brengen.
* **Csv- Dossier** (Toekomstige versie): Upload een Csv- dossier dat uw publieksgegevens voor snelle en ongecompliceerde gegevensopname bevat.
* **Amazon Web Services**: Verbind met uw opslag van Amazon S3 aan bron publieksgegevens direct van uw S3 emmers. Zie [&#x200B; AWS S3 voor publiek vormen die &#x200B;](./configure-aws-s3-audience-sourcing.md) gids voor geleidelijke instructies aantrekken.
* **Snowflake** (Toekomstige versie): Gebruik uw gegevenspakhuis van Snowflake om in publieksgegevens foutloos te trekken.
* **Google Cloud Platform** (Toekomstige versie): verbind met uw Opslag van de Wolk van Google aan bron publieksgegevens direct van uw emmers GCS.

Selecteer de gegevensbron en selecteer vervolgens **[!UICONTROL Next]** .

![&#x200B; Add publiek werkruimte met de benadrukte optie van Adobe Experience Platform.](/help/assets/setup/add-manage-audiences/select-data-connection-source.png){zoomable="yes"}

#### Sandbox selecteren

Nadat u de gegevensbron hebt geselecteerd, moet u de sandbox selecteren die het publiek bevat dat u voor Collaboration wilt gebruiken. Selecteer de sandbox in de lijst met beschikbare sandboxen en selecteer vervolgens **[!UICONTROL Next]**

![&#x200B; Add publiek werkruimte met geselecteerde zandbak.](/help/assets/setup/add-manage-audiences/select-sandbox.png){zoomable="yes"}

#### Beleid inzake governance en handhavingsmaatregelen {#governance-policy-and-enforcement-actions}

Vervolgens moet u ervoor zorgen dat de juiste marketingacties zijn ingesteld voor de brongegevens. U moet ook toestemming geven voor het gebruik van gegevens van Experience Platform voor gegevenssamenwerking.

Gebruik marketingacties om te bepalen welke publieksgegevens vanuit Experience Platform naar Collaboration moeten worden overgebracht. De marketingactie **[!UICONTROL Data Collaboration]** ondersteunt de labels voor gegevensgebruik in C4, C5 en C9. De marketingactie **[!UICONTROL Data Science]** ondersteunt het label voor gegevensgebruik C9.

Lees meer over [&#x200B; C4, C5, en C9 de etiketten van het gegevensgebruik &#x200B;](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference#contract){target="_blank"}.

* Wanneer checkbox **&#x200B;**&#x200B;**&#x200B; wordt toegelaten, wordt om het even welke gegevens die in Experience Platform worden geëtiketteerd zoals hierboven beschreven uitgesloten en &#x200B;** niet** gebracht in Collaboration.
* Met checkbox ***gehandicapt***, is er geen beperking op gegevens die uit Experience Platform worden voortgebracht.

Meer informatie over labels voor gegevensgebruik vindt u in de documentatie van Experience Platform:

* [&#x200B; overzicht van de gebruiksetiketten van Gegevens &#x200B;](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/overview){target="_blank"}
* [&#x200B; de etiketten van het gebruiksgebruik van Gegevens verklarende woordenlijst &#x200B;](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference){target="_blank"}

Daarnaast wilt u uw regels voor toestemming selecteren die u wilt toepassen op gegevens die worden gedownload naar Collaboration.

![&#x200B; Add de werkruimte van het publiek bij de sectie van het beleid van het Bestuur en van de handhavingsacties.](/help/assets/setup/add-manage-audiences/data-collaboration-consent.png){zoomable="yes"}

Nadat u de marketingacties en de regels voor toestemming hebt geselecteerd, selecteert u **[!UICONTROL Next]** om door te gaan naar de volgende stap. Er verschijnt een bevestigingsvenster waarin u wordt gevraagd de voorwaarden te accepteren. Schakel het selectievakje in en selecteer vervolgens **[!UICONTROL OK]** om te bevestigen.

![&#x200B; het beleid van het Bestuur en de dialoog van de handhavingsacties met checkbox en O.K. benadrukte optie.](/help/assets/setup/add-manage-audiences/data-collaboration-consent-confirmation.png){zoomable="yes"}

### Geef details

Geef vervolgens een naam en een beschrijving voor de gegevensverbinding op. Deze informatie zal u helpen de gegevensverbinding later identificeren.

![&#x200B; Add publiek werkruimte met de optie om een naam en een beschrijving te verstrekken.](/help/assets/setup/add-manage-audiences/data-connection-details.png){zoomable="yes"}

### Toewijzingsvelden {#map-fields}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_source_fields"
>title="Source-velden"
>abstract="Source-velden zijn naamruimten en kenmerken van uw implementatie van Experience Platform. U kunt deze toewijzen aan doelvelden die zijn gedefinieerd in Collaboration."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_target_fields"
>title="Doelvelden"
>abstract="Doelvelden zijn de sleutels die worden gekozen tijdens het instellen van de account. Standaard zijn alle gekozen sleutels beschikbaar."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_apply_transformation"
>title="Transformatie toepassen"
>abstract="Wanneer het betrekken van *niet-gehakt* gebieden, gebruik deze optie om Collaboration te hebben het hakken toepassen en de gewone gebieden in gehakte gebieden omzetten."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_identity_namespaces"
>title="Identiteitsnaamruimten"
>abstract="Selecteer een naamruimte voor identiteit in de standaard- en aangepaste naamruimten die beschikbaar zijn in uw Experience Platform-organisatie."
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/identity/features/namespaces.html#standard" text="Standaard- en naamruimten in Experience Platform"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_profile_attributes"
>title="Profielkenmerken"
>abstract="Selecteer kenmerken in het samenvoegingsschema voor de klasse Profile in Experience Platform. In deze weergave worden de kenmerken weergegeven die aanwezig zijn in het samenvoegingsschema en die behoren tot de klasse Individueel profiel XDM."
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/profile/union-schemas/union-schema.html" text="Unieschema in Experience Platform"

Vervolgens selecteert u bronvelden die u wilt toewijzen aan doelvelden in Collaboration. De beschikbare doelvelden worden gebaseerd op de overeenkomende toetsen die u hebt geselecteerd tijdens het instellen van de account.

>[!IMPORTANT]
>
>U kunt momenteel geen gegevensverbindingen bewerken om nieuwe kaartvelden op te nemen. Als u nieuwe sleutels van gelijke aan uw rekening toevoegt nadat uw gegevensverbinding is gecreeerd, zult u een nieuwe gegevensverbinding moeten tot stand brengen om aan hen in kaart te brengen.

![&#x200B; Add publiek werkruimte met de optie om brongebieden aan doelgebieden in kaart te brengen.](/help/assets/setup/add-manage-audiences/add-map-fields.png){zoomable="yes"}

>[!TIP]
>
>U kunt meerdere bronvelden toewijzen aan hetzelfde doelveld. Als u bijvoorbeeld e-mailadressen hebt in twee verschillende velden in Experience Platform, kunt u elk van deze adressen als twee aparte rijen toewijzen aan het doelveld van **[!UICONTROL Hashed email]** . Gebruik de optie **[!UICONTROL Add field]** om extra toewijzingsrijen toe te voegen.

>[!BEGINSHADEBOX]

**[!UICONTROL Source fields]** zijn naamruimten en kenmerken van Experience Platform. Deze omvatten zowel standaard [&#x200B; als &#x200B;](https://experienceleague.adobe.com/docs/experience-platform/identity/features/namespaces.html#standard){target="_blank"} douane [&#x200B; identiteitsnaamruimten. &#x200B;](https://experienceleague.adobe.com/docs/experience-platform/identity/features/namespaces.html#create-namespaces){target="_blank"} Zij omvatten ook profielattributen die in het [&#x200B; verenigingsschema &#x200B;](https://experienceleague.adobe.com/docs/experience-platform/profile/union-schemas/union-schema.html){target="_blank"} aanwezig zijn en tot de individuele klasse van het Profiel XDM behoren.

Source-velden worden toegewezen aan de doelvelden die zijn gedefinieerd in Collaboration.

**[!UICONTROL Target fields]** geeft aan hoe naar de identiteiten wordt verwezen in Collaboration. Doelvelden zijn de sleutels die worden gekozen tijdens het instellen van de account. Standaard zijn alle gekozen sleutels beschikbaar.

Gebruik de **[!UICONTROL Apply transformation]** optie wanneer u *niet-gehashte* gebieden aan gehakte gebieden betrekt. Collaboration past de hashing toe en transformeert de velden. Het hash-algoritme dat door Adobe wordt gebruikt, is SHA256.

>[!ENDSHADEBOX]

Selecteer het lege bronveld naast het doelveld als u met de toewijzing van velden wilt beginnen. Het dialoogvenster **[!UICONTROL Select source field]** wordt weergegeven. Selecteer tussen de opties **[!UICONTROL Identity namespaces]** en **[!UICONTROL Profile attributes]** om het gewenste bronveld te zoeken en selecteer vervolgens het veld in de lijst. U kunt ook de zoekoptie gebruiken om het gewenste veld te zoeken.

![&#x200B; de Uitgezochte dialoog van het brongebied met de e-mailgetoonde opties.](/help/assets/setup/add-manage-audiences/select-source-field.png){zoomable="yes"}

Gebruik de optie **[!UICONTROL Apply transformation]** als u een niet-gehasht veld wilt betrekken bij een gehasht doelveld. Als u bijvoorbeeld een tweede e-mailveld wilt toevoegen, selecteert u de optie **[!UICONTROL Add field]** om een nieuwe rij toe te voegen en selecteert u **[!UICONTROL Hashed email]** voor het doelveld. Selecteer een bronveld voor een niet-gehashte e-mail en selecteer vervolgens **[!UICONTROL Apply transformation]** .

![&#x200B; Add de werkruimte van het publiek met de e-mailbrongebieden die aan het doelgebied worden in kaart gebracht, met Toepassen transformatie die voor één wordt van een knevel voorzien.](/help/assets/setup/add-manage-audiences/apply-transformation.png){zoomable="yes"}

Ga door met het toevoegen van toewijzingsparen voor elk doelveld. Als u niet wenst om een gelijke sleutel te gebruiken, kunt u het verwijderen gebruikend schrapping (![&#x200B; pictogram van de Schrapping &#x200B;](/help/assets/icons/delete.png)) naast het gebied. Als de overeenkomende sleutel wordt verwijderd, kunt u deze niet gebruiken wanneer u een publiek uit de verbinding ophaalt.

![&#x200B; Add publiek werkruimte met de optie van de Schrapping naast een benadrukt doelgebied.](/help/assets/setup/add-manage-audiences/remove-target-field.png){zoomable="yes"}

Als u alle toewijzingsvelden hebt, selecteert u **[!UICONTROL Next]** om door te gaan.

![&#x200B; voegt toe publiek werkruimte met de kaartgebieden die binnen worden gevuld en de Volgende benadrukte optie.](/help/assets/setup/add-manage-audiences/confirm-field-mapping.png){zoomable="yes"}

### Schema {#schedule}

Stel vervolgens in wanneer het publiek moet worden ingevuld. Het publiek wordt volgens dit schema vernieuwd.

![&#x200B; Add publiekswerkruimte met de het plannen getoonde opties.](/help/assets/setup/add-manage-audiences/audience-scheduling.png){zoomable="yes"}

>[!IMPORTANT]
>
>Het aanpassen van de frequentie van publieksupdates zal helpen de [&#x200B; de kredietactiviteit van het Beheer van de Publiek beheren &#x200B;](/help/guide/setup/my-activity.md#types-of-activities), die per publiek wordt berekend verfrist zich. Het selecteren van een hogere frequentie kan invloed hebben op de versheid van de gegevens beschikbaar voor publiek ontdekt rapporten en publieksactivering.

Selecteer in het vervolgkeuzemenu **[!UICONTROL Frequency]** de frequentie waarmee het publiek zich moet vernieuwen.

![&#x200B; Add publiek dat werkruimte met open drop-down van de Frequentie plant.](/help/assets/setup/add-manage-audiences/audience-scheduling-frequency.png){zoomable="yes"}

Selecteer vervolgens **[!UICONTROL Date range]** . De begindatum is de datum waarop het publiek begint met het vullen met profielen en de einddatum is wanneer het publiek stopt met vernieuwen.

![&#x200B; Add publiek dat werkruimte met de getoonde de waaieroptie van de Datum plant.](/help/assets/setup/add-manage-audiences/audience-scheduling-date-range.png){zoomable="yes"}

>[!IMPORTANT]
>
>Na de einddatum in het datumbereik wordt het vernieuwen van alle soorten publiek die afkomstig zijn van deze gegevensverbinding beëindigd. Om de verbinding te vernieuwen, volg [&#x200B; gegevensverbinding &#x200B;](/help/guide/setup/manage-data-connection.md) gids beheren.

### Soorten publiek selecteren {#select-audiences}

Nadat u de publieksbron hebt geselecteerd, kiest u een specifiek publiek dat u wilt opnemen. Gebruik de opties voor zoeken en filteren om het relevante publiek te zoeken via de gegevensverbinding. Selecteer het gewenste publiek en selecteer vervolgens **[!UICONTROL Next]** .

![&#x200B; Add publiek werkruimte met een lijst van beschikbare doelsoorten.](/help/assets/setup/add-manage-audiences/select-audience.png){zoomable="yes"}

### Controleren

Bekijk alle configuraties en instellingen voordat u de publiekstoevoeging voltooit. Controleer of alle gegevens correct zijn en selecteer **[!UICONTROL Complete]** om de gegevensverbinding te voltooien.

![&#x200B; Add publiek werkruimte met alle uitgezochte getoonde configuraties.](/help/assets/setup/add-manage-audiences/review-connection.png){zoomable="yes"}

## Het dashboard voor soorten publiek weergeven {#view-audiences-dashboard}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_missing_identities"
>title="Ontbrekende identiteiten"
>abstract="Het aantal identiteiten zal beschikbaar zijn nadat de volgende gegevensverbinding na het gevormde programma verfrist zich. De eerste vernieuwing vindt gewoonlijk plaats binnen 24 uur nadat de gegevensverbinding is ingesteld. De voortdurende verfrissingen zullen het gevormde programma volgen."

Na het zoeken naar soorten publiek worden in de **[!UICONTROL My audiences]** -werkruimte alle soorten publiek weergegeven die momenteel in Collaboration zijn binnengebracht.

![&#x200B; Mijn publiek werkruimte die alle afkomstig publiek tonen.](/help/assets/setup/add-manage-audiences/audiences-workspace.png)

Elk publiek bevat een overzicht van de volgende informatie:

| Item | Beschrijving |
|----------|---------|
| **[!UICONTROL Name]** | De naam van het publiek. |
| **[!UICONTROL Identities]** | Geeft het aantal identiteiten aan dat in dit publiek aanwezig is. Als hetzelfde profiel twee of meer identiteiten heeft en deze identiteiten als overeenkomende sleutels in het project worden gebruikt, wordt het profiel twee keer weergegeven in de telling. |
| **[!UICONTROL Status]** | Geeft aan of het publiek actief is en kan worden gebruikt in projecten. Een **[!UICONTROL Pending]** -status geeft aan dat het publiek onlangs is gedownload en dat identiteiten nog niet zijn gevuld. Het publiek op basis van bronnen krijgt profielen na de eerste vernieuwing, die gewoonlijk binnen 24 uur na het instellen van de gegevensverbinding plaatsvindt. |
| **[!UICONTROL Source]** | Geeft aan waar het publiek vandaan kwam. In de huidige release van Collaboration is Experience Platform de enige ondersteunde bron. |
| **[!UICONTROL Data connection]** | De gegevensverbinding waarvan het publiek afkomstig is. U kunt de naam selecteren om de gegevensverbinding te bekijken. |
| **[!UICONTROL Connection access]** | Bepaalt of het publiek privé of openbaar is. Openbare doelgroepen zijn te vinden in overlappende rapporten en kunnen binnen een project worden geactiveerd. |
| **[!UICONTROL Created]** | Geeft aan wanneer het publiek oorspronkelijk naar Collaboration was gedownload. |
| **[!UICONTROL Last updated]** | Geeft de laatste datum en tijd aan waarop het publiek in Collaboration is bijgewerkt. Dit verwijst niet naar wanneer het publiek het laatst werd verfrist, maar eerder wanneer de configuratie of de meta-gegevens van het publiek het laatst werden veranderd. |

![&#x200B; de Mijn publiekswerkruimte die alle afkomstig publiek tonen.](/help/assets/setup/add-manage-audiences/audiences-workspace.png){zoomable="yes"}

Om snelle acties op een publiek uit te voeren, selecteer de ellips **...** naast de publieksnaam. De volgende opties zijn beschikbaar:

* Met **[!UICONTROL Edit categories]** kunt u verschillende categorietags toevoegen aan het publiek. Voor meer informatie, verwijs naar de [&#x200B; categorieën &#x200B;](#categories) hieronder sectie.
* **[!UICONTROL Delete]** verwijdert het publiek uit de gegevensverbinding.

![&#x200B; Mijn publiek werkruimte met het open weglatingsmenu en uitgeeft categorieën en benadrukt de opties van de Schrapping.](/help/assets/setup/add-manage-audiences/audiences-ellipsis-menu.png){zoomable="yes"}

## Individuele doelgroepen weergeven {#view-individual-audiences}

Als u informatie voor een afzonderlijk publiek wilt weergeven en bijwerken, selecteert u het desbetreffende publiek in de werkruimte van **[!UICONTROL My audiences]** . De publiekswerkruimte bevat gedetailleerde informatie over het geselecteerde publiek, zoals de details, identiteiten, categorieën, toegang tot de verbinding en instellingen voor de zichtbaarheid van metagegevens.

### Details publiek

De volgende informatie wordt voor elk individueel publiek getoond:

| Item | Beschrijving |
|----------|---------|
| **[!UICONTROL Status]** | Geeft aan of het publiek actief is en kan worden gebruikt in projecten. |
| **[!UICONTROL Source]** | Geeft aan waar het publiek vandaan kwam. In de huidige release van Collaboration is Experience Platform de enige ondersteunde bron. |
| **[!UICONTROL Data connection]** | De gegevensverbinding waarvan het publiek afkomstig is. |
| **[!UICONTROL Last updated]** | Geeft de laatste datum en tijd aan waarop het publiek in Collaboration is bijgewerkt. Dit verwijst niet naar wanneer het publiek het laatst werd verfrist, maar eerder toen de configuratie of de meta-gegevens van het publiek het laatst werden veranderd |
| **[!UICONTROL Last updated by]** | Geeft de gebruiker aan die het publiek voor het laatst heeft bijgewerkt. |
| **[!UICONTROL Created]** | Geeft aan wanneer het publiek oorspronkelijk naar Collaboration was gedownload. |
| **[!UICONTROL Created by]** | Geeft de gebruiker aan die het publiek naar Collaboration heeft gedownload. |

![&#x200B; de werkruimte van een individueel publiek.](/help/assets/setup/add-manage-audiences/audience-details.png){zoomable="yes"}

#### Identiteiten {#identities}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_identities"
>title="Identiteiten"
>abstract="Een uitsplitsingsweergave van de identiteiten waaruit dit publiek bestaat, gescheiden door de overeenkomende sleutel."

De sectie **[!UICONTROL Identities]** geeft het aantal identiteiten aan dat in het publiek aanwezig is. De sectie bevat ook een identiteitsverdeling van identiteiten door gelijkesleutel om u te helpen de samenstelling van het publiek begrijpen.

![&#x200B; de sectie van Identiteiten van de werkruimte van een individueel publiek.](/help/assets/setup/add-manage-audiences/audience-details-identities.png){zoomable="yes"}

Het boven de afzonderlijke gedeelten van de uitsplitsing naar matchsleutel houden zal een nauwkeurige telling van de identiteit voor de desbetreffende sleutel opleveren.

![&#x200B; de sectie van Identiteiten van de werkruimte van een individueel publiek met de getoonde onderbreking van een gelijke sleutel.](/help/assets/setup/add-manage-audiences/audience-details-identities.png)

#### Categorieën {#categories}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_categories"
>title="Categorieën"
>abstract="Geef uw publiek tags voor eenvoudige organisatie, filteren en ophalen. U kunt een publiek met meerdere categorieën tags toewijzen en vervolgens deze categorietags gebruiken om het gewenste publiek in andere gebieden van het product te filteren."

Voor eenvoudige publieksorganisatie, het filtreren, en het terugwinnen, kunt u uw publiek etiketteren. U kunt een publiek met veelvoudige categorieën etiketteren en dan kunt u deze categorietags gebruiken om uw gewenste publiek in [&#x200B; te filtreren ontdekken &#x200B;](/help/guide/collaborate/discover.md) productgebied, wanneer het runnen van publiek overlappende rapporten.

Als u categorieën wilt toevoegen, selecteert u de optie **[!UICONTROL Edit]** in de sectie **[!UICONTROL Categories]** .

![&#x200B; de sectie van Categorieën van de werkruimte van een individueel publiek.](/help/assets/setup/add-manage-audiences/audience-details-categories.png){zoomable="yes"}

Het dialoogvenster **[!UICONTROL Categories]** wordt weergegeven, zodat u de categorieën kunt selecteren die u aan het publiek wilt toevoegen. Als u een afzonderlijke categorie wilt selecteren, schakelt u het selectievakje naast de categorienaam in.


#### Toegang tot verbinding {#connection-access}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_connection_access"
>title="Toegang tot verbinding"
>abstract="<p>De soorten publiek kunnen van drie types zijn: publiek, privé, en douane.</p><p> Hun beschikbaarheid voor gebruik in projecten met medewerkers verschilt gebaseerd op het plaatsen van de verbindingstoegang.</p>"

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_access"
>title="Meer informatie"
>abstract=""

De beschikbaarheid van een publiek voor gebruik in projecten met medewerkers verschilt afhankelijk van de instelling voor de toegang tot de verbinding. In de sectie **[!UICONTROL Connection access]** kunt u aangeven of het publiek privé, openbaar of alleen beschikbaar moet zijn voor specifieke verbindingen. Het publiek is bruikbaar en te ontdekken in verbindingen.

Als u de toegang tot de verbinding van de doelgroep wilt bijwerken, selecteert u de optie **[!UICONTROL Edit]** in de **[!UICONTROL Connection access]** -sectie.

![&#x200B; de de toegangssectie van de Verbinding van de werkruimte van een individueel publiek.](/help/assets/setup/add-manage-audiences/audience-details-connection-access.png){zoomable="yes"}

Het dialoogvenster **[!UICONTROL Connection access]** wordt weergegeven met drie beschikbare toegangsopties voor de verbinding:

* **[!UICONTROL Private audience]**. Dit publiek is *niet* beschikbaar voor gebruik in overlappende rapporten of voor activering in verbindingen met om het even welke medewerkers. Terwijl het publiek niet voor medewerkers beschikbaar is om te bekijken of te gebruiken, draagt de bevolking van het publiek nog aan de totale bevolking in de **[!UICONTROL All audiences]** mening in de [&#x200B; vergelijkingspubliekssectie &#x200B;](/help/guide/collaborate/discover.md#compare-audiences) bij. Wijzig de instelling in Openbaar of Aangepast als u het publiek wilt gebruiken in verbindingen met medewerkers.
* **[!UICONTROL Public audience]**. Deze doelgroepen zijn beschikbaar voor gebruik in overlappende rapporten en voor activering in verbindingen met deelnemers.
* **[!UICONTROL Custom audience]**. Deze soorten publiek zijn alleen beschikbaar voor gebruik in overlappende rapporten en voor activering in opgegeven verbindingen. Terwijl het publiek niet voor medewerkers beschikbaar is om te bekijken of te gebruiken, draagt de bevolking van het publiek nog aan de totale bevolking in de **[!UICONTROL All audiences]** mening in de [&#x200B; vergelijkingspubliekssectie &#x200B;](/help/guide/collaborate/discover.md#compare-audiences) bij.

Selecteer de gewenste toegangsoptie voor de verbinding en selecteer vervolgens **[!UICONTROL Save]** om de wijzigingen toe te passen.

![&#x200B; het de toegangsdialoog van de Verbinding met de beschikbare getoonde opties.](/help/assets/setup/add-manage-audiences/audience-details-connection-access-dialog.png){zoomable="yes"}

>[!IMPORTANT]
>
>Ongeacht de toegangsstatus (public, private of custom), levert de populatie van een publiek een bijdrage aan de **[!UICONTROL All audiences]** -populatie in de **[!UICONTROL Compare audiences]** -sectie in een project.

De beschikbaarheid van het publiek voor gebruik in projecten met medewerkers verschilt gebaseerd op het plaatsen van de verbindingstoegang.

#### Zichtbaarheid metagegevens {#metadata-visibility}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_metadata_visibility"
>title="Zichtbaarheid metagegevens"
>abstract="<p>Geeft aan welke metagegevens van het publiek zichtbaar zijn voor andere deelnemers voordat ze verbinding maken met u of binnen de projectweergave.</p> <p> **de telling van de Identiteit** controleert of uw medewerker identiteitstellingen voor uw publiek kan bekijken wanneer het bekijken van overlappende rapporten in de ontdekking tabel.</p><p> **het publiek overlapt %** controleert of de medewerkers overlappende percentages tussen hun publiek en van u kunnen ontdekken.</p><p> **[!UICONTROL Audience index]** bepaalt of deelnemers de publieksindex in een project kunnen weergeven. Deze functionaliteit is alleen beschikbaar wanneer u drie of meer actieve doelgroepen hebt.</p> <br> Als u wilt dat de zichtbaarheidsinstellingen voor metagegevens van kracht worden, moet het publiek zijn ingesteld op Openbaar of Aangepast."

>[!NOTE]
>
>Als voor uw medewerker alle soorten publiek zijn ingesteld op Private, is de sectie **[!UICONTROL Relevant audiences]** van een project in de **[!UICONTROL Discover]** -werkruimte leeg. Voor meer informatie, lees [&#x200B; ontdek &#x200B;](/help/guide/collaborate/discover.md#relevant-audiences) gids.

De zichtbaarheid van metagegevens geeft de zichtbaarheid van de metagegevens van een publiek aan voor andere deelnemers voordat ze verbinding maken met u of binnen verschillende projectweergaven. Als u de zichtbaarheid van de metagegevens van de doelgroep wilt bijwerken, selecteert u de optie **[!UICONTROL Edit]** in de **[!UICONTROL Metadata visibility]** -sectie.

![&#x200B; de de zichtbaarheidssectie van Meta-gegevens van de werkruimte van een individueel publiek.](/help/assets/setup/add-manage-audiences/audience-details-metadata-visibility.png){zoomable="yes"}

Het dialoogvenster **[!UICONTROL Metadata visibility]** wordt weergegeven, zodat u de zichtbaarheidsinstellingen voor het publiek kunt configureren. Er zijn twee montages van de meta-gegevenszichtbaarheid die u voor elk publiek kunt vormen:

**[!UICONTROL Show identity count]**: Dit het plaatsen controleert of uw medewerker identiteitstellingen voor uw publiek kan bekijken wanneer [&#x200B; het bekijken overlappende rapporten in het ontdekkingslusje &#x200B;](/help/guide/collaborate/discover.md#discover-overlaps) binnen een project.

**[!UICONTROL Show audience overlap %]**: Dit het plaatsen controleert of de medewerkers [&#x200B; overlappende percentages &#x200B;](/help/guide/collaborate/discover.md#compare-audiences) tussen hun publiek en uw publiek kunnen ontdekken.

**[!UICONTROL Audience index]**: Wanneer reeks aan waar, kunnen uw medewerkers de [&#x200B; publieksindex &#x200B;](/help/guide/collaborate/discover.md#audience-index-score) binnen een project bekijken. Deze functionaliteit is alleen beschikbaar wanneer u drie of meer actieve doelgroepen hebt.

>[!NOTE]
>
>De instellingen voor de zichtbaarheid van metagegevens worden pas van kracht als het publiek is ingesteld op Openbaar of Aangepast.

![&#x200B; het de zichtbaarheidsdialoog van Meta-gegevens met de beschikbare getoonde opties.](/help/assets/setup/add-manage-audiences/audience-details-metadata-dialog.png){zoomable="yes"}

## Meerdere soorten publiek bewerken {#edit-audiences}

Vanuit het doeldashboard kunt u meerdere soorten publiek tegelijk bewerken. U doet dit door het publiek dat u wilt bewerken te selecteren door de vakken naast de namen te selecteren. Nadat u het publiek hebt geselecteerd, kunt u handelingen uitvoeren met de opties in het menu Bewerken.

![&#x200B; Mijn aangewezen publiek werkruimte met twee geselecteerd publiek en uitgeeft menu.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit.png)

### Zichtbaarheid van metagegevens in bulk bewerken {#bulk-edit-metadata-visibility}

Selecteer het publiek in het doeldashboard en selecteer **[!UICONTROL Edit metadata visibility]** in het menu Bewerken.

![&#x200B; Mijn publiek werkruimte met de Edit benadrukte optie van het meta-gegevenszicht.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-metadata.png)

Het dialoogvenster **[!UICONTROL Metadata visibility]** wordt weergegeven, zodat u de zichtbaarheidsinstellingen voor het geselecteerde publiek kunt configureren. Standaard worden geen opties geselecteerd. Kies de opties die u op alle geselecteerde doelgroepen wilt toepassen en selecteer vervolgens **[!UICONTROL Save]** .

![&#x200B; het de zichtbaarheidsdialoog van Meta-gegevens met de beschikbare getoonde opties.](/help/assets/setup/add-manage-audiences/audience-details-metadata-dialog.png)

### Toegang tot een bulkbewerkingsverbinding {#bulk-edit-connection-access}

Selecteer het publiek in het doeldashboard en selecteer **[!UICONTROL Edit connection access]** in het menu Bewerken.

![&#x200B; Mijn publiek werkruimte met de Edit benadrukte optie van de verbindingstoegang.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-connection-access.png)

Het dialoogvenster **[!UICONTROL Connection access]** wordt weergegeven, zodat u de toegangsinstellingen voor het geselecteerde publiek kunt configureren. Standaard wordt de optie **[!UICONTROL Private audience]** geselecteerd. Kies de opties die u op alle geselecteerde doelgroepen wilt toepassen en selecteer vervolgens **[!UICONTROL Save]** .

![&#x200B; het de toegangsdialoog van de Verbinding met de beschikbare getoonde opties.](/help/assets/setup/add-manage-audiences/audience-details-connection-access-dialog.png)

### Publiceer publieksnamen en -beschrijvingen in bulk {#bulk-edit-audience-names-descriptions}

Selecteer het publiek in het doeldashboard en selecteer **[!UICONTROL Edit name and description]** in het menu Bewerken.

![&#x200B; Mijn publiek werkruimte met Edit naam en beschrijving benadrukte optie.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-name-description.png)

Het dialoogvenster **[!UICONTROL Name and description]** wordt weergegeven, zodat u de naam en beschrijving voor elk geselecteerd publiek kunt configureren. Standaard worden de huidige namen en beschrijvingen voor elk publiek weergegeven. Breng de gewenste wijzigingen aan en selecteer vervolgens **[!UICONTROL Save]** .

![&#x200B; de Naam en beschrijvingsdialoog met de beschikbare getoonde opties.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-name-description-dialog.png)

### Categorieën voor bulkbewerking {#bulk-edit-categories}

Selecteer het publiek in het doeldashboard en selecteer **[!UICONTROL Edit categories]** in het menu Bewerken.

![&#x200B; Mijn publiek werkruimte met de Edit benadrukte categoriesoptie.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-categories.png)

Het dialoogvenster **[!UICONTROL Categories]** wordt weergegeven, zodat u de categorieën voor elk geselecteerd publiek kunt configureren. Standaard worden geen categorieën geselecteerd. Als u een categorie wilt selecteren, selecteert u eerst de hoofdcategorie en daarna de subcategorieën die u wilt opnemen. Breng de gewenste wijzigingen aan en selecteer vervolgens **[!UICONTROL Save]** .

![&#x200B; de dialoog van Categorieën met de beschikbare getoonde opties.](/help/assets/setup/add-manage-audiences/audiences-bulk-edit-categories-dialog.png)

## Volgende stappen

Na het sourcen van publiek, is het tijd om medewerkers aan [&#x200B; te ontdekken verbinden &#x200B;](/help/guide/connect/establishing-connections.md) met om aan projecten samen te werken.
