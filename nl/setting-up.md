---
description: RTFM
---

# 🛠️ Instellen

Als je fouten ondervindt, bekijk dan de [Veelgestelde Vragen](faq.md).

Voordat je begint met instellen, zorg ervoor dat je een standalone Discord-client hebt (**niet in de browser**) en dat je de activiteitsstatus in Discord-instellingen hebt ingeschakeld:

![image](https://github.com/maximmax42/CustomRP-Docs/assets/2225711/a1b8cb1e-7f88-4061-b297-2691523718a5)

## Installatieproces

* Open de [Discord Developer portal](https://discord.com/developers/applications).
* Klik op **Nieuwe Applicatie** in de rechterbovenhoek.

![](https://user-images.githubusercontent.com/2225711/161050202-c796103d-6712-401e-be96-3f3712512375.png)

* Kies een naam voor de applicatie, deze zal worden weergegeven na "Playing" in de status; klik op **Aanmaken**.
* Kopieer de **Applicatie-ID** en plak deze in het Custom RP-veld **ID**, druk vervolgens op **Verbinden**.&#x20;

![](https://user-images.githubusercontent.com/2225711/161050341-8169af53-5d3f-44d6-b745-cc711e8d1476.png)

* Als dit correct is gedaan, zou je status in Discord nu moeten zeggen "Playing **\[naam van de app]**". In geval van fouten, bekijk de [Veelgestelde Vragen](faq.md).
  * De status wordt niet weergegeven als je onzichtbaar bent.
  * Als je een aangepaste status hebt ingesteld (deze met emoji), wordt deze voorrang gegeven boven je CustomRP-status. De CustomRP-status wordt echter wel weergegeven in het profielpop-upvenster.
* Nu kun je de andere velden invullen (alles is optioneel):
  * **Details**: Eerste regel in de aanwezigheid onder de app-naam.
  * **Status**: Tweede regel in de aanwezigheid. Wordt de eerste als Details leeg is.
  * **Party**: Verschijnt als `(X van Y)` na de Status-regel. Als Status leeg is, wordt Party-aantal niet weergegeven.
  * **Tijdstempel**: Een timer die telt naar of vanaf een specifieke tijdstempel. Weergegeven onder Details en Status als `xx:xx:xx verstreken` of `xx:xx:xx resterend`. Kan slechts tot `23:59:59` weergeven voordat het overgaat naar `00:00`.
  * **Grote en kleine afbeeldingen**: Afbeeldingen die aan de linkerkant van de aanwezigheid worden weergegeven. Als beide aanwezig zijn, bevindt de kleine afbeelding zich rechtsonder in de grote afbeelding.
    * **Sleutel**: Ofwel een directe URL (voorkeur, omdat je op die manier ook GIF's kunt gebruiken) of een Art Asset-naam.
      * _URL-methode:_ Als je afbeelding al op internet staat, plaats dan de **directe link** (meestal gedaan door met de rechtermuisknop op de afbeelding te klikken en iets te kiezen als "Afbeeldingslink kopiëren") in het veld. Als je afbeelding op je pc staat, gebruik dan een website voor het hosten en delen van afbeeldingen (bijv. Imgur, ImageShack, etc.). Het wordt **niet aanbevolen** om afbeeldingen te uploaden die in Discord DM's/kanalen zijn verzonden, omdat hun links te snel te groot worden en ze na 2 weken verlopen.
        * Als je na het verbinden vastloopt op "Aanwezigheid bijwerken...", is de kans groot dat de URL die je hebt ingevoerd te lang was of geen directe URL was. Als je zeker weet dat het een directe is, gebruik dan een URL-verkorter.
      * _Art Asset-methode:_ Op de pagina van je applicatie, navigeer naar Rich Presence -> Art Assets en upload ten minste één afbeelding onder Rich Presence Assets. In CustomRP is er een handige **Upload Assets**-knop in het Bestand-menu (je kunt ook Ctrl+U gebruiken) die je daar naartoe brengt als je ID-veld correct is ingesteld.
        * Opmerking 1: Hoewel de afbeeldingen meestal direct bruikbaar worden, kan het in sommige gevallen enkele uren duren.
        * Opmerking 2: Hoewel je je asset elke naam kunt geven tot 999 symbolen, accepteert de app alleen namen met maximaal 256 symbolen.
    * **Tekst**: Een tekst die verschijnt wanneer je over de afbeelding zweeft (of lang tapt op mobiel).
  * **Knoppen**:
    * **Tekst**: Een tekst die op de knop wordt weergegeven.
    * **URL**: Een URL die de knop opent bij het klikken.
* Klik op **Aanwezigheid bijwerken** (of **Verbinden** als je nog niet verbonden bent).
* Gefeliciteerd, je bent geweldig!

### Ik gebruik meer dan één Discord-client, wat moet ik doen?

Als je meer dan één Discord-client hebt en je wilt dat je aanwezigheid op een ander account wordt weergegeven dan degene die de app automatisch heeft gekozen, druk dan op **Verbinding verbreken**, houd dan de Ctrl+Shift-toetsen ingedrukt op je toetsenbord en druk op **Verbinden**. Een venster met een nummerinvoer zal verschijnen, voer een nummer 1 in, sluit het venster en druk opnieuw op **Verbinden**, zonder Ctrl+Shift. Als het weer het verkeerde account is, probeer dan nummer 0, dan 2, enzovoort tot 9.

Let op dat als je meerdere Discord-clients hebt die opstarten bij het opstarten, het pipe-nummer dat aan elke client is toegewezen mogelijk niet persistent is bij elke opstart en kan veranderen afhankelijk van welke client als eerste is gestart. Om dit te voorkomen, kun je extra clients handmatig starten of de Windows Taakplanner gebruiken om de opstart van de clients te vertragen.

Als je 2 accounts hebt die je tegelijkertijd gebruikt en je wilt dat elk van hen een andere aanwezigheid heeft, volg dan deze stappen:

* Stel je hoofdaccount eerst in met de bovenstaande instructies.
* Download de nieuwste **portable (.zip)** versie van CustomRP (of van de [website](https://www.customrp.xyz) of de [GitHub releases pagina](https://github.com/maximmax42/Discord-CustomRP/releases/latest)) en pak het ergens uit.
  * Dit werkt alleen met versies 1.16 en nieuwer.
* Open `Start Second Instance.bat` of maak een snelkoppeling naar CustomRP.exe met het argument `--second-instance` (of `-2`).
* Stel het programma in zoals je je hoofdinstantie hebt ingesteld.
  * Tip: Als je al een preset hebt die je wilt gebruiken met je tweede instantie, kun je het batchbestand of de snelkoppeling bewerken om het pad naar de preset op te nemen. Voorbeeld: `CustomRP.exe -2 "C:\Some Folder\preset.crp"` (aanhalingstekens om het pad zijn noodzakelijk als het pad spaties bevat).
* Voordat je verbindt, verander de pipe zoals eerder beschreven en verbind.

Als je 3 of meer accounts tegelijkertijd gebruikt, dan... waarom? Maar als genoeg van jullie mij lastigvallen, zal ik ondersteuning toevoegen voor het gebruik van meer instanties.

## Notities

* Als je geen kleine of grote afbeelding wilt instellen, laat dan alle gerelateerde velden in het programma leeg.
* Als er geen grote afbeelding is ingesteld, worden de instellingen voor kleine afbeeldingen genegeerd.
