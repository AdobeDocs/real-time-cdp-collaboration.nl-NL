---
title: Auditlogboeken
description: Leer hoe u de functie Auditlogboeken in Real-Time CDP Collaboration gebruikt om gebruikersactiviteiten en wijzigingen bij te houden.
audience: admin
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3af1ac47-dc3d-4f19-a6b9-9e4e835977c0
source-git-commit: ff22dde9730fab89481338753b1dc4a0adf1d57e
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 1%

---

# Auditlogboeken

{{limited-availability-release-note}}

Om de transparantie en zichtbaarheid van activiteiten die in het systeem worden uitgevoerd te vergroten, kunt u gebruikersactiviteit controleren op verschillende services en mogelijkheden in de vorm van auditlogboeken in Adobe Real-Time Customer Data Platform (CDP). Deze logboeken vormen een audittrail die kan helpen bij het oplossen van problemen in Real-Time CDP Collaboration en uw bedrijf kan helpen effectief te voldoen aan het beleid voor gegevensbeheer van bedrijven en de wettelijke vereisten.

In basale zin vertelt *een auditlogboek wie* welke *actie heeft uitgevoerd* en *wanneer*. Elke actie die in een logboek wordt geregistreerd bevat meta-gegevens die op het actietype, datum en tijd, e-mailidentiteitskaart van de gebruiker die de actie, en extra attributen relevant voor het actietype uitvoerde.

Gebruik de functionaliteit voor auditlogs in Real-Time CDP Collaboration om gebruikersactiviteiten en wijzigingen binnen het platform bij te houden. Deze functie is geïntegreerd met de Adobe Experience Platform-auditservice en de gebruikersinterface voor deze functie bevindt zich in Experience Platform.

![ het overzichtsscherm op hoog niveau van de functionaliteit van controlelogboeken ](/help/assets/setup/audit-logs/audit-logs-overview.png)

Voor uitvoerigere informatie over controlelogboeken, bezoek de [ documentatie van de Logboeken van de Controle van Adobe Experience Platform ](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview).

## Toegangscontrolelogboeken

U kunt controlelogboeken op twee manieren openen, zoals beschreven in de hieronder secties. Beide opties tonen een lijst van controlelogboeken die diverse activiteiten vangen die binnen de UI van Real-Time CDP Collaboration worden uitgevoerd

### Toegang tot auditlogs vanuit de gebruikersinterface van Real-Time CDP Collaboration

1. Navigeer naar het tabblad **[!UICONTROL My Activity]** in de gebruikersinterface van Real-Time CDP Collaboration.
2. Selecteer de Experience Platform-koppeling in de UI-tekst boven aan de pagina.

![ de controlelogboeken van de Toegang van Real-Time CDP Collaboration UI ](/help/assets/setup/audit-logs/access-from-collaboration-ui.png)

### Krijg rechtstreeks toegang tot auditlogboeken in de gebruikersinterface van Experience Platform

1. Navigeer naar de gebruikersinterface van Adobe Experience Platform en selecteer de **[!UICONTROL Audits]** sectie in het menu aan de linkerkant. Neem contact op met de systeembeheerders van uw organisatie om de benodigde machtigingen te verkrijgen als u geen auditlogboeken kunt bekijken.

![Toegang tot auditlogboeken vanuit de gebruikersinterface van Experience Platform](/help/assets/setup/audit-logs/access-from-experience-platform-ui.png)

## Controlelogboeken weergeven en gebruiken

U kunt als volgt de auditlogs weergeven:

1. Navigeer naar de **[!UICONTROL Audits]** sectie in de gebruikersinterface van Adobe Experience Platform.
2. Gebruik de filters om de logboeken te verfijnen op basis van uw criteria.
3. Selecteer een logboekvermelding om gedetailleerde informatie weer te geven, waaronder het tijdstempel, de aanvraag-ID, de resourcedetails en de actiestatus.

![Gedetailleerd auditlogboek](/help/assets/setup/audit-logs/filters-and-detailed-view.png)

### Vastgelegde activiteiten

Auditlogboeken bevatten gedetailleerde informatie over gebruikersactiviteiten, waaronder:

* **identiteitskaart van de Gebruiker**: Het herkenningsteken van de gebruiker die de actie uitvoerde.
* **Actie**: Het type van uitgevoerde actie (b.v., creeer, update, schrap).
* **Middel**: Het middel dat werd gewijzigd of gecreeerd.
* **Tijdstempel**: De tijd toen de actie werd uitgevoerd.

Deze logboeken maken een uitgebreid spoor van alle activiteiten binnen uw Real-Time CDP Collaboration-instantie. Dit is handig voor gegevensbeheer en naleving van regelgeving. Lees meer over [ het leiden controlelogboeken in UI ](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#managing-audit-logs-in-the-ui).

### Controllerlogboeken filteren

De gebruikersinterface van auditlogboeken bevat verschillende filters waarmee u naar specifieke logboeken kunt zoeken:

* **Categorie**: Verwijs naar het middeltype (bijvoorbeeld: samenwerkingsinstantie, verbinding, project).
* **Actie**: Het type van uitgevoerde actie (bijvoorbeeld: creeer, schrap, update).
* **identiteitskaart van het Verzoek**: Een uniek herkenningsteken voor het verzoek.
* **E-mailadres** gebruiker: het e-mailadres van de gebruiker die de actie heeft uitgevoerd.
* **Status**: De status van de actie (bijvoorbeeld: toegestaan, ontkend).
* **de Waaier van de Datum**: De waaier van data waarvoor u logboeken wilt bekijken.

Lees meer over [ het filtreren controlelogboeken ](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#filter-audit-logs).

### Voorbeeldgebruik

De logboeken van de controle worden geproduceerd en getoond in de audits UI van Experience Platform wanneer u acties binnen Real-Time CDP Collaboration UI, zoals het leiden van publiek, het uitbreiden van verbindingsuitnodigingen, het creëren van projecten, etc. uitvoert. Bewerkingen voor het maken of bijwerken van delen van een project worden bijvoorbeeld vastgelegd zoals hieronder wordt weergegeven:

![ Voorbeeld van controlelogboeken die wanneer het creëren van en het bijwerken van delen van een project worden geproduceerd.](/help/assets/setup/audit-logs/create-project-audits.png)

## Voordelen

Begrijp enkele voordelen van het gebruiken van controlelogboeken:

* **Beheer van Gegevens**: De controlelogboeken van het gebruik om ervoor te zorgen dat alle activiteiten binnen het platform worden gevolgd en controleerbaar.
* **Regelgevende Naleving**: De eigenschap verstrekt een spoor van gebruikersactiviteiten om aan regelgevende vereisten te voldoen.
* **het Oplossen van problemen**: De logboeken van de controle helpen in het identificeren van en het oplossen van kwesties door gedetailleerde logboeken van gebruikersacties te verstrekken.

## Referentie categorieën en handelingen

In de onderstaande tabel staan alle categorieën en acties voor Real-Time CDP Collaboration vermeld.

![ Beschikbare die categorieën in de controlelogboeken van Real-Time CDP Collaboration worden benadrukt.](/help/assets/setup/audit-logs/available-categories.png)

| Categorie | Acties | Beschrijving |
|-------------------------------|------------------------------------------|-------------|
| **[!UICONTROL Collaboration Instance]** | Maken, bijwerken, verwijderen | Organisatierekeningen beheren, waaronder het maken, bijwerken en verwijderen van organisaties. Lees meer over [het opzetten van organisaties](/help/guide/setup/onboard-organization.md). |
| **[!UICONTROL Collaboration Connection Invite]** | maken, bijwerken, verwijderen, goedkeuren, afwijzen | Beheer verbindingsuitnodigingen, waaronder het maken, bijwerken, verwijderen, goedkeuren en afwijzen van uitnodigingen. Lees meer over [verbindingsuitnodigingen](/help/guide/connect/establishing-connections.md). |
| **[!UICONTROL Collaboration Connection]** | Maken, bijwerken, verwijderen, goedkeuren, afwijzen, goedkeuring vragen | Beheer samenwerkingsverbindingen, waaronder het maken, bijwerken, verwijderen, goedkeuren, afwijzen en goedkeuren van verbindingen. |
| **[!UICONTROL Collaboration Data Connection]** | Maken, bijwerken, verwijderen | Gegevensverbindingen beheren voor samenwerking om doelgroepen te importeren en te beheren, inclusief het maken, bijwerken en verwijderen van gegevensverbindingen. Lees meer over [het beheren van dataverbindingen](/help/guide/setup/manage-data-connection.md). |
| **[!UICONTROL Collaboration Data Entity]** | maken, bijwerken, verwijderen | Gegevensentiteiten beheren voor samenwerking, waaronder gegevensentiteiten maken, bijwerken en verwijderen. Gegevensentiteiten in deze context verwijzen naar het publiek. Lees meer over [ het invoeren en het leiden van publiek ](/help/guide/setup/onboard-audiences.md). |
| **[!UICONTROL Collaboration Project]** | maken, bijwerken, verwijderen | Projecten beheren in samenwerking, waaronder projecten maken, bijwerken en verwijderen. Lees meer over [ het leiden projecten ](/help/guide/collaborate/manage-projects.md). |
| **[!UICONTROL Collaboration Module]** | maken, bijwerken, verwijderen | Beheer verschillende modules binnen samenwerkingsprojecten, met inbegrip van het creëren van, het bijwerken van, en het schrappen van diverse modules in UI. Bijvoorbeeld, de capaciteit om [ publiek ](/help/guide/collaborate/share.md) te delen. |

{style="table-layout:auto"}

Door gebruik te maken van de functionaliteit voor auditlogs, kunt u een duidelijke en gedetailleerde registratie bijhouden van alle activiteiten binnen uw Real-Time CDP Collaboration-instantie, zodat transparantie en verantwoordingsplicht gewaarborgd zijn.
