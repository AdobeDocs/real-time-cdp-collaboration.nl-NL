---
title: Amazon Marketing Cloud
description: Meer informatie over samenwerken met Amazon Marketing Cloud in Real-Time CDP Collaboration.
audience: publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
source-git-commit: 57b847c25edbf88f4708bda74be41fe6141472a7
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Amazon Marketing Cloud

{{limited-availability-release-note}}

Na het vormen van een verbinding met [!DNL Amazon Marketing Cloud] ([!DNL AMC]), kunnen de adverteerders [ een project ](../manage-projects.md#create-project) tot stand brengen om met [!DNL AMC] samen te werken aan hefboomwerking zijn geavanceerde analytische mogelijkheden. Nadat u een project hebt gemaakt, kunt u de sectie **[!UICONTROL Discover]** gebruiken om publieksinzichten te vergelijken en relevante doelgroepen voor uw campagnes te ontdekken.

>[!IMPORTANT]
>
>De enige gebruiksgevallen die met [!DNL AMC] worden gesteund zijn **ontdekking van het publiek** en **Meting**. Momenteel is alleen de sectie **[!UICONTROL Discover]** beschikbaar in uw project met [!DNL AMC] .

## Discover {#discover}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_compare_audiences"
>title="Soorten publiek vergelijken"
>abstract="Vergelijk je publiek met alle consumenten die je Amazon Ads bereikt."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_relevant_audiences"
>title="Relevant publiek"
>abstract="Amazon-doelsegmenten die uw publiek het hoogst overlapt, waarbij alleen DSP-indrukkingen in aanmerking worden genomen (deze segmenten kunnen alleen worden gericht in de DSP)."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_resolved_ids"
>title="Opgeloste id&#39;s"
>abstract="Het aantal ID&#39;s dat Amazon kan oplossen met behulp van uw publieksgegevens."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_overlapping_ad_exposed_ids"
>title="Overlappende en belichte id&#39;s"
>abstract="Dit staat voor het aantal &#39;Opgeloste id&#39;s&#39; van het geüploade publiek dat ook via Amazon Ads aan een advertentie is blootgesteld."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_overlap_percentage"
>title="Overlappen %"
>abstract="Het percentage &quot;Opgeloste id&#39;s&quot; dat via Amazon Ads aan een advertentie is blootgesteld."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_amc_discover_amazon_breakdown"
>title="Uitsplitsing naar Amazon en product"
>abstract="Uitsplitsing van &quot;Overlappende en belichte id&#39;s&quot; bereikt door Amazon Ads Sponsored Product en/of Amazon Ads DSP."

In de sectie **[!UICONTROL Discover]** kunt u uw AMC-publiek vergelijken met alle consumenten die worden bereikt door uw Amazon Ads. U kunt ook Amazon-doelsegmenten voor uw publiek bekijken met de meeste overlappingen, waarbij u alleen DSP-indrukken in aanmerking neemt (deze segmenten kunnen alleen in de DSP worden geactiveerd).

>[!IMPORTANT]
>
>De gegevens van het publiek worden verwerkt vanuit het publiek dat naar uw [!DNL Amazon Ads] -account is geüpload. Leren hoe de eigenschap van de Doelen van gebruiksExperience Platform om uw publiek naar uw [!DNL Amazon Ads] rekening te verzenden, lees de [ verbinding van de Advertentie van Amazon ](https://experienceleague.adobe.com/en/docs/experience-platform/destinations/catalog/advertising/amazon-ads) gids.

![ ontdekt sectie in een project met Amazon Marketing Cloud.](/help/assets/collaborate/advertising-platforms/amc-discover.png){zoomable="yes"}

### Soorten publiek vergelijken {#compare-audiences}

In de sectie **[!UICONTROL Compare audiences]** vindt u inzichten in de manier waarop uw [!DNL AMC] -publiek overlapt met de gebruikers die door de Amazon Ads worden bereikt. In de sectie **[!UICONTROL Compare audiences]** kunt u de volgende cijfers weergeven:

| Metrisch | Beschrijving |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL Resolved IDs] | Het aantal id&#39;s dat [!DNL Amazon’s Identity Resolution] heeft kunnen oplossen met behulp van uw publieksgegevens. |
| [!UICONTROL Overlapping ad exposed IDs] | Het aantal [!UICONTROL Resolved IDs] van het geüploade publiek dat ook via [!DNL Amazon Ads] aan een advertentie is blootgesteld. |
| [!UICONTROL Overlap %] | Het aandeel van [!UICONTROL Resolved IDs] dat via [!DNL Amazon Ads] aan een advertentie is blootgesteld. |
| [!UICONTROL Breakdown by Amazon ad product] | Uitsplitsing van [!UICONTROL Overlapping ad exposed IDs] bereikt door [!UICONTROL Sponsored Product] en/of [!UICONTROL DSP] . Elke id wordt weergegeven als een individueel percentage van het totale aantal blootgestelde id&#39;s. Aangezien een id tot zowel [!UICONTROL Sponsored Products] als [!UICONTROL DSP] kan behoren, bedragen de percentages mogelijk niet 100%. |


### Relevant publiek {#relevant-audiences}

De sectie **[!UICONTROL Relevant audiences]** biedt inzicht in [!DNL Amazon] doelsegmenten, of soorten publiek, waarmee uw publiek de meeste overlappingen heeft, waarbij alleen DSP-indrukkingen in aanmerking worden genomen (deze segmenten kunnen alleen in de DSP worden geactiveerd). U kunt door alle relevante doelgroepen en binnen elke sectie van een knevel voorzien, kunt u de volgende metriek bekijken:

| Metrisch | Beschrijving |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL Resolved IDs] | Het aantal id&#39;s dat [!DNL Amazon’s Identity Resolution] heeft kunnen oplossen met behulp van uw publieksgegevens. |
| [!UICONTROL Overlapping ad exposed IDs] | Dit staat voor het aantal [!UICONTROL Resolved IDs] van het geüploade publiek dat ook via [!DNL Amazon Ads] aan een advertentie is blootgesteld. Hierbij wordt alleen rekening gehouden met DSP-impressies. |
| [!UICONTROL Overlap %] | Het aandeel van [!UICONTROL Resolved IDs] dat via [!DNL Amazon Ads] aan een advertentie is blootgesteld. |
| [!UICONTROL Categories] | De categorie of categorieën waartoe het publiek behoort. Een publiek kan tot veelvoudige categorieën behoren. |

### Overlappingen ontdekken met [!DNL Amazon Marketing Cloud] {#discover-overlaps}

De sectie **[!UICONTROL Discover overlaps with Amazon Marketing Cloud]** biedt inzicht in hoe uw publiek overlapt met [!DNL Amazon] doelsegmenten, of soorten publiek. U kunt de volgende cijfers weergeven:

| Metrisch | Beschrijving |
|--------------------------------|---------------------------------------------------------------------------------------------------|
| [!UICONTROL Resolved IDs] | Het aantal id&#39;s dat [!DNL Amazon’s Identity Resolution] heeft kunnen oplossen met behulp van uw publieksgegevens. |
| [!UICONTROL Overlapping ad exposed IDs] | Dit staat voor het aantal [!UICONTROL Resolved IDs] van het geüploade publiek dat ook via [!DNL Amazon Ads] aan een advertentie is blootgesteld. Hierbij wordt alleen rekening gehouden met DSP-impressies. |
| [!UICONTROL Overlap %] | Het aandeel van [!UICONTROL Resolved IDs] dat via [!DNL Amazon Ads] aan een advertentie is blootgesteld. |