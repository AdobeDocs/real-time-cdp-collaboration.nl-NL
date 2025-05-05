---
title: Het berekenen van overlappende tellingen en percentages
description: Begrijp hoe de overlappingen tellen en de percentages in diverse gebieden van Adobe Real-Time CDP Collaboration worden berekend
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/nl/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 23dc33af83366806f7d99161b4b713a33daeec76
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 6%

---


# Het berekenen van overlappende tellingen en percentages

In Adobe Real-Time CDP Collaboration is het van cruciaal belang dat u de overlappingen van het publiek begrijpt voor het optimaliseren van uw marketingstrategieën en het zorgen voor effectieve samenwerking tussen adverteerders en uitgevers. In dit document wordt uitgelegd hoe u het aantal overlappingen en de percentages in de verschillende productgebieden berekent aan de hand van voorbeeldgegevens.

## Voorbeeldgegevens - Aantal identiteiten

### Aannames voor berekeningsdoeleinden

In dit voorbeeld wordt ervan uitgegaan dat:

* De adverteerder heeft drie soorten publiek (A1, A2, A3).
* De uitgever heeft drie soorten publiek (P1, P2, P3).
* Alle overeenkomende sleutelidentiteiten sluiten elkaar uit voor alle doelgroepen.

>[!NOTE]
>
>In werkelijkheid zou er enige overlapping zijn tussen de overeenkomende sleutelidentiteiten van elk publiek, maar om het eenvoudig te houden, gaat dit voorbeeld ervan uit dat ze in dit geval exclusief zijn.

### Advertentiesoorten

| Advertentiesoorten | A1 | A2 | A3 | ALLES |
|----------------------|------|------|------|------|
| Onderbroken e-mailidentiteiten | 300K | 450K | 250K | 1M |
| Id-identiteiten van stempel | 500K | 200K | 700K | 1,4 M |
| Totaal aantal identiteiten | 800K | 650K | 950K | 2,4 M |

### Soorten publiek uitgever

| Soorten publiek uitgever | P1 | P2 | P3 | ALLES |
|---------------------|------|------|------|------|
| Onderbroken e-mailidentiteiten | 150K | 600K | 550K | 1,3 M |
| Id-identiteiten van stempel | 400K | 350K | 100K | 850K |
| Totaal aantal identiteiten | 550K | 950K | 800K | 2,3 M |

## Overlappende tellingen en percentages berekenen

### Voorbeeldgegevens - Aantal overlappingen

#### Adverteerder Elke versus elke uitgever

|                     | A1 - P1 | A2 - P2 | A3 - P3 |
|---------------------|---------|---------|---------|
| Overlappen door onderbroken e-mail | 100K | 300K | 150K |
| Overlappen door liveramp-id | 200K | 150K | 50K |
| Totale overlapping | 300K | 450K | 200K |

#### Adverteerder Elke vs Publisher ALL

|                     | A1 - ALLES | A2 - ALLES | A3 - P ALL |
|---------------------|------------|------------|------------|
| Overlappen door onderbroken e-mail | 250K | 400K | 200K |
| Overlappen door liveramp-id | 350K | 150K | 230K |
| Totale overlapping | 600K | 550K | 430K |

#### Adverteerder ALL vs Publisher Elke

|                     | ALLES - P1 | ALLES - P2 | A ALL - P3 |
|---------------------|------------|------------|------------|
| Overlappen door onderbroken e-mail | 120K | 530K | 200K |
| Overlappen door liveramp-id | 350K | 330K | 50K |
| Totale overlapping | 470K | 860K | 250K |

#### Adverteerder ALL vs Publisher ALL

|                     | ALLES - ALLES PASSEN |
|---------------------|---------------|
| Overlappen door onderbroken e-mail | 850K |
| Overlappen door liveramp-id | 730K |
| Totale overlapping | 1,58 MB |

## Module detecteren

De module **[!UICONTROL Discover]** in Adobe Real-Time CDP Collaboration biedt waardevolle inzichten in uw publieksgegevens. Door publieksoverlap te begrijpen, kunt u potentiële samenwerkingsmogelijkheden tussen uitgevers en adverteerders identificeren. Met de sectie **[!UICONTROL Audience Insights]** in de module **[!UICONTROL Discover]** kunt u de aantallen overlappingen en percentages tussen verschillende soorten publiek analyseren.

![ de ontdekkingsmodule van het samenwerkingswerkschema.](/help/assets/reference/overlap-calculations/discover-module-overlap-calculations.png)

Hieronder vindt u voorbeeldberekeningen en -formules voor verschillende overlappende scenario&#39;s.

### Alle adverteerders en alle uitgeverijen

| Advertentiesoorten | Soorten publiek uitgever | Aantal identiteiten (A) | Overlappende identiteiten (B) | Overlap percentage | Uitsplitsing naar sleutel afstemmen | Uitsplitsing naar sleutel afstemmen % |
|----------------------|---------------------|--------------------|----------------------------|-----------------|---------------------|-----------------------|
| ALLES | ALLES | Totaal aantal identiteitsgegevens van ALLE adverteerders <br> Identiteitstelling = 1M + 1,4M = 2,4M | Totale overlapping tussen ALLE adverteerdersoorten en ALLE uitgeverssoorten voor alle match keys <br> Overlappende identiteiten = 1,58M | Percentage overlappende identiteiten ten opzichte van het totale aantal identiteiten van ALLE adverteerders <br> Overlap % = (B / A) * 100 = (1,58M / 2,4M) * 100 = 65,83% <br> Overlap percentage = 65,83% | Overlappende identiteiten per overeenkomende sleutel <br> Overlappen per gehashte e-mail = 850K <br> Overlappen door liveramp Id = 730K | Percentage overlappende overeenkomende sleutel boven totale overlappende identiteiten <br> Identieke sleutel % voor onderbroken e-mail = (850K / 1,58M) * 100 = 53,8% <br> voor limitatieve id = (730K / 1,58M) * 100 = 46,2% |

### Alle adverteerders en één uitgeverspubliek

| Advertentiesoorten | Soorten publiek uitgever | Aantal identiteiten (A) | Overlappende identiteiten (B) | Overlap percentage | Uitsplitsing naar sleutel afstemmen | Uitsplitsing naar sleutel afstemmen % |
|----------------------|---------------------|--------------------|----------------------------|-----------------|---------------------|-----------------------|
| ALLES | 1 P2 | Totaal aantal identiteitsgegevens van alle adverteerders <br> Identiteitstelling = 1M + 1,4M = 2,4M | Totale overlapping tussen ALLE adverteerders en geselecteerd uitgeverspubliek P2 voor alle overeenkomende sleutels <br> Overlappende identiteiten = 860 K | Percentage overlappende identiteiten ten opzichte van het totale aantal identiteiten van ALLE adverteerders <br> Overlap % = (B / A) * 100 = (860K / 2,4M) * 100 = 35,83% <br> Overlap percentage = 35,83% | Overlappende identiteiten per overeenkomende sleutel <br> Overlappen per gehashte e-mail = 530K <br> Overlappen door liveramp Id = 330K | Percentage overlappende overeenkomende sleutel boven totale overlappende identiteiten <br> Identieke sleutel % voor onderbroken e-mail = (530K / 860K) * 100 = 61,62% <br> voor liveramp Id = (330K / 860K) * 100 = 38,38% |

### Eén adverteerderspubliek en alle uitgeversgebruikers

| Advertentiesoorten | Soorten publiek uitgever | Aantal identiteiten (A) | Overlappende identiteiten (B) | Overlap percentage | Uitsplitsing naar sleutel afstemmen | Uitsplitsing naar sleutel afstemmen % |
|----------------------|---------------------|--------------------|----------------------------|-----------------|---------------------|-----------------------|
| 1 A1 | ALLES | Het totale aantal identiteitsgegevens van het geselecteerde publiek A1 <br> Identiteitskaart = 300K + 500K = 800K | Totale overlapping tussen adverteerderspubliek A1 en ALLE uitgeverspubliek voor alle overeenkomende sleutels <br> Overlappende identiteiten = 600K | Percentage overlappende identiteiten boven identiteitsaantallen van het geselecteerde publiek van adverteerders (A1) <br> Overlap % = (B / A) * 100 = (600K / 800K) * 100 = 75% <br> Overlap percentage = 75% | Overlappende identiteiten per overeenkomende sleutel <br> Overlappen per gehashte e-mail = 250K <br> Overlappen door liveramp Id = 350K | Percentage overlappende overeenkomende sleutel boven totale overlappende identiteiten <br> Identieke sleutel % voor onderbroken e-mail = (250K / 600K) * 100 = 41,67% <br> voor liveramp Id = (350K / 600K) * 100 = 58,33% |

### Eén adverteerder en één uitgeverspubliek

| Advertentiesoorten | Soorten publiek uitgever | Aantal identiteiten (A) | Overlappende identiteiten (B) | Overlap percentage | Uitsplitsing naar sleutel afstemmen | Uitsplitsing naar sleutel afstemmen % |
|----------------------|---------------------|--------------------|----------------------------|-----------------|---------------------|-----------------------|
| 1 A2 | 1 P2 | Het totale aantal identiteitsgegevens van het geselecteerde publiek A2 <br> Identiteitskaart = 450K + 200K = 650K | Totale overlapping tussen geselecteerde adverteerderspubliek A2 en geselecteerd uitgeverspubliek P2 voor alle overeenkomende sleutels <br> Overlappende identiteiten = 450 K | Percentage overlappende identiteiten boven identiteitsaantallen van mijn geselecteerde publiek (A2) <br> Overlap % = (B / A) * 100 = (450K / 650K) * 100 = 69,23% <br> Overlap percentage = 69,23% | Overlappende identiteiten per overeenkomende sleutel <br> Overlappen per gehashte e-mail = 300K <br> Overlappen door liveramp Id = 150K | Percentage overlappende overeenkomende sleutel boven totale overlappende identiteiten <br> Identieke sleutel % voor onderbroken e-mail = (300K / 450K) * 100 = 66,67% <br> voor liveramp Id = (150K / 450K) * 100 = 33,33% |
