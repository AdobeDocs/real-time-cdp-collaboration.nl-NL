---
title: Vorm  [!DNL Snowflake]  voor de Bron van het Publiek
description: Leer hoe te om uw  [!DNL Snowflake Secure Data Share]  als zelfbediening gegevensbron te vormen en te verbinden om publieksgegevens in Real-Time CDP Collaboration in te nemen.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/nl/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 517a28afc83b0e1b4a9e64fa53eb90e0ad5541e9
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 0%

---

# [!DNL Snowflake] configureren voor publiekssourcing

Leer hoe u [!DNL Snowflake Secure Data Share] in de gebruikersinterface van Adobe Real-Time CDP Collaboration configureert en koppelt aan brongegevens voor activering en overlappende analyse.

## Overzicht {#overview}

[!DNL Snowflake] is een van de ondersteunde opties voor het aanschaffen van gegevens voor het eerste publiek in Collaboration. Andere beschikbare methodes omvatten het bronpubliek van [&#x200B; Experience Platform &#x200B;](./onboard-audiences.md), verbindend een [[!DNL AWS S3]  emmertje &#x200B;](./configure-aws-s3-audience-sourcing.md), of het uploaden van het dossier van a [&#x200B; CSV &#x200B;](./upload-csv-audience-sourcing.md).

Voer de onderstaande stappen uit om uw [!DNL Snowflake Secure Data Share] aan te sluiten en uw publieksgegevens naar Collaboration te verzenden. Zodra de opstelling volledig is, kunt u, uw afkomstig publiek voor uw samenwerkingsprojecten herzien activeren en beheren.

## Vereisten {#prerequisites}

Voordat u de [!DNL Snowflake] -verbinding configureert, moet u controleren of aan de volgende voorwaarden is voldaan:

* U hebt een [!DNL Snowflake Share] gemaakt en de benodigde machtigingen ingesteld in uw [!DNL Snowflake] -account om Adobe toegang te verlenen tot uw [!DNL Snowflake Secure Data Share] -account.
* U kunt de volgende [!DNL Snowflake Share] -waarden gebruiken:

   * **naam van het Aandeel**
   * **identiteitskaart van de Rekening**
   * **Schema**
   * **Mening**

* De publieksgegevens in uw [!DNL Snowflake Secure Data Share] moeten aan de formaatvereisten voldoen die in de [&#x200B; van de Bron dienst van het Publiek Specificatie (v1.2) &#x200B;](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.2.pdf) gids worden geschetst.
* Alle overeenkomende toetsen in het publieksbestand van [!DNL Snowflake] moeten ook zijn ingeschakeld voor uw Collaboration-account. Leer hoe te [&#x200B; om gelijke sleutels &#x200B;](./onboard-account.md#set-up-match-keys) toe te laten of [&#x200B; nieuwe gelijke sleutels &#x200B;](./onboard-account.md#edit-match-keys) aan uw rekening toe te voegen.

## Uw [!DNL Snowflake] verbinding configureren {#configure-snowflake-connection}

Van het **[!UICONTROL My audiences]** lusje binnen de **[!UICONTROL Setup]** werkruimte, selecteer het add pictogram (![&#x200B; voeg pictogram toe.](/help/assets/icons/plus.png)) en selecteer vervolgens **[!UICONTROL Audience]** .

Als dit uw eerste publiek is, kunt u ook de optie **[!UICONTROL Add audience]** selecteren.

![&#x200B; Mijn publiek tabel in de werkruimte van de Opstelling met toevoegen pictogram en voegt getoonde publieksoptie toe.](../../assets/setup/snowflake-audience-sourcing/add-audience.png)

De workflow voor het toevoegen van publiek wordt weergegeven. Selecteer **[!UICONTROL Add a new data connection]** en selecteer vervolgens **[!UICONTROL Next]** .

![&#x200B; Add publiek werkruimte met Add een nieuwe benadrukte optie van de gegevensverbinding.](../../assets/setup/snowflake-audience-sourcing/add-data-connection.png){zoomable="yes"}

### [!DNL Snowflake] selecteren als gegevensverbinding {#select-snowflake}

Selecteer vervolgens **[!UICONTROL Snowflake]** als gegevensverbinding, gevolgd door **[!UICONTROL Next]** .

![&#x200B; het selectiescherm van de gegevensverbinding met [!DNL Snowflake] beschikbaar als selecteerbare optie.](../../assets/setup/snowflake-audience-sourcing/select-snowflake-data-connection.png)

### Revisiebestand {#review-audience-file}

Er wordt een dialoogvenster weergegeven met uitleg over de vereisten van het doelbestand [!DNL Snowflake Share] en [!DNL Snowflake] voordat u kunt beginnen met het zoeken naar een site. Zorg ervoor dat de [!DNL Snowflake Share] is gemaakt met de juiste naam voor delen, account-id, schema en weergave. Controleer de handleiding van **[[!UICONTROL Audience Sourcing Specification]](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.2.pdf)** om te bevestigen dat de publieksgegevens op de juiste wijze zijn opgemaakt en gestructureerd voor gebruik in Collaboration.

Selecteer **[!UICONTROL Start onboarding]** wanneer u klaar bent.

![&#x200B; bereidt uw [!DNL Snowflake Share] voor op het instappen dialoog met een verbinding aan de Specificaties van de Bron van het Publiek voor.](../../assets/setup/snowflake-audience-sourcing/prepare-snowflake-share-onboarding-dialog.png)

### [!DNL Snowflake Share] -verbinding verifiëren {#authenticate-snowflake-share-connection}

In deze stap moet u de vereiste [!DNL Snowflake Share] -gegevens opgeven om uw [!DNL Snowflake Share] te verbinden met Collaboration:

| Veld | Beschrijving | Voorbeeld |
|--------------------|-------------|------------------------------|
| Naam delen | De naam van de [!DNL Snowflake Share] . | `ADOBE_DATA_SHARE` |
| Account-id | De unieke id van je Snowflake-account. | `CUSTOMER_ORG.CUSTOMER_SNOWFLAKE_ACCOUNT` |
| Schema | Het schema in uw [!DNL Snowflake Share] dat uw publieksgegevens bevat. | `CUSTOMER_SCHEMA` |
| Weergave | De gegevensset die Collaboration in publieksgegevens ophaalt. | `SECURE_VIEW_FOR_ADOBE` |

{style="table-layout:auto"}

Selecteer **[!UICONTROL Next]** nadat u alle vereiste gegevens hebt ingevoerd.

![&#x200B; de [!DNL Snowflake Share] verbindingsvorm met de naam van het Aandeel, de identiteitskaart van de Rekening, het Schema, en de gebieden van de Mening vulde, en de Volgende benadrukte knoop.](../../assets/setup/snowflake-audience-sourcing/snowflake-authentication-credentials-form.png)

Onder aan de volgende pagina wordt een bevestigingsvenster weergegeven waarin wordt bevestigd dat de [!DNL Snowflake Share] -verbinding met Collaboration is gemaakt.

![&#x200B; een bevestigingsdialoog bevestigt uw [!DNL Snowflake Share] verbinding met succes werd gevestigd.](../../assets/setup/snowflake-audience-sourcing/snowflake-share-connection-established.png)

### Naam en beschrijving opgeven {#provide-name-description}

Voer in de weergave **[!UICONTROL Provide details]** een beschrijvende naam en een optionele beschrijving in voor uw [!DNL Snowflake] -gegevensverbinding. Selecteer **[!UICONTROL Next]** als u klaar bent.

![&#x200B; verstrek detailsscherm toont de naam en de beschrijving van de gegevensverbinding, met de Volgende benadrukte knoop.](../../assets/setup/snowflake-audience-sourcing/provide-name-description.png)

### Toewijzingsvelden {#map-fields}

Het scherm **[!UICONTROL Mapping]** is momenteel alleen-lezen. U kunt geen transformaties toevoegen, verwijderen of toepassen. Collaboration brengt automatisch bronidentiteitsgebieden van uw [!DNL Snowflake Share] gegevens aan doelgebieden in kaart die op de **[Specificatie van de Bron van het Publiek (v1.2)](../../assets/quick-start/RTCDP_Collaboration_Audience_Sourcing_Spec_v1.2.pdf)** worden gebaseerd.

Bevestig de toegewezen velden visueel en selecteer **[!UICONTROL Next]** om door te gaan. U kunt ook een voorbeeld van voorbeeldgegevens in de [!DNL Snowflake Share] bekijken met de optie **[!UICONTROL Preview source data]** .

![&#x200B; het gebiedsscherm van de Kaart toont de auto-in kaart gebrachte bron en doelgebieden, met de van de bron Voorproef gegevens en Volgende benadrukte opties.](../../assets/setup/snowflake-audience-sourcing/map-fields-screen.png)

Wanneer u een voorbeeld wilt bekijken, wordt het dialoogvenster **[!UICONTROL [!DNL Snowflake Share] data preview]** weergegeven met een voorbeeldgegevens in tabelindeling. Controleer dit en selecteer vervolgens **[!UICONTROL Close]** .

![[!DNL Snowflake Share] in het dialoogvenster met de voorvertoning van de gegevens worden de voorbeeldgegevens van de gemarkeerde opties [!DNL Snowflake Share] en Sluiten weergegeven. &#x200B;](../../assets/setup/snowflake-audience-sourcing/preview-source-data.png)

<!-- NOTE: Manual mapping will be available in the future. -->
<!-- In the **[!UICONTROL Map fields]** screen, you can use the **[!UICONTROL Source field]** and **[!UICONTROL Target field]** dropdowns to update the auto-mapped fields, or include additional fields with the **[!UICONTROL Add field]** option. Once finished, select **[!UICONTROL Next]**. -->

<!-- ![The Map fields screen showing the mapped fields with the Next option highlighted.](../../assets/setup/snowflake-audience-sourcing/map-fields.png) -->

### Vernieuwingsfrequentie en datumbereik plannen {#refresh-frequency-date-range}

Gebruik vervolgens in de **[!UICONTROL Schedule]** -weergave het vervolgkeuzemenu om de vernieuwingsfrequentie tussen een en zes dagen te selecteren. Gebruik vervolgens het kalenderpictogram om de begin- en einddatum voor de doelgroep op te geven.

>[!IMPORTANT]
>
>Als u uw Collaboration-credits effectief wilt beheren, stelt u de vernieuwingsfrequentie in zodat deze overeenkomt met de updatefrequentie van de onderliggende [!DNL Snowflake] -gegevens of deze niet overschrijdt. Het minimaal ondersteunde vernieuwingsinterval is één keer per zes dagen.

![&#x200B; het scherm van het Programma benadrukt vernieuwt frequentie en de configuraties van de datumwaaier, en de Volgende optie.](../../assets/setup/snowflake-audience-sourcing/refresh-frequency-date-range.png)

### De verbinding controleren en voltooien {#review-and-complete}

Tot slot herzie uw configuratiemontages in het summiere scherm. Deze weergave bevat een overzicht van de volgende secties:

* **[!UICONTROL Data connection]**: geeft de naam, de account-id, het schema en de weergave van uw [!DNL Snowflake Share] weer.
* **[!UICONTROL Details]**: geeft de naam en de optionele beschrijving van uw gegevensverbinding weer, zodat u deze later kunt herkennen.
* **[!UICONTROL Mapping]**: geeft aan hoe de bronvelden van het bestand voor uw publiek worden toegewezen aan doelvelden die in Collaboration worden gebruikt.
* **[!UICONTROL Schedule]**: geeft aan hoe vaak de verbinding de publieksgegevens en het actieve datumbereik voor de sourcing vernieuwt.

Selecteer het potloodpictogram (![&#x200B; geef pictogram &#x200B;](/help/assets/icons/edit.png) uit) als u een sectie moet uitgeven. Selecteer **[!UICONTROL Complete]** om alle secties te bevestigen.

![&#x200B; het schermvertoningen van het Overzicht een samenvatting van gegevensverbinding, details, afbeelding en planningsmontages, met de Volledige benadrukte optie.](../../assets/setup/snowflake-audience-sourcing/review-settings.png)

Een bevestigingsdialoogvenster bevestigt dat de gegevensverbinding is gemaakt en dat de doelgroep bezig is met het zoeken naar een verbinding.

## Bronpubliek bekijken {#review-sourced-audiences}

Nadat de installatie is voltooid, begint Collaboration publiek te betrekken van uw [!DNL Snowflake Share] . Als het publiek bezig is met het aanschaffen van een advertentie, wordt een banner boven aan de weergave weergegeven.

![&#x200B; Mijn publieklusje toont het Publiek dat in vooruitlopende banner.](../../assets/setup/snowflake-audience-sourcing/audience-sourcing-in-progress.png)

>[!TIP]
>
>De brontijd van het publiek varieert op basis van de grootte van uw [!DNL Snowflake] gegevens en de vernieuwingsfrequentie die u hebt geconfigureerd. De grotere datasets of minder vaak verfrissen programma&#39;s kunnen langer duren om in de **[!UICONTROL My audiences]** werkruimte te verschijnen.

Wanneer de bron is voltooid, zijn op het tabblad **[!UICONTROL My Audiences]** uw doelgroepen beschikbaar met dezelfde functies en informatie als die van Experience Platform.

![&#x200B; Mijn publiek tabel toont een lijst van bronpubliek in tabelvorm mening.](../../assets/setup/snowflake-audience-sourcing/snowflake-audience-list.png)

Selecteer in de rasterweergave of tabelweergave een rij-item of **[!UICONTROL View audience]** om een overzicht van een specifiek publiek weer te geven. De status, bron en naam van de gegevensverbinding van het publiek worden weergegeven, samen met gedetailleerde deelvensters voor **[!UICONTROL Identities]** , **[!UICONTROL Categories]** , **[!UICONTROL Connection access]** en **[!UICONTROL Metadata visibility]** . Zie [&#x200B; hoe te om een individueel publiek &#x200B;](./onboard-audiences.md#view-individual-audiences) voor details te bekijken.

Gebruik deze mening om publieksconfiguratie en zichtbaarheidsmontages te bevestigen alvorens het publiek in samenwerkingsprojecten te gebruiken.

## De [!DNL Snowflake] gegevensverbinding weergeven {#view-snowflake-connection}

De zojuist toegevoegde [!DNL Snowflake] verbinding is direct beschikbaar op het tabblad **[!UICONTROL My data connections]** . De publieksbron wordt weergegeven als [!UICONTROL [!DNL Snowflake]] .

Uw [!DNL Snowflake] gegevensverbinding bevat dezelfde functionaliteit en details als andere publieksgegevensverbindingen. Leer meer over [&#x200B; om gegevensverbindingen &#x200B;](../setup/manage-data-connection.md) te bekijken en te beheren.

![&#x200B; het Mijn lusje van gegevensverbindingen toont de [!DNL Snowflake] gegevensverbinding met het bron van statusinformatie.](../../assets/setup/snowflake-audience-sourcing/data-connection-tab-snowflake.png)

## Volgende stappen {#next-steps}

U hebt de [!DNL Snowflake] nu geconfigureerd en verbonden als gegevensbron in Collaboration. Na het betrekken voltooit, kunt u [&#x200B; samenwerkingsprojecten &#x200B;](../collaborate/manage-projects.md) tot stand brengen, [&#x200B; publiek &#x200B;](../collaborate/activate.md) activeren, [&#x200B; overzicht overlapt en inzichten &#x200B;](../collaborate/measure.md), en [&#x200B; beheert uw publieksmontages en zicht &#x200B;](./onboard-audiences.md).

Raadpleeg de volgende documentatie voor informatie over andere methoden voor publiekssourcing:

* [Vorm  [!DNL Amazon S3]  voor publieksbron](./configure-aws-s3-audience-sourcing.md)
* [Source-publiek uit Experience Platform](./onboard-audiences.md)
* [CSV-bestand uploaden om publiek te bereiken](./upload-csv-audience-sourcing.md)
