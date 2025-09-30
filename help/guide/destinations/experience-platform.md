---
title: Adobe Experience Platform configureren als bestemming
description: Leer hoe u Adobe Experience Platform configureert en beheert als een doel in Real-Time CDP Collaboration.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/nl/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 594610a0-9102-448a-b59b-ec162ef9dd57
source-git-commit: 0dead396657c97cec47ddd64c8ec3c349f541a8f
workflow-type: tm+mt
source-wordcount: '1432'
ht-degree: 0%

---

# Adobe Experience Platform configureren als bestemming

{{limited-availability-release-note}}

Configureer deze bestemming om het publiek van uw project naar Adobe Experience Platform te activeren. Als u het publiek activeert naar Adobe Experience Platform, kunt u de mogelijkheden van het platform benutten voor publiekssegmentatie, -analyse en -activering via verschillende marketingkanalen. Meer over Adobe Experience Platform leren, verwijs naar het [ overzicht van Experience Platform ](https://experienceleague.adobe.com/nl/docs/experience-platform/landing/home){target="_blank"}.

>[!WARNING]
>
>U kunt een doel niet bijwerken nadat het is gemaakt. Als u instellingen moet wijzigen, moet u het bestaande doel verwijderen en een nieuw doel maken.

## Doel configureren {#configure-destination}

Als u Adobe Experience Platform als doel wilt configureren, navigeert u naar **[!UICONTROL Setup]** en selecteert u de tab **[!UICONTROL My destinations]** . Selecteer **[!UICONTROL Set up]** voor Adobe Experience Platform.

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
>id="rtcdp_collaboration_destinations_activation_mapping"
>title="Meer informatie"
>abstract=""

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_target_namespaces"
>title="Doelnaamruimten"
>abstract="Doelnaamruimten bepalen aan welke naamruimte de overeenkomende sleutel wordt toegewezen in Adobe Experience Platform. De gehakte gelijke sleutels moeten aan een doelnamespace worden in kaart gebracht die gehakte waarden steunt."

Alle overeenkomende toetsen die voor uw account zijn ingeschakeld, worden standaard in de activeringstoewijzing opgenomen. Als u een overeenkomende sleutel niet rechtstreeks wilt toewijzen aan een doelnaamruimte, kunt u de optie voor de gekoppelde sleutel gebruiken om deze te vervangen door een andere overeenkomende sleutel. Voor meer informatie over verbonden sleutels, zie de [ sectie hieronder ](#linked-keys).

#### Doelnaamruimten toewijzen {#map-target-namespaces}

Als u elke overeenkomende sleutel wilt toewijzen aan een doelnaamruimte, selecteert u het veld **[!UICONTROL Target namespaces]** naast de overeenkomende sleutel. Het dialoogvenster **[!UICONTROL Select source field]** wordt weergegeven. Zoek de doelnaamruimte in de lijst of zoek naar een specifieke naamruimte. Selecteer de doelnaamruimte die u voor de overeenkomende toets wilt gebruiken en selecteer vervolgens **[!UICONTROL Select]** .

>[!IMPORTANT]
>
>De gehakte gelijke sleutels moeten aan een doelnamespace worden in kaart gebracht die gehakte waarden steunt. De **[!UICONTROL Hashed email]** -sleutel moet bijvoorbeeld worden toegewezen aan de naamruimte **[!UICONTROL Email(SHA256, lowercased)]** in Adobe Experience Platform. U kunt de sleutel **[!UICONTROL Hashed email]** match niet toewijzen aan de naamruimte **[!UICONTROL Email]** , omdat deze naamruimte hashed-waarden niet ondersteunt.

![ de Uitgezochte dialoog van het brongebied met de Uitgezochte benadrukte optie.](/help/assets/destinations/adobe-experience-platform/select-target-namespace.png)

Herhaal dit proces voor elke gelijke sleutel die u in de activeringstoewijzing wilt omvatten. Als u geen overeenkomende sleutel wilt opnemen, kunt u deze verwijderen of de optie voor de gekoppelde sleutel gebruiken om deze te vervangen door een andere overeenkomende sleutel.

#### Gekoppelde toetsen {#linked-keys}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_destinations_linked_key"
>title="Gekoppelde sleutel"
>abstract="Met gekoppelde sleutels kunt u opgeven dat tijdens de activering een andere overeenkomende toets moet worden gebruikt in plaats van de oorspronkelijke overeenkomende toets. Een profiel kan alleen worden geactiveerd als het waarden bevat voor zowel de oorspronkelijke overeenkomende sleutel als de gekoppelde overeenkomende sleutel."

Met gekoppelde sleutels kunt u opgeven dat tijdens de activering een andere overeenkomende toets moet worden gebruikt in plaats van de oorspronkelijke overeenkomende toets. Neem het volgende voorbeeld om beter te begrijpen hoe gekoppelde toetsen werken:

Een retailer wil de gegevens die worden geactiveerd naar Experience Platform verzenden naar zijn CRM-systeem. De retailer heeft Hashed IP als gelijke sleutel voor hun rekening toegelaten om het gelijke tarief te verhogen wanneer het activeren van publiek. Nochtans, steunt het systeem van CRM van retailer Hashed IP niet als identiteitsnamespace, zodat willen zij de de overeenkomende sleutel van identiteitskaart van CRM in plaats daarvan gebruiken wanneer het activeren van publiek aan Experience Platform. De retailer kan de optie voor gekoppelde sleutels gebruiken om het publiek naar Experience Platform te activeren met CRM-id in plaats van naar onderbroken IP.

>[!NOTE]
>
>Een profiel kan alleen worden geactiveerd als het waarden bevat voor zowel de oorspronkelijke overeenkomende sleutel als de gekoppelde overeenkomende sleutel. Bijvoorbeeld, als Hashed identiteitskaart met identiteitskaart van CRM wordt verbonden, moet een profiel waarden voor zowel Hashed identiteitskaart als identiteitskaart van CRM hebben om worden geactiveerd. Als een van deze waarden ontbreekt, wordt het profiel niet geactiveerd.

Als u een gekoppelde sleutel wilt gebruiken, schakelt u de optie **[!UICONTROL Linked key]** in of uit naast de overeenkomende sleutel die u in de plaats wilt gebruiken. De sectie **[!UICONTROL Linked key]** lijkt u te vragen om de afbeelding te maken.

![ de Gekoppelde belangrijkste optie en de sectie die in het Create bestemmingswerkschema wordt benadrukt.](/help/assets/destinations/adobe-experience-platform/linked-key.png)

Selecteer de **[!UICONTROL Linked key]** die u wilt gebruiken in het vervolgkeuzemenu. In het volgende voorbeeld selecteert de retailer **[!UICONTROL CRM ID]** als de gekoppelde sleutel.

![ Linked zeer belangrijke dropdown die in het Create bestemmingswerkschema wordt benadrukt.](/help/assets/destinations/adobe-experience-platform/select-linked-key.png)

Vervolgens wilt u de doelnaamruimte voor de gekoppelde sleutel opgeven als u dat nog niet hebt gedaan. Als u al de doelnaamruimte voor de overeenkomende sleutel hebt geselecteerd in de sectie **[!UICONTROL Create activation mapping]** , wordt deze automatisch ingevuld. Als u nog geen doelnaamruimte hebt geselecteerd voor de gekoppelde sleutel, kunt u dat nu doen.

Selecteer het veld **[!UICONTROL Target namespaces]** naast de gekoppelde sleutel. Het dialoogvenster **[!UICONTROL Select source field]** wordt weergegeven. Zoek de doelnaamruimte in de lijst of zoek naar een specifieke naamruimte. Selecteer de doelnaamruimte die u voor de gekoppelde sleutel wilt gebruiken en selecteer vervolgens **[!UICONTROL Select]** .

![ de Uitgezochte dialoog van het brongebied.](/help/assets/destinations/adobe-experience-platform/select-linked-key-target-namespace.png)

De gekoppelde sleutel is nu geconfigureerd.

>[!NOTE]
>
>U kunt slechts één gekoppelde sleuteldoelnaamruimte per activeringstoewijzing gebruiken. Als u bijvoorbeeld een koppeling tot stand brengt tussen de hashed-id en de CRM-id, wordt deze koppeling ook gekoppeld aan de CRM-id wanneer u de gekoppelde-sleuteloptie voor een ander veld inschakelt.

Wanneer u alle overeenkomende toetsen hebt toegewezen, controleert u uw instellingen. De sectie **[!UICONTROL Preview]** bevat een overzicht van uw configuratie.

![ de sectie van de Voorproef in Create bestemmingswerkschema.](/help/assets/destinations/adobe-experience-platform/preview.png)

>[!IMPORTANT]
>
>Op dit moment activeert elke match-toets naar Experience Platform als een apart publiek. Als u bijvoorbeeld [!UICONTROL Hashed email] en [!UICONTROL Hashed phone] als overeenkomende toetsen hebt, worden twee verschillende soorten publiek gemaakt in Poorten publiek wanneer een publiek wordt geactiveerd.

Selecteer **[!UICONTROL Create destination]** als u tevreden bent met de configuratie. Er verschijnt een bevestigingsbericht dat aangeeft dat de bestemming is gemaakt.

## Adobe Experience Platform gebruiken als doel

Zodra u Experience Platform als bestemming hebt gevormd, kunt u [ beginnen activerend publiek ](../collaborate/activate.md) aan het platform door uw projecten. Momenteel is het activeringsproces een proces in één stap dat door de deelnemer wordt geïnitieerd. Wanneer een adverteerder bijvoorbeeld een publiek activeert, wordt deze naar de vooraf geconfigureerde bestemming van de uitgever (Experience Platform) verzonden. De uitgever hoeft geen extra stappen te ondernemen om het publiek naar de bestemming te sturen. Hetzelfde geldt voor het merk-tot-merk samenwerkingspatroon.

>[!IMPORTANT]
>
>U **moet** Experience Platform als bestemming *vormen alvorens* uw medewerker een publiek activeert. Als de bestemming niet wordt gevormd, zal het publiek naar u worden verzonden en in het **[!UICONTROL Activate]** lusje binnen een project zichtbaar, maar zal niet aan Experience Platform worden geactiveerd.

Nadat het publiek wordt geactiveerd, zal het in [ Portaal van het Publiek ](#audience-portal) in Experience Platform met Real-Time CDP Collaboration als oorsprong beschikbaar zijn.  Deze doelgroepen kunnen vervolgens worden gebruikt in campagnes en de betrokkenheid van klanten.

### Poort publiek {#audience-portal}

Nu u Adobe Experience Platform als bestemming hebt gevormd, kunt u de geactiveerd publiek in het Portaal van het Publiek bekijken. De Portaal van het publiek is een centrale hub binnen Adobe Experience Platform die u toestaat om uw publiek te bekijken en te beheren. De portal Publiek biedt nu Real-Time CDP Collaboration als oorsprong bij het filteren van uw publiek.

>[!IMPORTANT]
>
>U bent verantwoordelijk voor het toepassen van de benodigde labels voor gegevensgebruik op het publiek dat u activeert op Adobe Experience Platform. Voor meer informatie, verwijs naar de [ etiketten van het gegevensgebruik ](https://experienceleague.adobe.com/nl/docs/experience-platform/data-governance/labels/overview){target="_blank"} gids.

![ het Portaal van de Publiek met Real-Time CDP Collaboration als oorsprong in de filteropties.](/help/assets/destinations/adobe-experience-platform/audience-portal.png)

Meer over het Portaal van het Publiek leren, verwijs naar de [ gids van het Portaal van het Publiek van 0&rbrace;.](https://experienceleague.adobe.com/nl/docs/experience-platform/segmentation/ui/audience-portal#manage-audiences){target="_blank"}
