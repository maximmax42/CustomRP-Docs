---
description: Stop alsjeblieft met me dezelfde vragen te stellen in de server.
---

# ❓ Veelgestelde Vragen

## Vragen

### Is dit een virus? Mijn antivirus/VirusTotal/etc zegt dat er een virus is.

Nee. CustomRP bevat geen virussen; de broncode is voor iedereen beschikbaar om te controleren.

Waarom zeggen sommige antivirusprogramma's en VirusTotal dan dat er een virus is? Voornamelijk omdat mijn app a) niet populair genoeg is om door Windows en sommige antivirusprogramma's als betrouwbaar te worden beschouwd, en b) niet is ondertekend met een codeondertekeningscertificaat (omdat ik Russisch ben, kan ik er momenteel zelfs geen kopen, en als dat wel kon, zijn ze behoorlijk duur).

### Kan ik meer dan 2 knoppen toevoegen?

Nee, dat is een beperking van Discord.

### Kan ik een ander type activiteit gebruiken (bijv. luisteren, kijken, streamen)?

Nee, dat is ook een beperking van Discord.

### Waarom laat Discord, als ik een tijdstempel instel voor een paar dagen in de toekomst, alleen zien hoeveel uur er over zijn?

Je raadt het al, ook dat is een beperking van Discord.

### Komen er Linux/Mac-versies?

De app is gebouwd met een Windows-only bibliotheek, dus ondersteuning voor Linux en Mac zou betekenen dat de hele app herschreven moet worden in een andere bibliotheek/programmeertaal, wat ik op dit moment niet van plan ben.

### Er opende een venster genaamd "Pipe" om een of andere reden, wat is dit?

Het opende omdat je Ctrl+Shift hebt ingedrukt en op de Verbinden-knop hebt geklikt (of Ctrl en de Verbinden-knop of Opnieuw verbinden in het systeemvakmenu op oudere versies). Laat het op -1 staan en sluit het. Het wordt gebruikt in situaties waarin je meerdere Discord-clients tegelijkertijd hebt draaien. Door het pijpnummer te wijzigen, kies je effectief welke client je aanwezigheid moet hebben.

## Probleemoplossing

Voordat je iets probeert, zorg ervoor dat je de laatste versie van CustomRP gebruikt!

### Ik heb CustomRP geïnstalleerd maar het start niet.

Dit komt hoogstwaarschijnlijk doordat je antivirusprogramma de app blokkeert bij het starten. Voeg de map `%appdata%\CustomRP` toe aan de uitzonderingen.

### Ik heb CustomRP geïnstalleerd, toegang verleend voor analyses en de app werkt niet meer.

Sluit de app in Taakbeheer, verwijder de map `%localappdata%\maximmax42`, start de app opnieuw en sta geen analyses toe.

### De app heeft verbinding gemaakt, maar ik zie de status niet in mijn profiel.

Zorg ervoor dat je de activiteitsstatus hebt ingeschakeld in de Discord-instellingen:

![image](https://github.com/maximmax42/CustomRP-Docs/assets/2225711/a1b8cb1e-7f88-4061-b297-2691523718a5)

### De app werkte eerst, maar nu maakt hij oneindig verbinding.

Je hebt mogelijk een time-out van Discord gekregen vanwege het vaak verbinden/wijzigen van je aanwezigheid. Verbreek de verbinding, wacht 5-10 minuten en probeer opnieuw verbinding te maken. Het kan ook helpen om Discord opnieuw te starten.

### De app zegt "Verkeerde ID?" / "Is Discord actief?" of maakt oneindig verbinding, hoewel ik zeker weet dat ik alles goed heb gedaan en Discord actief is.

Hier zijn enkele dingen die je kunt proberen:
- **Zorg ervoor dat je een standalone Discord-client gebruikt (niet in de browser).**
- Herstart je pc. Tip: een pc-herstart lost vaak veel problemen op.
- Als je BetterDiscord/Vencord/etc geïnstalleerd hebt, verwijder het tijdelijk, laat CustomRP minstens één keer verbinding maken met Discord en installeer het dan opnieuw.
- Als je meerdere Discord-clients gebruikt, sluit dan tijdelijk alle clients behalve degene waarop je de aanwezigheid wilt hebben.
- Voer CustomRP uit als administrator.
- Voeg `%appdata%\CustomRP` of, in het geval van een draagbare versie, de map waarin je CustomRP hebt uitgepakt, toe aan de uitzonderingen van de firewall en/of antivirusprogramma's en herstart je pc volledig.
  - Als je niet zeker weet of je een antivirusprogramma hebt, heb je er hoogstwaarschijnlijk een - Windows Defender is aanwezig op elke computer met Windows 10/11.
- Herinstalleer Discord.

Als niets heeft geholpen, kan ik helaas niets anders voorstellen, sorry.

### De app blijft hangen op "Aanwezigheid bijwerken..."

Controleer de URL's van de afbeeldingen; ze zijn mogelijk te lang of geen directe links.

### De app werkte eerst, maar crashte toen en nu start hij helemaal niet meer op.

Misschien heb je een lange string met speciale tekens (of tekst in een taal met niet-Latijnse letters) in een veld ingevoerd en dat heeft de app laten crashen. Om dit op te lossen, druk op Win+R, typ `%localappdata%\maximmax42` en verwijder of hernoem mappen met CustomRP in de naam, start dan de app opnieuw. Let op dat dit de app volledig reset.

### De app blijft crashen bij het bijwerken/proberen te verbinden/enz.

Als je de app kunt starten en een crashrapport krijgt waarin staat `System.IO.FileNotFoundException: Could not load file or assembly...`, installeer de app dan opnieuw.

Als je geen antwoord op je vraag/probleem kunt vinden, stuur dan een bericht naar een `#support` kanaal op de [CustomRP Discord-server](https://www.customrp.xyz/discordserver), stuur een bericht naar maximmax42 op Discord of [open een probleem](https://github.com/maximmax42/Discord-CustomRP/issues/new/choose).
