---
title: Auditlogboeken
description: Leer hoe u de functie Auditlogboeken in Real-Time CDP Collaboration gebruikt om gebruikersactiviteiten en wijzigingen bij te houden.
audience: admin
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/nl/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3af1ac47-dc3d-4f19-a6b9-9e4e835977c0
source-git-commit: dd1386f9371cb40285315d11e07b139d3115e147
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 1%

---

# Auditlogboeken

{{limited-availability-release-note}}

Om de transparantie en de zichtbaarheid van de in het systeem uitgevoerde activiteiten te vergroten, kunt u gebruikersactiviteiten voor verschillende services en mogelijkheden controleren in de vorm van auditlogs in Adobe Real-Time Customer Data Platform (CDP). Deze logboeken vormen een auditspoor dat kan helpen met het oplossen van problemenkwesties in Real-Time CDP Collaboration, en uw zaken helpen effectief aan het beleid en de regelgevende vereisten van het collectieve gegevensbeheer voldoen.

In een fundamentele betekenis, vertelt een controlelogboek *wie* *uitvoerde wat* actie, en *wanneer*. Elke actie die in een logboek wordt geregistreerd bevat meta-gegevens die op het actietype, datum en tijd, e-mailidentiteitskaart van de gebruiker die de actie, en extra attributen relevant voor het actietype uitvoerde.

Gebruik de functionaliteit voor auditlogs in Real-Time CDP Collaboration om gebruikersactiviteiten en wijzigingen binnen het platform bij te houden. Deze functie is geïntegreerd met de Adobe Experience Platform-auditservice en de gebruikersinterface voor deze functie bevindt zich in Experience Platform.

![ het overzichtsscherm op hoog niveau van de functionaliteit van controlelogboeken ](/help/assets/setup/audit-logs/audit-logs-overview.png)

Voor uitvoerigere informatie over controlelogboeken, bezoek de [ documentatie van de Logboeken van de Controle van Adobe Experience Platform ](https://experienceleague.adobe.com/nl/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview){target="_blank"}.

## Toegangscontrolelogboeken

U kunt controlelogboeken op twee manieren openen, zoals beschreven in de hieronder secties. Beide opties tonen een lijst van controlelogboeken die diverse activiteiten vangen die binnen de UI van Real-Time CDP Collaboration worden uitgevoerd

### Toegang tot auditlogs vanuit de gebruikersinterface van Real-Time CDP Collaboration

1. Navigeer naar het tabblad **[!UICONTROL My Activity]** in de gebruikersinterface van Real-Time CDP Collaboration.
2. Selecteer de Experience Platform-koppeling in de UI-tekst boven aan de pagina.

![ de controlelogboeken van de Toegang van Real-Time CDP Collaboration UI ](/help/assets/setup/audit-logs/access-from-collaboration-ui.png)

### De controlelogboeken van de toegang direct in het gebruikersinterface van Experience Platform

1. Navigeer naar de gebruikersinterface van Adobe Experience Platform en selecteer de sectie **[!UICONTROL Audits]** in het linkermenu. Bereik uit aan de systeembeheerders van uw organisatie om de noodzakelijke toestemmingen te verkrijgen als u geen controlelogboeken kunt bekijken.

![ de controlelogboeken van de Toegang van Experience Platform UI ](/help/assets/setup/audit-logs/access-from-experience-platform-ui.png)

## Controlelogboeken weergeven en gebruiken

U kunt als volgt de auditlogs weergeven:

1. Navigeer naar de sectie **[!UICONTROL Audits]** in de gebruikersinterface van Adobe Experience Platform.
2. Gebruik de filters om de logbestanden te verkleinen op basis van uw criteria.
3. Selecteer een logbestandvermelding om gedetailleerde informatie weer te geven, zoals de tijdstempel, de aanvraag-id, de brongegevens en de status van de handeling.

![ Gedetailleerd Logboek van de Controle ](/help/assets/setup/audit-logs/filters-and-detailed-view.png)

### Vastgelegde activiteiten

Auditlogboeken bevatten gedetailleerde informatie over gebruikersactiviteiten, waaronder:

* **identiteitskaart van de Gebruiker**: Het herkenningsteken van de gebruiker die de actie uitvoerde.
* **Actie**: Het type van uitgevoerde actie (b.v., creeer, update, schrap).
* **Middel**: Het middel dat werd gewijzigd of gecreeerd.
* **Tijdstempel**: De tijd toen de actie werd uitgevoerd.

Deze logboeken maken een uitgebreid spoor van alle activiteiten binnen uw Real-Time CDP Collaboration-instantie. Dit is handig voor gegevensbeheer en naleving van regelgeving. Lees meer over [ het leiden controlelogboeken in UI ](https://experienceleague.adobe.com/nl/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#managing-audit-logs-in-the-ui).

### Controllerlogboeken filteren

De gebruikersinterface van auditlogboeken bevat verschillende filters waarmee u naar specifieke logboeken kunt zoeken:

* **Categorie**: Verwijs naar het middeltype (bijvoorbeeld: samenwerkingsinstantie, verbinding, project).
* **Actie**: Het type van uitgevoerde actie (bijvoorbeeld: creeer, schrap, update).
* **identiteitskaart van het Verzoek**: Een uniek herkenningsteken voor het verzoek.
* **E-mail van de Gebruiker**: Het e-mailadres van de gebruiker die de actie uitvoerde.
* **Status**: De status van de actie (bijvoorbeeld: toegestaan, ontkend).
* **de Waaier van de Datum**: De waaier van data waarvoor u logboeken wilt bekijken.

Lees meer over [ het filtreren controlelogboeken ](https://experienceleague.adobe.com/nl/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#filter-audit-logs).

### Voorbeeldgebruik

De logboeken van de controle worden geproduceerd en getoond in de audits UI van Experience Platform wanneer u acties binnen Real-Time CDP Collaboration UI, zoals het leiden van publiek, het uitbreiden van verbindingsuitnodigingen, het creëren van projecten, etc. uitvoert. Bijvoorbeeld, worden de verrichtingen om delen van een project tot stand te brengen of bij te werken gevangen zoals hieronder getoond:

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
| **[!UICONTROL Collaboration Instance]** | maken, bijwerken, verwijderen | Organisatierekeningen beheren, waaronder het maken, bijwerken en verwijderen van organisaties. Lees meer over [ vestiging organisaties ](/help/guide/setup/onboard-organization.md). |
| **[!UICONTROL Collaboration Connection Invite]** | maken, bijwerken, verwijderen, goedkeuren, afwijzen | Verbindingsuitnodigingen beheren, waaronder uitnodigingen maken, bijwerken, verwijderen, goedkeuren en afwijzen. Lees meer over [ verbinding uitnodigt ](/help/guide/connect/establishing-connections.md). |
| **[!UICONTROL Collaboration Connection]** | maken, bijwerken, verwijderen, goedkeuren, afwijzen, goedkeuring aanvragen | Beheer samenwerkingsverbindingen, waaronder het maken, bijwerken, verwijderen, goedkeuren, afwijzen en aanvragen van goedkeuring voor verbindingen. |
| **[!UICONTROL Collaboration Data Connection]** | maken, bijwerken, verwijderen | Gegevensverbindingen beheren voor samenwerking bij het importeren en beheren van soorten publiek, zoals het maken, bijwerken en verwijderen van gegevensverbindingen. Lees meer over [ het beheren van gegevensverbindingen ](/help/guide/setup/manage-data-connection.md). |
| **[!UICONTROL Collaboration Data Entity]** | maken, bijwerken, verwijderen | Gegevensentiteiten beheren voor samenwerking, waaronder gegevensentiteiten maken, bijwerken en verwijderen. Gegevensentiteiten in deze context verwijzen naar het publiek. Lees meer over [ het invoeren en het leiden van publiek ](/help/guide/setup/onboard-audiences.md). |
| **[!UICONTROL Collaboration Project]** | maken, bijwerken, verwijderen | Projecten beheren in samenwerking, waaronder projecten maken, bijwerken en verwijderen. Lees meer over [ het leiden projecten ](/help/guide/collaborate/manage-projects.md). |
| **[!UICONTROL Collaboration Module]** | maken, bijwerken, verwijderen | Beheer verschillende modules binnen samenwerkingsprojecten, met inbegrip van het creëren van, het bijwerken van, en het schrappen van diverse modules in UI. Bijvoorbeeld, de capaciteit om [ publiek ](/help/guide/collaborate/share.md) te delen. |

{style="table-layout:auto"}

Door gebruik te maken van de functionaliteit voor auditlogs, kunt u een duidelijke en gedetailleerde registratie bijhouden van alle activiteiten binnen uw Real-Time CDP Collaboration-instantie, zodat transparantie en verantwoordingsplicht gewaarborgd zijn.
