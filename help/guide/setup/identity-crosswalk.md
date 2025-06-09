---
title: Identiteitskruizen
description: Leer allen over identiteitsoverzichten in Real-Time CDP Collaboration, met inbegrip van hoe brengt de identiteitsoverzichten binnen van verschillende bronnen, en hoe te om identiteitsoverzichten te beheren
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
hidefromtoc: true
hide: true
exl-id: a51f112d-3da7-4482-a24a-6d9f269d28d1
source-git-commit: fda414120decc0c76712616ff85b83febede53e9
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# Identiteitskruizen

{{limited-availability-release-note}}

Leer allen over identiteitsoverzichten in Real-Time CDP Collaboration, met inbegrip van hoe te om identiteitsoverzichten van verschillende bronnen binnen te brengen, en hoe te om identiteitsoverzichten te beheren.

Identiteitskruisen vergemakkelijken de veilige en privacy-volgzame verbinding van klantenidentiteiten over veelvoudige datasets en platforms. Door gehakte herkenningstekens te gebruiken, zorgt Real-Time CDP Collaboration ervoor dat de gebruikers identiteiten kunnen synchroniseren en in overeenstemming brengen zonder persoonlijke identificeerbare informatie (PII) bloot te stellen. Dit laat een verenigde mening van de klant voor betere samenwerking en gerichte marketing inspanningen toe.

<!--
In Real-Time CDP Collaboration, use identity crosswalks alongside your audiences by [TODO] insert material here. 
-->


Als eerste stap, moet u identiteitsoverzichten in Real-Time CDP Collaboration invoeren. Als u identiteitskruisverwijzingen wilt importeren in Real-Time CDP Collaboration, leest u de onderstaande sectie:

>[!NOTE]
>
>In de bètaversie van Real-Time CDP Collaboration, kunt u identiteitsoverzichten van uw datasets in Real-Time CDP invoeren. Verdere opties zijn beschikbaar in volgende releases.

## Identiteitskruisverwijzingen importeren in Real-Time CDP Collaboration {#import-crosswalk}

Navigeer aan **[!UICONTROL Setup]** > **[!UICONTROL Identity crosswalks]** lusje, selecteer het add pictogram (![ voeg pictogram toe.](/help/assets/icons/plus.png) ) en selecteert u **[!UICONTROL Identity crosswalk]**

![ Opname van hoe te om aan het scherm te krijgen om identiteitskruisverwijzingen toe te voegen ](/help/assets/setup/identity-crosswalks/import-identity-crosswalk.gif)

### Kruisbron selecteren

Selecteer een bron waar u het identiteitskruis van zult invoeren. In de eerste versie van Real-Time CDP Collaboration, is Experience Platform de enige gesteunde bron voor het invoeren van oversteekplaatsen.

>[!TIP]
>
>De kruisen die u van Experience Platform invoert worden bedoeld als *datasets* in Platform.

Na het selecteren van Experience Platform als bron van uw kruis, selecteer de [ zandbak van Experience Platform ](https://experienceleague.adobe.com/en/docs/experience-platform/sandbox/home) waarvan u het identiteitskruis invoert.

![ Opname van hoe te om een dwarshellbron te selecteren ](/help/assets/setup/identity-crosswalks/select-crosswalk-source.gif)

### Kruisje selecteren

Na het selecteren van Experience Platform als de bron van uw kruizen,

### Geef details

Geef een naam en een beschrijving voor het identiteitskruisje dat u in het product importeert.

### Verbindingssleutel selecteren {#select-join-key}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_import_crosswalk_join_key"
>title="Verbindingssleutel"
>abstract="Een verbindingssleutel is een uniek herkenningsteken dat wordt gebruikt om verslagen over verschillende datasets aan te passen en te verbinden. Het zorgt ervoor dat de gegevens uit diverse bronnen nauwkeurig met het zelfde individu of de zelfde entiteit kunnen worden geassocieerd. Om het even welke kolomkopballen van het geselecteerde kruis kunnen als verbindingssleutel dienen."

Een verbindingssleutel is een uniek herkenningsteken dat wordt gebruikt om verslagen over verschillende datasets aan te passen en te verbinden. Het zorgt ervoor dat de gegevens uit diverse bronnen nauwkeurig met het zelfde individu of de zelfde entiteit kunnen worden geassocieerd. Door de aangewezen verbindingssleutel te selecteren, kunt u gegevens effectief samenvoegen en in overeenstemming brengen, die de nauwkeurigheid en volledigheid van uw campagnes verbeteren.

Om het even welke kolomkopballen van het geselecteerde kruis kunnen als verbindingssleutel dienen.

Selecteer de gewenste verbindingssleutel voor de crosswalltabel en selecteer **[!UICONTROL Next]** om door te gaan naar de volgende stap.

### Controleren

Bekijk een van de selecties in de vorige schermen. Als u tevreden bent met de selectie, selecteert u **[!UICONTROL Next]** om de workflow te voltooien.

## Volgende stappen

Na het leren hoe te om identiteitsoverzichten in Real-Time CDP in te voeren, kunt u alle identiteitsoverzichten bekijken die u tot dusver aan Real-Time CDP Collaboration hebt toegevoegd. U kunt nu ook de identiteitskruisen gebruiken die u bij het invoeren van publiek in Real-Time CDP Collaboration hebt ingevoerd.
