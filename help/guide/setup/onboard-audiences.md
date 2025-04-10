---
title: Soorten publiek importeren en beheren
description: Meer informatie over het importeren en beheren van soorten publiek in Adobe Real-Time CDP Collaboration
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 0a5158fa-73d3-4406-af20-2b6c7be9934e
source-git-commit: ff22dde9730fab89481338753b1dc4a0adf1d57e
workflow-type: tm+mt
source-wordcount: '2577'
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

Voordat u het publiek met medewerkers kunt delen en overlappende berekeningen kunt uitvoeren, moet het publiek naar Real-Time CDP Collaboration worden geïmporteerd. Volg de workflowstappen in de onderstaande sectie om het publiek te importeren.

![ Mijn publiek het scherm alvorens om het even welk publiek aan org is toegevoegd.](/help/assets/setup/add-manage-audiences/org-without-audiences-added.png)

Van het **[!UICONTROL My audiences]** lusje, selecteer plus **+** symbool, en selecteer **Publiek**.

### Gegevensverbinding selecteren {#select-data-connection}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_marketing_actions"
>title="Marketingacties"
>abstract="<p>Gebruik marketingacties om te bepalen welke publieksgegevens uit Experience Platform in Real-Time CDP Collaboration moeten worden geïmporteerd. De </strong> marketing actie van Collaboration van 0} Gegevens steunt C4, C5 en C9 de etiketten van het gegevensgebruik. <strong> De </strong> marketing actie van de Wetenschap van 0} Gegevens steunt het C9 etiket van het gegevensgebruik.<strong></p> <p> <ul><li> Met checkbox <em> toegelaten </em>, wordt om het even welk gegeven dat met de etiketten duidelijk is die hierboven in Experience Platform worden geroepen uitgesloten en wordt <strong> niet </strong> gebracht in Real-Time CDP Collaboration.</li><li> Met checkbox <em> gehandicapt </em>, is er geen beperking op gegevens van Experience Platform die in Real-Time CDP Collaboration kunnen worden ingevoerd.</li></ul></p>"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/overview.html" text="Overzicht van labels voor gegevensgebruik"
>additional-url="https://experienceleague.adobe.com/docs/experience-platform/data-governance/labels/reference.html" text="Verklarende woordenlijst met gegevensgebruikslabels"

>[!IMPORTANT]
>
>Nadat u verbinding hebt gemaakt met de eerste gegevensverbinding en uw eerste publiek hebt geïmporteerd, kunt u vervolgens selecteren om meerdere publiek te importeren vanuit deze bestaande gegevensverbinding. In dit geval, zal het werkschema u aan de [ uitgezochte publiek ](#select-audience) stap direct nemen, aangezien alle in de eerste plaats vereiste informatie van de andere stappen van de bestaande verbinding zal worden ingevoerd.

Een gegevensverbinding is de gegevensbron waaruit u publiek importeert in Real-Time CDP Collaboration. Voor de eerste release van Real-Time CDP Collaboration is Adobe Experience Platform de enige ondersteunde gegevensverbinding.

Alle instellingen, zoals identiteitstoewijzing of planning die u configureert voor uw gegevensverbinding, worden toegepast op alle publiek dat wordt geïmporteerd vanuit deze gegevensverbinding.

>[!TIP]
>
>Er is een aparte workflow waarin u altijd alle gegevensverbindingen kunt weergeven en bewerken die u in deze stap hebt toegevoegd. Lees meer over [ het beheren van gegevensverbindingen ](/help/guide/setup/manage-data-connection.md).

![ Uitgezochte publiek bron het scherm dat opties voor AEP RTCDP, Csv- Dossier, Amazon S3, en Snowflake toont.](/help/assets/setup/add-manage-audiences/Step-Select-Audience-Source.png)

#### Gegevensbron selecteren

In deze stap kiest u de bron van uw publieksgegevens. De beschikbare bronnen zijn onder meer:

* **Adobe Experience Platform**: Selecteer deze optie om uw publiek van Adobe Experience Platform Real-Time CDP te brengen.
* **Csv- Dossier** (Toekomstige versie): Upload een Csv- dossier dat uw publieksgegevens voor snelle en ongecompliceerde gegevensopname bevat.
* **Amazon Web Services** (Toekomstige versie): Verbind met uw opslag van Amazon S3 om publieksgegevens van uw S3 emmers direct in te voeren.
* **Snowflake** (Toekomstige versie): Gebruik uw gegevenspakhuis van Snowflake om in publieksgegevens foutloos te trekken.

#### Sandbox selecteren

Na het selecteren van **Adobe Experience Platform** als gegevensbron, moet u de zandbak selecteren die het publiek omvat dat u zult invoeren.

![ Uitgezochte zandbak voor het invoeren van publiek ](/help/assets/setup/add-manage-audiences/import-audiences-select-sandbox.png)

Selecteer **[!UICONTROL Next]** nadat u de gewenste sandbox hebt geselecteerd.

#### Beleid inzake governance en handhavingsmaatregelen {#governance-policy-and-enforcement-actions}

Vervolgens moet u ervoor zorgen dat de juiste marketingacties zijn ingesteld voor de geïmporteerde gegevens. U moet ook toestemming geven voor het gebruik van uit Real-Time CDP geïmporteerde gegevens voor gegevenssamenwerking.

Gebruik marketingacties om te bepalen welke publieksgegevens uit Experience Platform in Real-Time CDP Collaboration moeten worden geïmporteerd. De **marketing actie van Collaboration van 0} Gegevens steunt C4, C5 en C9 de etiketten van het gegevensgebruik.** De **marketing actie van de Wetenschap van 0} Gegevens steunt het C9 etiket van het gegevensgebruik.**

Lees meer over [ C4, C5, en C9 de etiketten van het gegevensgebruik ](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference#contract){target="_blank"}.

* Met checkbox *toegelaten*, wordt om het even welk gegeven dat met de etiketten duidelijk is die hierboven in Experience Platform worden geroepen uitgesloten en wordt *niet* gebracht in Real-Time CDP Collaboration.
* Met checkbox *gehandicapt*, is er geen beperking op gegevens van Experience Platform die in Real-Time CDP Collaboration kunnen worden ingevoerd.

Meer informatie over labels voor gegevensgebruik vindt u in de documentatie van Experience Platform:

* [ overzicht van de gebruiksetiketten van Gegevens ](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/overview){target="_blank"}
* [ de etiketten van het gebruiksgebruik van Gegevens verklarende woordenlijst ](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/labels/reference){target="_blank"}

![ Vereiste marketing acties voor gegevenssamenwerking.](/help/assets/setup/add-manage-audiences/data-collaboration-consent.png)

### Geef details

Geef vervolgens een naam en een beschrijving op waarmee u deze gegevensverbinding in de toekomst kunt herkennen.

<!--

>[!IMPORTANT]
>
>Note a difference in terminology where the sandbox selected from Real-Time CDP is considered a dataset in the UI in Real-Time CDP Collaboration.

-->

### Toewijzingsvelden {#map-fields}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_source_fields"
>title="Source-velden"
>abstract="Source-velden zijn naamruimten en kenmerken van uw bestaande Real-Time CDP-implementatie. U kunt deze toewijzen aan doelvelden die zijn gedefinieerd in Real-Time CDP Collaboration."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_mapping_target_fields"
>title="Doelvelden"
>abstract="De doelvelden komen overeen met de overeenkomende toetsen die u hebt geselecteerd bij het instappen van uw bedrijf. Gehashte e-mails zijn momenteel de enige ondersteunde overeenkomende sleutels."

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

![ het scherm van de Velden van de Kaart die brongebieden tonen aan doelgebieden in kaart worden gebracht.](/help/assets/setup/add-manage-audiences/Step-Map-Fields.png)

In de stap van de kaartgebieden, kunt u selecteren hoe om het even welke identiteitsgebieden voor de profielen die van de gegevensverbinding worden gebracht aan de gelijknamensleutels zouden moeten in kaart brengen die u in uw organisatie selecteerde.

>[!TIP]
>
>U kunt meerdere bronvelden toewijzen aan hetzelfde doelveld. Als u bijvoorbeeld e-mailadressen hebt in twee verschillende velden in Experience Platform, kunt u beide aan het doelveld van **[!UICONTROL Hashed email]** toewijzen als twee aparte rijen.

>[!BEGINSHADEBOX]

**[!UICONTROL Source fields]** geeft aan hoe naar de identiteiten wordt verwezen in de bron waaruit u gegevens importeert.

**[!UICONTROL Target fields]** geeft aan hoe naar de identiteiten wordt verwezen in Real-Time CDP Collaboration. De waarden die u hier kunt selecteren, komen overeen met de sleutels die u instelt in het bedrijf dat de workflow aan boord heeft.

Gebruik de **[!UICONTROL Apply transformation]** optie wanneer u *niet-gehakt* gebieden van uw bron invoert. In dit geval past Real-Time CDP Collaboration de hash toe en transformeert het de velden. Het hash-algoritme dat door Adobe wordt gebruikt, is SHA256.

>[!ENDSHADEBOX]

Voeg zoveel toewijzingsparen toe als u nodig hebt en selecteer **[!UICONTROL Next]** om door te gaan naar de volgende stap.

<!--

In this step, you can also add any identity crosswalks that you would like to use.

Identity crosswalks will be supported after the beta release.

#### Add identity crosswalk

Use identity crosswalks to connect different identifiers across datasets to enrich your audience data with additional attributes or dimensions. 

TODO add GIF Identity crosswalks screen showing a list of available identity crosswalks with details.

Select **[!UICONTROL Add identity crosswalk]** to see a screen where you can choose from various identity crosswalks that you have previously [imported into Real-Time CDP Collaboration](/help/guide/setup/identity-crosswalk.md#import-crosswalk). Each entry includes details such as the table name, type, description, and creation date.

After selecting the desired crosswalk, use a source field join key to map to the crosswalk table join key. 

>[!NOTE]
>
>After selecting an identity crosswalk, the **[!UICONTROL Add identity crosswalk]** control is greyed out. 

For further reading about identity crosswalks, refer to the [glossary](/help/guide/glossary.md).

-->


<!-- will uncomment this part when Manage use cases part becomes available

### Manage use cases {#manage-use-cases}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_audience_usecases"
>title="Use cases for identities"
>abstract="This control is disabled in the initial release of Real-Time CDP Collaboration"

![Manage use cases screen.](/help/assets/setup/add-manage-audiences/Step-manage-use-cases.png)

For every identity selected in the mapping step, select the use cases that you can use the identity for. Available use cases are: 

* Discover
* Share
* Activate
* Measure

Note that this control is disabled in the initial release of Real-Time CDP Collaboration.

After selecting the desired use cases for each identity, proceed to the next step. 

-->

### Schema {#schedule}

Plan wanneer het publiek moet worden gevuld en vernieuwd. Het lidmaatschap van het publiek wordt volgens dit schema vernieuwd.

![ het scherm van het Programma dat begin en einddata toont om het publiek te bevolken.](/help/assets/setup/add-manage-audiences/Step-Schedule.png)

Selecteer de vernieuwingsfrequentie voor het publiek. De beschikbare opties liggen tussen de vernieuwingssnelheden van 1 en 6 dagen.

>[!IMPORTANT]
>
>Het aanpassen van de frequentie van publieksupdates zal helpen de [ de kredietactiviteit van het Beheer van de Publiek beheren ](/help/guide/setup/my-activity.md#types-of-activities), die per publieksenlidmaatschap wordt berekend verfrist zich. Dit kan minder nieuwe gegevens opleveren die de doelgroep kan gebruiken om rapporten en het delen en activeren van het publiek te ontdekken.

![ het scherm dat van het Programma verschillende frequentiedetails voor het bijwerken van publiekslidmaatschap toont.](/help/assets/setup/add-manage-audiences/Step-Schedule-Set-Frequency.png)

>[!IMPORTANT]
>
>Na de einddatum in het datumbereik wordt het vernieuwen stopgezet van alle soorten publiek die worden geïmporteerd uit deze gegevensverbinding. Om de verbinding te vernieuwen, ga [ gegevensverbinding beheren ](/help/guide/setup/manage-data-connection.md), en plaats een nieuwe einddatum.

### Soorten publiek selecteren {#select-audience}

Nadat u de publieksbron hebt geselecteerd, kiest u een specifiek publiek dat u wilt opnemen. Gebruik de zoek- en filteropties op de pagina om het relevante publiek te zoeken vanuit de geselecteerde gegevensbron.

![Selecteer het publieksscherm met een lijst met beschikbare doelgroepen met selectievakjes om ze te selecteren.](/help/assets/setup/add-manage-audiences/Step-Select-Audience.png)

### Recensie

Bekijk alle configuraties en instellingen voordat u de toevoeging aan het publiek voltooit. Zorg ervoor dat alle details correct zijn en selecteer **[!UICONTROL Complete]** om het proces af te ronden.

## Dashboard voor doelgroepen weergeven {#view-audiences-dashboard}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_missing_identities"
>title="Ontbrekende identiteiten"
>abstract="Het aantal identiteiten wordt weergegeven `-` gedurende ongeveer de eerste 24 uur nadat een publiek is geïmporteerd in Real-Time CDP Collaboration. Na deze periode wordt het aantal identiteiten bijgewerkt met het aantal profielen dat in het publiek aanwezig is."

Nadat u doelgroepen hebt geïmporteerd in Real-Time CDP Collaboration, kunt u informatie over hen ophalen in een dashboardweergave. In de standaardweergave op de **[!UICONTROL My audiences]** pagina worden alle doelgroepen weergegeven die momenteel door uw organisatie zijn geïmporteerd in Real-Time CDP Collaboration.

![Overzichtspagina voor doelgroepen met alle doelgroepen die door een adverteerder zijn geïmporteerd](/help/assets/setup/add-manage-audiences/audiences-overview.png)

U kunt de volgende relevante informatie over elke doelgroep bekijken:

| Item | Beschrijving |
|----------|---------|
| **[!UICONTROL Identities]** | Geeft het aantal identiteiten aan dat in dit publiek aanwezig is. Als hetzelfde profiel twee of meer identiteiten heeft en deze identiteiten als overeenkomende sleutels in het project worden gebruikt, wordt het profiel twee keer weergegeven in de telling. |
| **[!UICONTROL Status]** | Geeft aan of het publiek actief is en kan worden gebruikt in projecten. Een status in behandeling geeft aan dat het publiek onlangs is geïmporteerd en dat publieksleden nog niet zijn gevuld. Het geïmporteerde publiek vult de profielen meestal binnen 24 uur. |
| **[!UICONTROL Source]** | Geeft de bron aan waaruit dit publiek is geïmporteerd. In de huidige release van Real-Time CDP Collaboration is Adobe Experience Platform de enige ondersteunde bron. |
| **[!UICONTROL Data connection]** | Meer informatie over waar dit publiek is geïmporteerd. Wanneer u bijvoorbeeld een publiek importeert uit de Experience Platform-bron, worden de afzonderlijke sandboxen waartoe uw organisatie toegang heeft, beschouwd als de gegevensverbindingen. |
| **[!UICONTROL Connection access]** | Bepaalt of dit publiek privé of openbaar is. Openbare doelgroepen zijn te vinden in overlappende rapporten en kunnen met deelnemers worden gedeeld. |
| **[!UICONTROL Created]** | Geeft aan wanneer dit publiek naar Real-Time CDP Collaboration is geïmporteerd. |
| **[!UICONTROL Last updated]** | Geeft de laatste datum en tijd aan waarop een aspect van dit publiek is bijgewerkt. |

Selecteer **[!UICONTROL Manage data connections]** om alle gegevensverbindingen weer te geven en te bewerken die u hebt ingesteld.
Selecteer de clip en **[!UICONTROL Delete]** om het publiek te verwijderen.
Selecteer de elipsis en **[!UICONTROL Edit categories]** om verschillende categorietags toe te voegen aan het publiek. Krijg meer informatie in de [ categorieën ](/#categories) hieronder sectie.
Selecteer de publieksnaam om afzonderlijke doelgroepen te inspecteren of te bewerken.

## Individuele doelgroepen weergeven {#view-individual-audiences}

In de publieksweergave vindt u meer informatie over uw publiek.

![ Mening en inspecteer individueel publiek.](/help/assets/setup/add-manage-audiences/view-inspect-audience.png)

De cijfers die u in dit scherm kunt bekijken, worden hieronder beschreven:

| Item | Beschrijving |
|----------|---------|
| **[!UICONTROL Status]** | Geeft aan of het publiek actief is en kan worden gebruikt in projecten. |
| **[!UICONTROL Source]** | Geeft de bron aan waaruit dit publiek is geïmporteerd. In de huidige release van Real-Time CDP Collaboration is Adobe Experience Platform de enige ondersteunde bron. |
| **[!UICONTROL Data connection]** | Meer informatie over waar dit publiek is geïmporteerd. Wanneer u bijvoorbeeld een publiek importeert uit de Experience Platform-bron, worden de afzonderlijke sandboxen waartoe uw organisatie toegang heeft, beschouwd als de gegevensverbindingen. |
| **[!UICONTROL Last updated]** | Geeft de laatste datum en tijd aan waarop een aspect van dit publiek is bijgewerkt. |
| **[!UICONTROL Last updated by]** | Geeft de gebruiker aan die dit publiek voor het laatst heeft bijgewerkt. |
| **[!UICONTROL Created]** | Geeft aan wanneer dit publiek naar Real-Time CDP Collaboration is geïmporteerd. |
| **[!UICONTROL Created by]** | Geeft de gebruiker aan die het publiek in Real-Time CDP Collaboration heeft geïmporteerd. |


U kunt nog twee besturingselementen op de pagina gebruiken om het publiek te bewerken of te verwijderen:

* **[!UICONTROL Delete]**: verwijder het publiek uit uw overzicht
* **[!UICONTROL Edit]**: Bewerk de metagegevens van het publiek zoals de naam of beschrijving.

![ Mening en inspecteer individueel publiek.](/help/assets/setup/add-manage-audiences/audiences-edit-delete-controls.png)

Meer informatie over het publiek is beschikbaar en gedeeltelijk bewerkbaar in de widgets hieronder:

![ Mening en inspecteer individueel publiek.](/help/assets/setup/add-manage-audiences/audiences-further-info-boxes.png)

* [Identiteiten](#identities)
* [Categorieën](#categories)
* [Toegang tot verbinding](#connection-access)
* [Zichtbaarheid metagegevens](#metadata-visibility)

### Identiteiten {#identities}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_identities"
>title="Identiteiten"
>abstract="Krijg een uitsplitsing van de identiteiten waaruit deze doelgroep bestaat, evenals een totaal aantal profielen met de respectievelijke identiteiten."

In dit gedeelte wordt het aantal profielen aangegeven dat aanwezig is in de doelgroep met een van de identiteiten die u hebt opgegeven bij het importeren van de doelgroepen. De sectie bevat ook een uitsplitsing van de identiteit, zodat u kunt zien welke identiteiten het grootste deel van de publiekspopulatie uitmaken.

### Categorieën {#categories}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_categories"
>title="Categorieën"
>abstract="Geef uw publiek tags voor eenvoudige organisatie, filteren en ophalen. U kunt een publiek met meerdere categorieën tags toewijzen en vervolgens deze categorietags gebruiken om het gewenste publiek in andere gebieden van het product te filteren."

Voor eenvoudige publieksorganisatie, het filtreren, en het terugwinnen, kunt u uw publiek etiketteren. U kunt een publiek met veelvoudige categorieën etiketteren en dan kunt u deze categorietags gebruiken om uw gewenste publiek in [ te filtreren ontdekken ](/help/guide/collaborate/discover.md) productgebied, wanneer het runnen van publiek overlappende rapporten.

### Toegang tot verbinding {#connection-access}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_connection_access"
>title="Toegang tot verbinding"
>abstract="<p>Er kunnen drie soorten doelgroepen zijn: openbaar, privé en op maat.</p><p> De beschikbaarheid voor gebruik in projecten met bijdragers is afhankelijk van de instelling voor verbindingstoegang. U kunt de toegang tot de verbinding altijd wijzigen van privé naar openbaar, maar u kunt die instelling niet meer wijzigen zodra een publiek is gedeeld met bijdragers.</p>"

Selecteer of het publiek privé voor jou moet zijn, of bruikbaar en vindbaar in connecties. De drie beschikbare opties zijn:

* **[!UICONTROL Public audience]**. Deze doelgroepen zijn beschikbaar voor gebruik in overlappende rapporten en voor het delen en activeren van verbindingen met deelnemers.
* **[!UICONTROL Private audience]**. Deze doelgroepen zijn *niet* beschikbaar voor gebruik in overlappende rapporten en voor delen en activeren in verbindingen met bijdragers Hoewel het niet beschikbaar is voor bijdragers om te bekijken of te gebruiken, draagt de populatie van deze doelgroep nog steeds bij aan de totale populatie in de **[!UICONTROL All audiences]** weergave in de [sectie](/help/guide/collaborate/discover.md#compare-audiences) Ontdekken en overlappen. Wijzig de instelling in openbaar of aangepast om de doelgroepen te gebruiken in verbindingen met bijdragers.
* **[!UICONTROL Custom audience]**. Deze doelgroepen zijn alleen beschikbaar voor gebruik in overlappende rapporten en voor delen en activeren in gespecificeerde verbindingen. Hoewel niet alle bijdragers kunnen worden bekeken of gebruikt, draagt de populatie van deze doelgroep nog steeds bij aan de totale populatie in de **[!UICONTROL All audiences]** weergave in de [sectie](/help/guide/collaborate/discover.md) Ontdekken en overlappen.

>[!IMPORTANT]
>
>Ongeacht de toegangsstatus (public, private of custom), draagt de populatie van een publiek bij aan de **[!UICONTROL All audiences]** -populatie in de analyse Audience Discovery overlapt deze. <br> ![ het systeem-geproduceerde **Alle publiek** publiek in de Ontdekking van het publiek overlapt analyse is inclusief van publiek met alle statussen van de verbindingstoegang (openbaar, privé, douane).](/help/assets/setup/add-manage-audiences/all-audiences-view.png " het systeem-geproduceerde **Alle publiek** publiek in **de Ontdekking van het publiek *** overlappende analyse is inclusief publiek met alle statussen van de verbindingstoegang (openbaar, privé, douane)."){width="100" zoomable="yes"}

De beschikbaarheid van het publiek voor gebruik in projecten met medewerkers verschilt gebaseerd op het plaatsen van de verbindingstoegang. U kunt de verbindingstoegang altijd wijzigen van privé in openbaar, maar u kunt die instelling niet meer wijzigen als een publiek wordt gedeeld met deelnemers.

### Zichtbaarheid metagegevens {#metadata-visibility}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_view_audience_metadata_visibility"
>title="Zichtbaarheid metagegevens"
>abstract="<p>Geeft aan welke van de metagegevens van de doelgroep zichtbaar is voor andere organisaties voordat deze verbinding maken met uw organisatie. </p> <p> **de telling van de Identiteit** controleert of uw partner identiteitscijfers voor uw publiek kan bekijken wanneer het bekijken van overlappende rapporten in de ontdekking tabel. **het publiek overlapt %** controleert of de medewerkers overlappende percentages tussen hun publiek en van u kunnen ontdekken."

>[!NOTE]
>
>Als voor uw medewerker alle soorten publiek zijn ingesteld op Private, is de weergave **[!UICONTROL Relevant audiences]** in de kijkcijfers leeg. [Meer informatie](/help/guide/collaborate/discover.md#relevant-audiences).

Geeft aan welke van de metagegevens van de doelgroep zichtbaar is voor andere organisaties voordat deze verbinding maken met uw organisatie of binnen verschillende projectweergaven.

**[!UICONTROL Show identity count]**: Dit het plaatsen controleert of uw partner identiteitstellingen voor uw publiek kan bekijken wanneer [ het bekijken overlappende rapporten in de ontdekking tabel ](/help/guide/collaborate/discover.md#discover-overlaps).

![ zij aan zij beelden met de optie van de showidentiteitstelling geschrapt en geselecteerd.](/help/assets/setup/add-manage-audiences/show-identity-count.png)

**[!UICONTROL Show audience overlap %]**: Wanneer geplaatst aan waar, kunnen de medewerkers [ overlappende percentages ](/help/guide/collaborate/discover.md#compare-audiences) tussen hun publiek en het publiek ontdekken dat tot u behoort. In de onderstaande opname heeft het publiek `agora-advertiser-aud3` deze configuratie bijvoorbeeld ingesteld op true en kan een medewerker overlappende percentages weergeven voor dat publiek. Voor het publiek `agora-advertiser-aud1` is deze instelling ingesteld op false, zodat de deelnemer overlappende percentages niet kan weergeven.

![ het percentage van de overlapping van het publiek voor twee verschillende soorten publiek.](/help/assets/setup/add-manage-audiences/audience-overlap-percentage.gif)

## Volgende stappen

Na het invoeren van publiek, gebruik [ verbind ](/help/guide/connect/establishing-connections.md) sectie om uitgevers te ontdekken om met te verbinden en te beginnen aan projecten samen te werken.
