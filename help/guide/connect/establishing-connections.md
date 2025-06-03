---
title: Verbinding maken met adverteerders of uitgevers
description: Na het ontdekken van potentiële medewerkers, leer hoe te om verbindingen te vestigen en beginnen aan projecten samen te werken.
audience: admin, publisher, advertiser
badgelimitedavailability: label="Beperkte beschikbaarheid" type="Informative" url="https://helpx.adobe.com/nl/legal/product-descriptions/real-time-customer-data-platform-collaboration.html newtab=true"
exl-id: 3fed93f7-1854-440c-802e-6b47e82918c9
source-git-commit: dd1386f9371cb40285315d11e07b139d3115e147
workflow-type: tm+mt
source-wordcount: '1248'
ht-degree: 0%

---

# Verbinding maken met adverteerders of uitgevers

{{limited-availability-release-note}}

Het tot stand brengen van een verbinding tussen twee partijen van een samenwerking (meestal een adverteerder en een uitgever) is in Real-Time CDP Collaboration een eerste vereiste voor bedrijven die samenwerken aan campagnes. Zowel uitgevers als adverteerders kunnen verbindingen instellen. Welke partij de verbinding in werking stelt zal nadien de *verbindingseigenaar* zijn.

## Workflow op hoog niveau

Op hoog niveau ziet de workflow er als volgt uit om een verbinding tot stand te brengen tussen een adverteerder en een uitgever:

1. De adverteerder [ doorbladert uitgevers en ontdekt ](/help/guide/connect/discover-publishers.md) die zij met willen werken
2. De adverteerder stuurt een verbindingsuitnodiging.
3. De uitgever accepteert de uitnodiging.
4. De adverteerder verzendt verbindingsinstellingen, inclusief overeenkomende sleutels en andere. Deze verbindingsmontages vertegenwoordigen de in-product termijnen van de samenwerking.
5. De uitgever accepteert verbindingsinstellingen. De uitgever kan desgewenst de eerste verbindingsinstellingen negeren en de adverteerder verzoeken herziene verbindingsinstellingen in te dienen.

![ diagram op hoog niveau van het adverteerder-uitgever verbindingsproces.](/help/assets/connect/establish-connection/advertiser-publisher-connection-process.png){zoomable="yes"}

Zodra de punten hierboven worden voltooid, kunnen de medewerkers te werk gaan [ een project ](/help/guide/collaborate/manage-projects.md#create-project) tot stand brengen om [ overlappende rapporten ](/help/guide/collaborate/discover.md) in werking te stellen en reclamecampagnes te schoppen.

>[!IMPORTANT]
>
>Zodra de verbinding tussen twee medewerkers is gevestigd, kunnen de verbindingsmontages niet meer worden herzien.

## Uitnodiging verzenden {#send-invite}

Als u een verbinding wilt instellen, selecteert u **[!UICONTROL Connect]** wanneer u door de uitgeversvoorraad bladert in het scherm met uitgevers zoeken.

![ verbind selecteur ](/help/assets/connect/establish-connection/connect-selection.png){zoomable="yes"}

Op dit punt is de uitnodiging verzonden en kunt u een voorvertoning van de verbindingsinstellingen bekijken, maar u kunt deze instellingen niet bewerken. U kunt de uitnodiging die in behandeling is weergeven op het tabblad **[!UICONTROL My connections]** . De status van de verbinding is **[!UICONTROL Invite sent]** .

![ In afwachting van Uitnodiging die naar uitgever wordt verzonden in de Mijn verbindingsmening.](/help/assets/connect/establish-connection/pending-invite-sent.png){zoomable="yes"}

Nadat de medewerker de uitnodiging heeft geaccepteerd, kunt u de verbindingsinstellingen configureren en deze naar de medewerker sturen om deze te controleren en te accepteren.

## Verbindingsinstellingen {#connection-settings}

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_usecases"
>title="Gebruiksscenario’s"
>abstract="De gebruiksscenario&#39;s worden vooraf gevuld met alle opties. U kunt de gebruiksgevallen bewerken voordat u de verbindingsinstellingen verzendt."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_matchkeys"
>title="Toetsen afstemmen"
>abstract="Identieke sleutels zijn vooraf ingevuld met degenen die u op uw organisatieniveau selecteerde. U kunt alle sleutels uitschakelen die u in deze verbinding niet wilt gebruiken."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit"
>title="Kredietsplitsing"
>abstract="In dit gedeelte wordt bepaald wie voor de overeenkomstige activiteiten in Real-Time CDP Collaboration betaalt. Momenteel, slechts is het publiek dat gebruikscase deelt configureerbaar."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_audiencesharing"
>title="Delen van publiek"
>abstract="Het Delen van het publiek is de activiteit die een partij neemt wanneer het verzoeken van hun gematchte gegevens om door hun samenwerkingspartner worden geactiveerd."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_creditsplit_measurement"
>title="Meting"
>abstract="Met dit gebruiksscenario kunt u activiteiten in Real-Time CDP Collaboration uitvoeren om rapporten en inzichten over de prestaties van de campagne te genereren."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_legalagreement"
>title="Juridische overeenkomst"
>abstract="Controleer of er een overeenkomst bestaat voor het uitwisselen van gegevens tussen beide partijen."

>[!CONTEXTUALHELP]
>id="rtcdp_collaboration_connection_settings_advertisername"
>title="Namen van adverteerders"
>abstract="<p>Optionele instelling. Geeft de naam en id aan waarmee de adverteerder bij de uitgever bekend is.</p><p>De naam van de adverteerder die u hier toevoegt, wordt vooraf ingevuld in de stap Project maken.</p><ul><li>Als de uitgever veelvoudige namen vormde, selecteer van de lijst.</li><li>Als slechts één naam wordt gevormd, wordt het vooraf geselecteerd automatisch.</li><li>Als er geen namen zijn geconfigureerd, wordt het veld voorgevuld met de naam van de adverteerderaccount van Real-Time CDP Collaboration.</li></ul>"
>additional-url="https://experienceleague.adobe.com/nl/docs/real-time-cdp-collaboration/using/collaborate/manage-projects#create-project" text="Een project maken"

Nadat de uitnodiging is verzonden, kunt u een voorbeeld van de verbindingsinstellingen bekijken. De uitnodiging moet worden geaccepteerd voordat u de verbinding kunt voltooien.

![ de mening van verbindingsmontages in de voorproefstaat.](/help/assets/connect/establish-connection/preview-connection-settings.png){zoomable="yes"}

Nadat de verbinding door uw medewerker is geaccepteerd, kunt u nu de verbindingsinstellingen voor de verbinding instellen. De verbindingsmontages bepalen de termijnen van uw samenwerking, zoals de gebruiksgevallen die u samen zult verwezenlijken, de gelijke sleutels die u in projecten, en meer zult gebruiken.

Navigeer naar **[!UICONTROL My connections]** als u verbindingsinstellingen wilt instellen en delen met uw medewerker. Voor alle verbindingen met de status **[!UICONTROL Pending]** kunt u **[!UICONTROL Set up connection]** selecteren om de verbindingsinstellingen te configureren.

![ de Mijn verbindingen mening met een In afwachting van verbinding en zijn benadrukte optie van de opstellingsverbinding.](/help/assets/connect/establish-connection/pending-connection.png){zoomable="yes"}

U kunt de onderstaande velden bewerken en definiëren:

![ de mening van de opstellingsverbinding ](/help/assets/connect/establish-connection/connection-view.png){zoomable="yes"}

+++Gebruik hoofdletters

Gebruiksscenario&#39;s worden vooraf ingevuld met alle beschikbare gebruiksgevallen. U kunt kiezen in welke gevallen uw verbinding wordt gebruikt door **[!UICONTROL Edit]** te selecteren en eventuele gebruiksgevallen die u niet wilt, uit te schakelen. De geselecteerde gebruiksgevallen zullen beïnvloeden welke meningen en opties [ beschikbaar binnen uw projecten ](../collaborate/manage-projects.md#project-use-cases) zijn.

![Gebruiksscenario’s](/help/assets/connect/establish-connection/view-use-cases.png){zoomable="yes"}

+++

+++Identieke toetsen

De sleutels van de gelijke worden vooraf gevuld met degenen die u [ op uw organisatieniveau ](/help/guide/setup/onboard-organization.md#set-up-match-keys) selecteerde. U kunt alle sleutels uitschakelen die u in deze verbinding niet wilt gebruiken, maar u kunt geen overeenkomende toetsen toevoegen die niet zijn geselecteerd bij het instellen van de organisatie.

![ de sleutels van de Gelijke ](/help/assets/connect/establish-connection/match-keys.png){zoomable="yes"}

+++

+++Kredietsplitsing

Gebruik de afdeling kredietsplitsing om te bepalen welke van de twee samenwerkende partijen de kosten voor de activiteiten zullen dekken. De splitsingsopties voor crediteringen worden bepaald door de geselecteerde gebruiksgevallen voor de verbinding. Hoewel voor de **[!UICONTROL Measurement]** use case één partij nodig is om de kosten te dekken, biedt de **[!UICONTROL Audience activation]** use case een extra mogelijkheid om elke partij hun eigen kosten te laten dekken. Voor informatie over de verdeling van kosten, lees de [ gids van de type van kredietactiviteit ](/help/guide/setup/my-activity.md#types-of-activities).

>[!NOTE]
>
>Publiek - De egress wordt altijd bedekt door de medewerker die het publiek ontvangt. Er is daarom geen selectie vereist.

![ de gespleten dialoog van het Krediet met opties in de verbindingswerkruimte.](/help/assets/connect/establish-connection/credit-split.png){zoomable="yes"}
+++

+++Overeenkomsten

Voordat u kunt doorgaan met deze verbinding, moet u erkennen dat er een overeenkomst bestaat voor het delen van gegevens tussen beide partijen.

![ Juridische overeenkomsten.](/help/assets/connect/establish-connection/legal-agreement.png){zoomable="yes"}

+++

+++Namen van adverteerders

Als uitgever die aan de verbindingsmontages werkt, kunt u selecteren om het even welke adverteerdernamen toe te voegen waardoor de adverteerder aan u in uw systemen gekend is. Als uitgever kunt u bijvoorbeeld meerdere adverteerdernamen toevoegen aan een verbinding wanneer de adverteerder waarmee u werkt, in meerdere geografische gebieden aanwezig is. Later in het proces, wanneer [ creërend een project ](/help/guide/collaborate/manage-projects.md#create-project) om aan samen te werken, zult u of uw medewerker de adverteerdernaam kunnen selecteren om met het project te associëren.

![ voeg adverteerdernamen modaal toe.](/help/assets/connect/establish-connection/add-advertiser-names-modal.png)

Hieronder wordt beschreven hoe de naamselectie van adverteerders werkt bij het maken van een project:

1. **Geen geplaatste adverteerdernaam**: Als geen adverteerdernamen worden toegevoegd, blijft Real-Time CDP Collaboration aan het gebruiken van de naam van de adverteerder als adverteerdernaam in gebreke.
2. **Één de naamreeks van adverteerders**: Als één enkele adverteerdernaam wordt toegevoegd, gebruikt Real-Time CDP Collaboration automatisch die naam als adverteerdernaam voor het project.
3. **Veelvoudige geplaatste adverteerdernamen**: Als meer dan één adverteerdernaam wordt toegevoegd, kunt u of uw medewerker om het even welke verstrekte namen selecteren wanneer het creëren van het project.

![ Advertiser namen.](/help/assets/connect/establish-connection/advertiser-names.png)

+++

Nadat u uw selectie hebt gemaakt, selecteert u **[!UICONTROL Submit]** om de voorgestelde instellingen ter controle naar uw medewerker te sturen.

Als u voorgestelde verbindingsmontages van uw medewerker ontvangt, kunt u of **[!UICONTROL Accept]** of **[!UICONTROL Reject]** die montages. Voordat u de verbindingsinstellingen accepteert, moet u bevestigen en bevestigen dat er een juridische overeenkomst bestaat tussen u en de medewerker. Als u verbindingsmontages verwerpt, bereik aan uw medewerker buiten het product en bespreek hoe zij de verbindingsmontages voor u zouden moeten herzien om hen te aanvaarden.

## Verbindingen verwijderen {#delete-connections}

U kunt om het even welke verbindingen met medewerkers schrappen die u niet wilt blijven werken met. Bestaande verbindingen verwijderen:

1. Ga naar **[!UICONTROL Connect]** > **[!UICONTROL My connections]**.
2. Selecteer **[!UICONTROL View connection]** op de verbindingskaart om toegang te krijgen tot de verbinding die u wilt verwijderen.
3. Selecteer het schrappingspictogram ![ schrappingspictogram ](/help/assets/common/delete.svg) om de dialoog van de de bevestigingsbevestiging van de schrappingsverbinding omhoog te brengen.
   ![ benadrukte verbindingspictogram van de Schrapping.](/help/assets/connect/establish-connection/delete-icon-highlighted.png){zoomable="yes"}
4. Bevestig de verwijdering door **[!UICONTROL Delete]** te selecteren.
   ![ Dialoog om schrapping van een verbinding te bevestigen. ](/help/assets/connect/establish-connection/delete-connection-dialog.png){zoomable="yes"}

>[!WARNING]
>
>Zodra de verbinding wordt geschrapt, zult u niet meer met de medewerker worden verbonden en alle bestaande projecten die deel van de samenwerking uitmaken zullen permanent worden geschrapt en onherstelbaar zijn.

## Volgende stappen

Na het vestigen van een verbinding met uw medewerker, kunt u en uw medewerker projecten [&#128279;](/help/guide/collaborate/manage-projects.md#create-project) nu tot stand brengen.
