---
title: Auditlogboeken
description: Leer hoe u de functie Auditlogboeken in Real-Time CDP Collaboration gebruikt om gebruikersactiviteiten en wijzigingen bij te houden.
audience: admin
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3af1ac47-dc3d-4f19-a6b9-9e4e835977c0
source-git-commit: eed99cfafd5ffad5a468741f7258c162454769b7
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 1%

---

# Auditlogboeken

{{limited-availability-release-note}}

Om de transparantie en zichtbaarheid van de in het systeem uitgevoerde activiteiten te vergroten, kunt u gebruikersactiviteiten voor verschillende services en mogelijkheden controleren in de vorm van auditlogs in Adobe Experience Platform. Deze logboeken vormen een auditspoor dat kan helpen met het oplossen van problemenkwesties in Adobe Real-Time CDP Collaboration, en uw zaken helpen effectief aan het beleid en de regelgevende vereisten van het collectieve gegevensbeheer voldoen.

In een fundamentele betekenis, vertelt een controlelogboek *wie* *uitvoerde wat* actie, en *wanneer*. Elke actie die in een logboek wordt geregistreerd bevat meta-gegevens die op het actietype, datum en tijd, e-mailidentiteitskaart van de gebruiker die de actie, en extra attributen relevant voor het actietype uitvoerde.

Gebruik de functionaliteit voor auditlogs in Collaboration om gebruikersactiviteiten en wijzigingen binnen het platform bij te houden. Deze functie is geïntegreerd met de Experience Platform-auditservice en de gebruikersinterface voor deze functie bevindt zich in Experience Platform.

![ het overzichtsscherm op hoog niveau van de functionaliteit van controlelogboeken.](/help/assets/setup/audit-logs/audit-logs-overview.png)

Voor uitvoerigere informatie over controlelogboeken, bezoek de [ documentatie van de controlelogboeken van Experience Platform ](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview){target="_blank"}.

## Toegangscontrolelogboeken

U kunt controlelogboeken op twee manieren openen, zoals beschreven in de hieronder secties. Beide opties geven een lijst weer met controlelogboeken waarin verschillende activiteiten worden vastgelegd die in Collaboration worden uitgevoerd.

### Toegang tot auditlogs vanuit de gebruikersinterface van Collaboration

1. Navigeer naar de tab **[!UICONTROL My Activity]** in de **[!UICONTROL Setup]** -werkruimte in Collaboration.
2. Selecteer de Experience Platform-koppeling in de tekst boven aan de pagina.

![ de controlelogboeken van de Toegang van het Mijn activiteitenlusje in Collaboration.](/help/assets/setup/audit-logs/access-from-collaboration-ui.png)

### De controlelogboeken van de toegang direct in het gebruikersinterface van Experience Platform

1. Navigeer aan [ Experience Platform ](https://platform.adobe.com/) en selecteer de **[!UICONTROL Audits]** sectie van het linkermenu. Bereik uit aan de systeembeheerders van uw organisatie om de noodzakelijke toestemmingen te verkrijgen als u geen controlelogboeken kunt bekijken.

![ de controlelogboeken van de Toegang van Experience Platform.](/help/assets/setup/audit-logs/access-from-experience-platform-ui.png)

## Controlelogboeken weergeven en gebruiken

U kunt als volgt de auditlogs weergeven:

1. Navigeer naar de sectie **[!UICONTROL Audits]** in Experience Platform.
2. Gebruik de [ filters ](#filter-audit-logs) om de logboeken te versmallen die op uw criteria worden gebaseerd.
3. Selecteer een logbestandvermelding om gedetailleerde informatie weer te geven, zoals de tijdstempel, de aanvraag-id, de brongegevens en de status van de handeling.

![ Gedetailleerd Logboek van de Controle ](/help/assets/setup/audit-logs/filters-and-detailed-view.png)

### Vastgelegde activiteiten

Auditlogboeken bevatten gedetailleerde informatie over gebruikersactiviteiten, waaronder:

* **Tijdstempel**: De nauwkeurige datum en de tijd van de actie die in een maand/dag/jaar wordt uitgevoerd - uur :minute AM/PM formaat.
* **naam van Activa**: De naam van het middel waarop de actie werd uitgevoerd.
* **Categorie**: Het type van middel de actie werd uitgevoerd op.
* **Actie**: De specifieke uitgevoerde actie, zoals creeer of schrap.
* **Gebruiker**: Het e-mailadres van de gebruiker die de actie uitvoerde.

Deze logboeken maken een uitgebreid spoor van alle activiteiten binnen uw Collaboration-instantie. Dit is handig voor gegevensbeheer en naleving van regelgeving. Lees meer over [ het leiden controlelogboeken in UI ](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#managing-audit-logs-in-the-ui).

### Controllerlogboeken filteren {#filter-audit-logs}

De gebruikersinterface van auditlogboeken bevat verschillende filters waarmee u naar specifieke logboeken kunt zoeken:

* **Categorie**: Het type van middel de actie werd uitgevoerd op, zoals de Instantie van Collaboration of Uitnodiging van de Verbinding van Collaboration.
* **Actie**: Het type van uitgevoerde actie. Welke acties beschikbaar zijn, is afhankelijk van de geselecteerde categorie. Acties voor Collaboration Instance omvatten bijvoorbeeld maken, bijwerken en verwijderen.
* **identiteitskaart van het Verzoek**: Een uniek herkenningsteken voor het verzoek.
* **Gebruiker**: Het e-mailadres van de gebruiker die de actie uitvoerde.
* **Status**: De status van de actie, zoals staat toe of ontkent.
* **de Waaier van de Datum**: De waaier van data waarvoor u logboeken wilt bekijken.

Lees meer over [ het filtreren controlelogboeken ](https://experienceleague.adobe.com/en/docs/experience-platform/landing/governance-privacy-security/audit-logs/overview#filter-audit-logs).

## Voordelen

Auditlogboeken bieden verschillende voordelen voor organisaties die Collaboration gebruiken:

* **Beheer van Gegevens**: De controlelogboeken van het gebruik om ervoor te zorgen dat alle activiteiten binnen het platform worden gevolgd en controleerbaar.
* **Regelgevende Naleving**: De eigenschap verstrekt een spoor van gebruikersactiviteiten om aan regelgevende vereisten te voldoen.
* **het Oplossen van problemen**: De logboeken van de controle helpen in het identificeren van en het oplossen van kwesties door gedetailleerde logboeken van gebruikersacties te verstrekken.

## Referentie categorieën en handelingen

In de onderstaande tabel staan alle categorieën en acties voor Real-Time CDP Collaboration vermeld.

![ Beschikbare die categorieën in de controlelogboeken van Real-Time CDP Collaboration worden benadrukt.](/help/assets/setup/audit-logs/available-categories.png)

| Categorie | Acties | Beschrijving |
|-------------------------------|------------------------------------------|-------------|
| **[!UICONTROL Collaboration Instance]** | maken, bijwerken, verwijderen | Accounts beheren, waaronder accounts maken, bijwerken en verwijderen. Om morel te leren, lees [ vormend uw rekeningen ](/help/guide/setup/onboard-account.md) gids. |
| **[!UICONTROL Collaboration Connection Invite]** | maken, bijwerken, verwijderen, goedkeuren, afwijzen | Verbindingsuitnodigingen beheren, waaronder uitnodigingen maken, bijwerken, verwijderen, goedkeuren en afwijzen. Voor meer informatie, lees [ het vestigen van verbindingen ](/help/guide/connect/establishing-connections.md) gids. |
| **[!UICONTROL Collaboration Connection]** | maken, bijwerken, verwijderen, goedkeuren, afwijzen, goedkeuring aanvragen | Verbindingen beheren, waaronder maken, bijwerken, verwijderen, goedkeuren, afwijzen en goedkeuring aanvragen voor verbindingen. |
| **[!UICONTROL Collaboration Data Connection]** | maken, bijwerken, verwijderen | Beheer de gegevensverbindingen vanaf waar u het publiek bront en beheert, inclusief het maken, bijwerken en verwijderen van gegevensverbindingen. Voor meer informatie, lees [ het leiden gegevensverbindingen ](/help/guide/setup/manage-data-connection.md) gids. |
| **[!UICONTROL Collaboration Data Entity]** | maken, bijwerken, verwijderen | Gegevensentiteiten voor Collaboration beheren, zoals gegevensentiteiten maken, bijwerken en verwijderen. Gegevensentiteiten in deze context verwijzen naar het publiek. Voor meer informatie, lees [ het aantrekken en het leiden van publiek ](/help/guide/setup/onboard-audiences.md) gids. |
| **[!UICONTROL Collaboration Project]** | maken, bijwerken, verwijderen | Projecten in Collaboration beheren, waaronder projecten maken, bijwerken en verwijderen. Voor meer informatie, lees de [ het leiden projecten ](/help/guide/collaborate/manage-projects.md) gids. |
| **[!UICONTROL Collaboration Module]** | maken, bijwerken, verwijderen | Beheer verschillende modules binnen projecten, met inbegrip van het creëren van, het bijwerken van, en het schrappen van diverse modules in UI. Bijvoorbeeld, de capaciteit om publiek [ te activeren ](/help/guide/collaborate/activate.md). |

{style="table-layout:auto"}

Door gebruik te maken van de functionaliteit voor auditlogs, kunt u een duidelijke en gedetailleerde registratie bijhouden van alle activiteiten binnen Collaboration, zodat transparantie en verantwoordingsplicht gewaarborgd zijn.
