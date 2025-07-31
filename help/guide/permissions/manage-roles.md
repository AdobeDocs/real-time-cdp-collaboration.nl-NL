---
title: Rollen beheren via machtigingen
description: Begrijp alle beschikbare rolmiddelen die toegang tot verschillende componenten binnen Real-Time CDP Collaboration UI verlenen.
audience: admin
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/nl/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 59cf5bf2-421b-4ebc-beab-30eafb098649
source-git-commit: a7215d453021be578a32ce1af4d659845c3b8493
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Rollen beheren {#manage-roles}

{{limited-availability-release-note}}

Om gebruikerstoegang tot verschillende componenten van Adobe Real-Time CDP Collaboration UI te beheren, kan een [ beheerder ](./manage-user-access.md#system-admin-gain-access) rollen bepalen en toewijzen. De rollen bepalen de toegang die een beheerder of een gebruiker [ middelen ](https://experienceleague.adobe.com/nl/docs/experience-platform/access-control/home#permissions){target="_blank"} in uw organisatie moet &lbrace;hebben. Deze gids zal informatie over de standaardrollen verstrekken die in Real-Time CDP Collaboration worden verstrekt, evenals de individuele toestemmingen u die aan douanerollen kunt worden toegewezen.

Om met het beheren van rollen te beginnen, zal een beheerder toegang tot het product van Experience Platform nodig hebben. Voor informatie bij het verkrijgen van administratieve toegang, of bij het verkrijgen van toegang tot Experience Platform, leest [ gebruikerstoegang ](./manage-user-access.md#manage-user-access-through-permissions) gids.

## Standaardrollen {#standard-roles}

Er zijn twee standaardrollen die aan u worden verstrekt die twee gemeenschappelijke gebruiksgevallen van het toegangsbeheer vullen. Dit zijn rollen &quot;alleen-lezen&quot;, wat betekent dat ze niet kunnen worden aangepast.

| Rolnaam | Rolbeschrijving | Machtigingen |
| --- | --- | --- | 
| Collaboration Managers | Dit is all-access toestemming, die alle 15 toestemmingen bevat. Hierdoor kan de gebruiker alle gegevens lezen, maken en bewerken. Het biedt ook toegang tot de **[!UICONTROL Prod]** -sandbox in Experience Platform, zodat u soorten publiek kunt importeren in Real-Time CDP Collaboration. | Alles uit de onderstaande tabel. |
| Collaboration Viewers | Dit is een alleen-lezen toegangsmachtiging. Een gebruiker kan gegevens, activiteiten, verbindingen, en meer lezen en ontdekken. Het biedt ook toegang tot de **[!UICONTROL Prod]** -sandbox in Experience Platform, zodat u soorten publiek kunt importeren in Real-Time CDP Collaboration. | Alle leesmachtigingen uit de onderstaande tabel. |

{style="table-layout:auto"}

## Specifieke toegangsrollen maken {#specific-access-roles}

U zult waarschijnlijk extra rollen willen tot stand brengen om verschillende niveaus van toegang tot verschillende gebruikers te verstrekken. Wanneer u rollen maakt, kunt u verschillende toegangsniveaus beheren door specifieke machtigingen binnen de **[!UICONTROL Collaborations]** -bron te selecteren. Leren om rollen tot stand te brengen en te beheren, verwijs naar de [ rollen ](https://experienceleague.adobe.com/nl/docs/experience-platform/access-control/abac/permissions-ui/roles#create-new-role){target="_blank"} gids.

>[!NOTE]
> Een gebruiker moet toegang hebben tot de **[!UICONTROL Prod]** -sandbox in Adobe Experience Platform om toegang te krijgen tot Collaboration. Als u gebruikers toegang wilt geven tot deze sandbox, moeten ze worden toegewezen aan een rol die de machtiging **[!UICONTROL Prod]** bevat in de **[!UICONTROL Sandboxes]** -bron.

Hieronder ziet u een lijst met beschikbare machtigingen binnen de samenwerkingsbron:

| Machtiging op hoog niveau | Beschrijving |
| --- | --- |
| Collaboration-instanties beheren | De samenwerkingsinstanties van een organisatie weergeven, maken, bijwerken en verwijderen. Ontdek de samenwerkingsinstanties van andere organisaties. |
| Collaboration-instanties lezen | Lees de samenwerkingsinstanties van een organisatie en ontdek de samenwerkingsinstanties van andere organisaties. |
| Verbindingsuitnodigingen beheren | De mening, creeert, en schrapt verbindingsuitnodigingen die door uw organisatie in werking worden gesteld. Accepteer en weiger een verbindingsuitnodiging die is geïnitieerd door andere organisaties. |
| Uitnodigingen voor leesverbinding | Verbindingsuitnodigingen weergeven. |
| Collaboration-verbindingen beheren | Een medewerker kan instellingen weergeven, maken en bijwerken, en verbindingen verzenden en verwijderen. |
| Collaboration-verbindingen lezen | Verbindingen weergeven. |
| Poortgegevens beheren | Aan boord en ontdek publiek. Werk publieke, persoonlijke en aangepaste doelgroepen bij en beheer de metagegevensinstellingen voor de doelinventaris. |
| Gegevens publiek lezen | Lees en ontdek publiek. |
| Metingsgegevens beheren | Metingsgegevens aan boord, bijwerken en verwijderen. |
| Metingsgegevens lezen | Metingsgegevens lezen. |
| Projecten beheren | Projecten weergeven, maken, bijwerken en verwijderen voor de detectie-, activeer- en meetactiviteiten. |
| Projecten lezen | Projecten weergeven voor alle detectie-, activeer- en meetactiviteiten. |
| Gebruikersactiviteiten lezen | Lees gebruikersactiviteiten. |
| Gebruikersactiviteiten exporteren | Gebruikersactiviteiten exporteren. |
| Collaboration-kredietcontrole lezen | Kredietcontrole op organisatorisch en instantieniveau. |

{style="table-layout:auto"}

## Volgende stappen

Na het creëren van rollen die toegang tot Collaboration bepalen, zult u de rollen [ aan beheerders en gebruikers moeten ](./manage-user-access.md#assign-a-role) toewijzen. Verwijs naar [ toestemmingen voor een rol ](https://experienceleague.adobe.com/nl/docs/experience-platform/access-control/abac/permissions-ui/permissions) gids voor een volledig overzicht van het beheren van rollen beheren.
