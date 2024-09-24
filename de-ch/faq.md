---
beschribig: Häufig gstellti Fragä
---

# ❓ FAQ

## Fragä

### Chani meh als zwei chnöpf adde?

Nei, das isch e limitierig vo Discord

### Chani e anderi art vo aktivität awende (z.b. lost, luegt, streamt)?

Nei, das isch au e limitierig vo Discord

### Warum zeigt Discord nur t verblibeni stunde ah, wenni en ziitstempel für e paar täg i dä zuekunft istelle?

Du hesch es errate, ebefalls e limitierig vo Discord

### Wirds e Linux/Mac-Version gä?

S program isch mitere reine Windows_Bibliotek erstellt wordä, deswege würdi e Linux/Mac version bedütä, das sganze program mitere andere bibliotek/programmiersprach neu gschribe werde müesti, wasi momentan ned plane.

### Us irgendwelem grund öffnet sich es Fenster names "Pipe", was isch das?

Es öffnet sich, will du Strg+Umschalt druckt häsch und uf dä Schaltflächi verbinde klickt hesch (oder Strg und Verbinde oder widerverbinde im Tray-Icon-Menü bi ältere versione). Lass es bi -1 und schlüss es. Si wird für situatione verwended, wenn du meh als nur eis Discord Fenster offe hesch. Wenn du t Pipe-Nummere änderisch, chasch uswele i welem client du t präsenz ha wilsch.

## Fählerbehebig

Befor du irgendöbis probiersch, lueg nah heb du t neusti verion vo CustomRP hesch!

### Wenni uft chnöpf uf mim profil klicke funktionieret die ned.

T chnöpf funktionieret ufem Discord-Client wo du bruchsch meistens ned wege Discord. Chasch si aber am Handy oder Webclient teste oder öber andersch frögä. 

### I ha CustomRP installiert, aber es startet ned.

Höchstwarschindli verhinderet din Antivirus dä start. Du muesch den dä Ordner "%appdata%\CustomRP" it usnahme adde.

### Ich habe CustomRP installiert, Analytiks erlaubt und die App funktioniert nicht mehr.

Beende die App im Task Manager, Lösche den `%localappdata%\maximmax42` Ordner, starte die App neu und erlaube die Analytiks nicht.

### Die App hat sich verbunden, aber Ich sehe den Status nicht in meinem Profil.

Stelle sicher, dass du den Aktivitätsstatus in den Discord-Einstellungen aktiviert hast:

<figure><img src="https://user-images.githubusercontent.com/115729033/195649622-ab1f09fc-4499-4421-a515-ba869fc40470.PNG" alt=""><figcaption></figcaption></figure>

### Die App hat funktioniert, aber jetzt Verbindet er sich unendlich.

Es kann sein, dass du eine Zeitüberschreitung von Discord erhalten hast, weil du zu häufig die verbinden oder die Präsenz wechseln. Trenne die Verbindung, warte 5-10 Minuten und versuche erneut, dich zu verbinden. Ein Neustart von Discord könnte auch helfen.

### Die App sagt "Falsche ID?"/"Läuft Discord?" oder verbindet sich auf unbestimmte Zeit, obwohl ich sicher bin, dass ich alles richtig gemacht habe und Discord läuft.

Manchmal wird dies durch BetterDiscord verursacht. Wenn du es installiert hast, deinstallieren es, lasse CustomRP mindestens einmal eine Verbindung zu Discord herstellen und installieren dann BD wieder. Wenn nicht, versuche CustomRP als Administrator zu starten. Wenn das nicht hilft, versuche, `%appdata%\CustomRP` oder, falls du eine portable Version verwendest, den Ordner, in dem du CustomRP extrahiert hast (und vielleicht Discord), zu den Firewall-/Antivirus-Ausnahmen hinzuzufügen, und starte dann deinen gesamten PC neu (Du könntest versuchen, nur Discord und CustomRP neu zu starten, aber in 95% der Fälle funktioniert das nicht). Du könntest auch versuchen, alle Discord-Clients außer Ihrem Hauptclient vorübergehend zu beenden. Wenn das nicht hilft, konnte ich nie herausfinden, was die Ursache dafür ist, tut mir leid.

### Die App hat davor funktioniert, aber dann ist sie gecrasht und startet jetzt gar nicht mehr.

Vielleicht hast du einen langen Text (oder einen Text in einer Sprache, die nicht lateinische Buchstaben verwendet) in ein Feld eingefügt, und das hat die Anwendung zum Absturz gebracht. Um dies zu beheben, drücke Win+R, gebe `%localappdata%\maximmax42` ein und löschen oder benenne Ordner mit CustomRP im Namen um, dann starte die App. Beachte, dass die Anwendung dadurch vollständig zurückgesetzt wird.

### Die App stürzt beim Aktualisieren/Verbinden/usw. ständig ab.

Wenn du in der Lage bist, die Anwendung zu starten und einen Absturzbericht zu erhalten, und es heißt `System.IO.FileNotFoundException: Could not load file or assembly...`, installiere die Anwendung bitte neu.

Wenn du keine Antwort auf deine Frage/dein Problem findest, senden eine Nachricht in den `#Support`-Channel auf dem [CustomRP Discord Server](https://www.customrp.xyz/discordserver), oder schreibe mir eine Direkt-Nachricht auf Discord (maximmax42#5572) oder [open an issue](https://github.com/maximmax42/Discord-CustomRP/issues/new/choose).
