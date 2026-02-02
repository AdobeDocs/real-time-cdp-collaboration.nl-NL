---
title: CSV-bestand uploaden voor audiobronnen
description: Leer hoe u uw CSV-bestand uploadt als bron voor zelfbediening voor het opnemen van publieksgegevens in Real-Time CDP Collaboration.
source-git-commit: 96d3f87cedcfde73ce01c2b53c0b2ce4365fd277
workflow-type: tm+mt
source-wordcount: '1033'
ht-degree: 0%

---

# CSV-bestand uploaden om publiek te bereiken

Deze gids verstrekt stappen om een Csv- dossier in Adobe Real-Time CDP Collaboration UI te uploaden om uw publieksgegevens voor gebruik in samenwerkingsprojecten te bron.

## Overzicht {#overview}

Het CSV- dossier uploadt is één methode aan bron de gegevens van het eerste publiek voor samenwerkingsprojecten. Dit is een alternatief aan [&#x200B; verbindend uw AWS S3 emmertje &#x200B;](./configure-aws-s3-audience-sourcing.md) of [&#x200B; die publiek van Experience Platform &#x200B;](./onboard-audiences.md) betrekken.

Volg deze workflow om een CSV-bestand met uw publieksgegevens te uploaden naar het eerste publiek in Collaboration en deze te beheren. U kunt identiteitsgebieden voor activering en overlappende analyse in kaart brengen. Nadat het bestand is geüpload en verwerkt, wordt het publiek in de bron beschikbaar in de **[!UICONTROL My audiences]** -werkruimte, waar u het bestand kunt bekijken, activeren en beheren voor uw samenwerkingsprojecten.

>[!IMPORTANT]
>
>* Het publiek dat door Csv uploadt wordt betrokken is beschikbaar voor **7 dagen**. Na deze periode, verloopt het publiek en moet voor gebruik in uw samenwerkingsprojecten opnieuw worden geupload.
>
>* U kunt per sessie één CSV-bestand uploaden. Als u meer soorten publiek wilt toevoegen, voltooit u de uploadworkflow opnieuw voor elk bestand dat u wilt bron.

## Vereisten {#prerequisites}

Voordat u CSV-bestanden kunt uploaden voor het zoeken naar publiek, moet u controleren of:

* Betaalde account aan boord in Real-Time CDP Collaboration. Zie [&#x200B; aan boord uw rekening &#x200B;](./onboard-account.md) voor geleidelijke instructies.
* De noodzakelijke toestemmingen om publiek in uw organisatie toe te voegen.
* Een CSV-bestand dat uw publieksgegevens bevat met identiteitsvelden zoals e-mail of telefoon.

## Een CSV-bestand uploaden {#upload-csv-file}

Van het **[!UICONTROL My audiences]** lusje binnen de **[!UICONTROL Setup]** werkruimte, selecteer het add pictogram (![&#x200B; voeg pictogram toe.](/help/assets/icons/plus.png) ) en selecteer vervolgens **[!UICONTROL Audience]** .

Als dit uw eerste publiek is, kunt u ook de optie **[!UICONTROL Add]** selecteren.

![&#x200B; Mijn publiek tabel in de werkruimte van de Opstelling met toevoegen pictogram en voegt getoonde publieksoptie toe.](../../assets/setup/add-manage-audiences/add-audiences.png)

De workflow voor het toevoegen van publiek wordt weergegeven. Selecteer **[!UICONTROL Add a new data connection]** en selecteer vervolgens **[!UICONTROL Next]** .

![&#x200B; Add publiek werkruimte met Add een nieuwe benadrukte optie van de gegevensverbinding.](../../assets/setup/add-manage-audiences/add-data-connection.png){zoomable="yes"}

### CSV-bestand selecteren als gegevensverbinding {#select-csv-file}

Selecteer **[!UICONTROL CSV File]** als gegevensverbinding, gevolgd door **[!UICONTROL Next]** .

![&#x200B; het selectiescherm van de gegevensverbinding met Csv- Dossier beschikbaar als selecteerbare optie.](../../assets/setup/csv-audience-sourcing/select-csv-data-connection.png)

### Bestand selecteren {#select-file}

Kies **[!UICONTROL Select from computer]** om een CSV-bestand van uw lokale systeem te uploaden. U kunt ook het CSV-bestand dat u wilt uploaden naar het deelvenster [!UICONTROL Drag and drop a CSV file] slepen.

>[!IMPORTANT]
>
>Alleen CSV-bestanden worden ondersteund. De maximumdossiergrootte is **2 GB**.

![&#x200B; selecteer een Csv- dossier dat publieksgegevens van uw lokaal systeem bevat.](../../assets/setup/csv-audience-sourcing/select-file.png)

Zodra geüpload, toont UI een samenvatting met inbegrip van het aantal kolommen, een geschat rijaantal, de structuur van het dossier, en een voorproef van de eerste 10 rijen van gegevens.

Controleer het overzicht en selecteer vervolgens **[!UICONTROL Next]** .

![&#x200B; voorproef de gegevens van het steekproefpubliek van uw Csv- dossier.](../../assets/setup/csv-audience-sourcing/preview-sample-data.png)

#### Bestand vervangen {#replace-file}

Als u een ander CSV-bestand moet uploaden, kiest u **[!UICONTROL Replace file]** en selecteert u het nieuwe bestand. De interface verfrist zich dan om een bijgewerkt overzicht van de nieuwe gegevens te tonen.

Selecteer **[!UICONTROL Next]** nadat u de gereviseerde samenvatting hebt bekeken.

![&#x200B; selecteer de Replace dossieroptie om een verschillend Csv- dossier te uploaden.](../../assets/setup/csv-audience-sourcing/replace-file.png)

### Bevestig bevestiging van toestemming {#confirm-consent}

Voordat u verdergaat, moet u erkennen dat de optie om te weigeren toestemming te geven is verwijderd uit uw publieksgegevens. Collaboration vereist schone publieksgegevens zonder gebruikers die ervoor hebben gekozen geen gegevens te delen.

Schakel het bevestigingsvak, gevolgd door **[!UICONTROL OK]** , in om te bevestigen. Vervolgens wordt het dialoogvenster gesloten en gaat u door naar het scherm kaartvelden.

![&#x200B; de dialoog van de toestemmings opt-out erkenning die bevestiging vereist alvorens te werk te gaan.](../../assets/setup/csv-audience-sourcing/consent-optout-acknowledgment.png)

### Identiteitsvelden bron toewijzen {#map-fields}

De afbeelding van het gebied bepaalt hoe Collaboration uw publieksgegevens voor activering en overlappende analyse gebruikt. Gebruik in het scherm **[!UICONTROL Map fields]** de vervolgkeuzemenu&#39;s om elk bronidentiteitsveld van uw CSV-bestand toe te wijzen aan het desbetreffende doelveld in Collaboration.

Als u aanvullende details over een doelveld nodig hebt, zoals het gegevenstype of de beschrijving, selecteert u **[!UICONTROL Target fields details]** voor meer informatie.

![&#x200B; dropdown om een gebied van de bronidentiteit van uw Csv- publieksgegevens aan het doelgebied in Collaboration in kaart te brengen.](../../assets/setup/csv-audience-sourcing/map-fields.png)

Controleer vervolgens de toegewezen velden en selecteer **[!UICONTROL Next]** .

![&#x200B; het scherm van de gebiedstoewijzing dat de in kaart gebrachte bron en gebieden van de doelidentiteit toont.](../../assets/setup/csv-audience-sourcing/confirm-mapped-fields.png)

### Het uploaden controleren en voltooien {#review-and-complete}

Het scherm **[!UICONTROL Review]** wordt weergegeven met een overzicht van de publieksinstellingen uit het CSV-bestand. Bekijk de informatie in de volgende secties:

* **[!UICONTROL File Information]**: geeft de bestandsnaam, het aantal kolommen en het geschatte aantal rijen weer.
* **[!UICONTROL Mapping]**: geeft aan hoe de bronvelden uit het geüploade publieksbestand (bijvoorbeeld `email` ) worden toegewezen aan doelvelden die worden gebruikt in Collaboration (bijvoorbeeld email met hashing).

Selecteer het potloodpictogram als u een sectie wilt bewerken. Selecteer **[!UICONTROL Complete]** om alle secties te bevestigen.

![&#x200B; herzie de samenvatting van uploadt montages met inbegrip van Csv- dossierinformatie en gebiedstoewijzingsdetails.](../../assets/setup/csv-audience-sourcing/review-upload-summary.png)

Onder de overzichtsgedeelten wordt een voortgangsbalk weergegeven om de voortgang van het uploaden aan te geven. Nadat het uploaden is voltooid, wordt in een bevestigingsvenster bevestigd dat het CSV-publiek is gemaakt en dat de doelgroep bezig is met het zoeken naar een site.

![&#x200B; na het uploaden van dossier, verschijnt een bevestigingsdialoog verklarend dat het publiek CSV werd gecreeerd en publiek die lopend.](../../assets/setup/csv-audience-sourcing/upload-success-sourcing-in-progress.png)

## Bronpubliek bekijken {#review-sourced-audiences}

Nadat u het CSV-bestand hebt geüpload, begint Collaboration het publiek van het bestand te betrekken. Dit kan enige minuten duren. Wanneer de bron is voltooid, zijn op het tabblad **[!UICONTROL My Audiences]** uw doelgroepen beschikbaar met dezelfde functies en informatie als die van Experience Platform.

![&#x200B; het lusje van het publiek dat een lijst van afkomstig publiek in netmening toont.](../../assets/setup/csv-audience-sourcing/csv-audiences-list.png)

Selecteer in de rasterweergave of tabelweergave een rij-item of **[!UICONTROL View audience]** om een overzicht van een specifiek publiek weer te geven. De status, bron en naam van de gegevensverbinding van het publiek worden weergegeven, samen met gedetailleerde deelvensters voor:

**[!UICONTROL Identities]**: geeft het totale aantal identiteiten en de totale uitsplitsing weer zodra er gegevens beschikbaar zijn.
**[!UICONTROL Categories]**: geeft alle tags weer die worden gebruikt voor het organiseren of filteren van het publiek.
**[!UICONTROL Connection access]**: geeft aan of het publiek privé, openbaar of gedeeld is met specifieke medewerkers.
**[!UICONTROL Metadata visibility]**: geeft aan welke publieksinformatie (zoals het aantal identiteiten, het overlappingspercentage en de index) zichtbaar is voor deelnemers.

Gebruik deze mening om publieksconfiguratie en zichtbaarheidsmontages te bevestigen alvorens het publiek in samenwerkingsprojecten te gebruiken. Voor meer informatie, zie [&#x200B; hoe te om een individueel publiek &#x200B;](./onboard-audiences.md#view-individual-audiences) te bekijken.

## Volgende stappen {#next-steps}

U hebt uw CSV-bestand nu geüpload in Collaboration. Nadat de bron is voltooid, kunt u:

* Maak samenwerkingsprojecten met uw publiek. Zie [&#x200B; publiek &#x200B;](../../guide/collaborate/discover.md) ontdekken.
* Activeer publiek aan verbonden bestemmingen. Zie [&#x200B; publiek &#x200B;](../../guide/collaborate/activate.md) activeren.
* Bekijk overlappingen en inzichten van het publiek. Zie [&#x200B; campagneprestaties van de Maatregel &#x200B;](../../guide/collaborate/measure.md).
* Beheer uw publieksinstellingen en zichtbaarheid. Zie [&#x200B; Source en beheer publiek &#x200B;](./onboard-audiences.md).

Voor informatie over andere publiek die methodes, zie [&#x200B; AWS S3 voor publiek vormen die &#x200B;](./configure-aws-s3-audience-sourcing.md) of [&#x200B; het publiek van Source van Experience Platform &#x200B;](./onboard-audiences.md) aantrekken.
