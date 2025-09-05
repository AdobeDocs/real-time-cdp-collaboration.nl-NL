---
title: Adobe Experience Platform configureren als bestemming
description: Leer hoe u Adobe Experience Platform configureert en beheert als een doel in Real-Time CDP Collaboration.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/nl/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 594610a0-9102-448a-b59b-ec162ef9dd57
source-git-commit: f13b0996c35bcb6060c583ca328c2c04daaf8abc
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---

# Adobe Experience Platform configureren als bestemming

{{limited-availability-release-note}}

Configureer deze bestemming om het publiek van uw project naar Adobe Experience Platform te activeren. Als u het publiek activeert naar Adobe Experience Platform, kunt u de mogelijkheden van het platform benutten voor publiekssegmentatie, -analyse en -activering via verschillende marketingkanalen. Meer over Adobe Experience Platform leren, verwijs naar het [ overzicht van Experience Platform ](https://experienceleague.adobe.com/nl/docs/experience-platform/landing/home){target="_blank"}.

## Doel configureren {#configure-destination}

Als u Adobe Experience Platform als doel wilt configureren, navigeert u naar **[!UICONTROL Setup]** en selecteert u de tab **[!UICONTROL Destinations]** . Selecteer **[!UICONTROL Set up]** voor Adobe Experience Platform.

![ De Mijn die bestemmingswerkruimte met de optie van de Opstelling voor de bestemming van Adobe Experience Platform wordt benadrukt.](/help/assets/destinations/adobe-experience-platform/setup-aep.png)

De **[!UICONTROL Create destination]** -workflow wordt weergegeven.

![ Create bestemmingswerkschema voor Adobe Experience Platform.](/help/assets/destinations/adobe-experience-platform/create-destination.png)

### Sandbox configureren {#configure-sandbox}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_audience_expiration"
>title="Vervaldatum van het publiek"
>abstract="De periode waarna het publiek niet meer beschikbaar zal zijn in Adobe Experience Platform. De standaardvervaldatum is 30 dagen, maar u kunt deze instellen op een waarde tussen 1 en 30 dagen."

Eerst selecteert u de sandbox waarin de publieksgegevens worden verzonden.

>[!IMPORTANT]
>
>U kunt alleen een sandbox selecteren waartoe de gebruiker toegang heeft. Door gebrek, hebben alle gebruikers van Collaboration toegang tot **Prod** zandbak. Om toegang te krijgen tot extra sandboxen, moet een beheerder extra sandboxen toevoegen aan een rol die aan de gebruiker is toegewezen. Voor meer informatie over het beheren van rollen, verwijs naar [ rollen ](../permissions/manage-roles.md) gids beheren.

Selecteer in de sectie **[!UICONTROL Configure sandbox]** het vervolgkeuzemenu **[!UICONTROL Sandbox]** of typ de naam van een sandbox.

![ Sandbox dropdown die in het Create bestemmingswerkschema wordt benadrukt.](/help/assets/destinations/adobe-experience-platform/select-sandbox.png)

U kunt ook **[!UICONTROL Browse sandbox]** selecteren om alle beschikbare sandboxen en de bijbehorende **[!UICONTROL Type]** , **[!UICONTROL Status]** en **[!UICONTROL Region]** weer te geven. Selecteer de sandbox die u wilt gebruiken en selecteer vervolgens **[!UICONTROL Save]** .

Configureer vervolgens de **[!UICONTROL Audience Expiration]** . Standaard is de vervaldatum van het publiek ingesteld op 30 dagen. U kunt de vervaldatum op een willekeurige plaats instellen, van 1 tot en met 30 dagen. Na de vervaldatum is het publiek niet meer beschikbaar in Adobe Experience Platform.

![ de sectie van de Vervalsing van het Publiek die in het Create bestemmingswerkschema wordt benadrukt.](/help/assets/destinations/adobe-experience-platform/audience-expiration.png)

### Activeringstoewijzing maken {#create-activation-mapping}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_activation_matchkeys"
>title="Aanpassingssleutels activering"
>abstract="Activeringssleutels worden weergegeven op basis van de sleutels die u hebt geselecteerd bij het maken van uw organisatie."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_target_namespaces"
>title="Doelnaamruimten"
>abstract="Doelnaamruimten bepalen aan welke naamruimte de overeenkomende sleutel wordt toegewezen in Adobe Experience Platform. De gehakte gelijke sleutels moeten aan een doelnamespace worden in kaart gebracht die gehakte waarden steunt."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_linked_key"
>title="Gekoppelde sleutel"
>abstract="Plaatsaanduiding voor contextafhankelijke gekoppelde sleutel."

Vervolgens moet u een activeringstoewijzing maken om te bepalen hoe de publieksgegevens naar Adobe Experience Platform worden verzonden. U kunt elk [ gelijke sleutel ](../setup/onboard-account.md#set-up-match-keys) in kaart brengen u terwijl het creëren van uw organisatie aan een doel namespace selecteerde. Het doel namespaces specificeert welke [ identiteit namespace ](https://experienceleague.adobe.com/nl/docs/experience-platform/identity/features/namespaces#standard){target="_blank"} de gelijke sleutel aan in Adobe Experience Platform in kaart zal worden gebracht.

>[!IMPORTANT]
>
>De gehakte gelijke sleutels moeten aan een doelnamespace worden in kaart gebracht die gehakte waarden steunt. De **[!UICONTROL Hashed email]** -sleutel moet bijvoorbeeld worden toegewezen aan de naamruimte **[!UICONTROL Email(SHA256, lowercased)]** in Adobe Experience Platform. U kunt de sleutel **[!UICONTROL Hashed email]** match niet toewijzen aan de naamruimte **[!UICONTROL Email]** , omdat deze naamruimte hashed-waarden niet ondersteunt.

Selecteer het veld **[!UICONTROL Target namespaces]** naast elke overeenkomende toets. Het dialoogvenster **[!UICONTROL Select source field]** wordt weergegeven. Zoek de doelnaamruimte in de lijst of zoek naar een specifieke naamruimte. Selecteer de doelnaamruimte die u voor de overeenkomende toets wilt gebruiken en selecteer vervolgens **[!UICONTROL Select]** .

![ de Uitgezochte dialoog van het brongebied met de Uitgezochte benadrukte optie.](/help/assets/destinations/adobe-experience-platform/select-target-namespace.png)

Wanneer u alle overeenkomende toetsen hebt toegewezen, controleert u de instellingen en selecteert u **[!UICONTROL Create]** om het maken van het doel te voltooien.

## Adobe Experience Platform gebruiken als doel

Zodra u Adobe Experience Platform als bestemming hebt gevormd, kunt u [ beginnen activerend publiek ](../collaborate/activate.md) aan het platform door uw projecten. Momenteel is het activeringsproces een eenstapsproces dat door de adverteerder is geïnitieerd. Wanneer de adverteerder een publiek activeert, wordt het verzonden naar de vooraf geconfigureerde bestemming van de uitgever (in dit geval Adobe Experience Platform). De uitgever hoeft geen extra stappen te ondernemen om het publiek naar de bestemming te sturen.

>[!IMPORTANT]
>
>U **moet** Adobe Experience Platform als bestemming *vormen alvorens* uw medewerker een publiek activeert. Als de bestemming niet wordt gevormd, zal het publiek naar u worden verzonden en in het **[!UICONTROL Activate]** lusje binnen een project zichtbaar, maar zal niet aan Adobe Experience Platform worden geactiveerd.

Nadat het publiek wordt geactiveerd, zal het in [ Portaal van het Publiek ](#audience-portal) in Experience Platform met Real-Time CDP Collaboration als oorsprong beschikbaar zijn.  Deze doelgroepen kunnen vervolgens worden gebruikt in campagnes en de betrokkenheid van klanten.

### Poort publiek {#audience-portal}

Nu u Adobe Experience Platform als bestemming hebt gevormd, kunt u de geactiveerd publiek in het Portaal van het Publiek bekijken. De Portaal van het publiek is een centrale hub binnen Adobe Experience Platform die u toestaat om uw publiek te bekijken en te beheren. De portal Publiek biedt nu Real-Time CDP Collaboration als oorsprong bij het filteren van uw publiek.

>[!IMPORTANT]
>
>U bent verantwoordelijk voor het toepassen van de benodigde labels voor gegevensgebruik op het publiek dat u activeert op Adobe Experience Platform. Voor meer informatie, verwijs naar de [ etiketten van het gegevensgebruik ](https://experienceleague.adobe.com/nl/docs/experience-platform/data-governance/labels/overview){target="_blank"} gids.

![ het Portaal van de Publiek met Real-Time CDP Collaboration als oorsprong in de filteropties.](/help/assets/destinations/adobe-experience-platform/audience-portal.png)

Meer over het Portaal van het Publiek leren, verwijs naar de [ gids van het Portaal van het Publiek van 0&rbrace;.](https://experienceleague.adobe.com/nl/docs/experience-platform/segmentation/ui/audience-portal#manage-audiences){target="_blank"}
