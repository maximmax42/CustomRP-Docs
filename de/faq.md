---
description: Häufig gestellte Fragen
---

# ❓ FAQ

{% hint style="warning" %}
Diese Seite könnte veraltet sein. Bitte lesen Sie die [englische Version dieser Seite](https://app.gitbook.com/s/5gJfBQC2iWNK0J953fo2/faq) für die aktuellen Informationen.
{% endhint %}

## Fragen

### Kann ich mehr als Zwei Knöpfe hinzufügen?

Nein, es ist eine Limitierung von Discord

### Kann ich eine andere Art von Aktivität verwenden (z.B Hört, Guckt, Streamt)?

Nein, es ist auch eine Limitierung von Discord

### Warum zeigt Discord nur die verbleibenden Stunden an, wenn ich einen Zeitstempel für einige Tage in der Zukunft einstelle?

Du hast es erraten, es ist auch eine Limitierung von Discord

### Wird es eine Linux/Mac-Version geben?

Die Anwendung wurde mit einer reinen Windows-Bibliothek erstellt, daher würde die Unterstützung von Linux und Mac bedeuten, dass die gesamte Anwendung in einer anderen Bibliothek/Programmiersprache neu geschrieben werden müsste, was ich derzeit noch nicht plane.

### Aus irgendeinem Grund öffnete sich ein Fenster namens "Pipe", was ist das?

Es öffnete sich, weil du Strg+Umschalt gedrückt hast und auf die Schaltfläche Verbinden geklickt hast (oder Strg und Verbinden oder Wiederverbinden im Tray-Icon-Menü bei älteren Versionen). Belasse es bei -1 und schließe es. Sie wird für Situationen verwendet, in denen du mehr als einen Discord-Client gleichzeitig laufen hast. Wenn du die Pipe-Nummer änderst, kannst du auswählen, in welchem Client du die präsens haben möchtest.

## Fehlerbehebung

Bevor du irgendetwas probierst, stelle sicher das du die letzte Version von CustomRP benutzt!

### Wenn ich auf die Knöpfe in meinem Profil drücke, funktioneren sie nicht.

Die Knöpfe werden auf dem Desktop-Client, mit dem du CustomRP verwendest, nicht funktionieren, das ist eine Eigenart von Discord. Du kannst die Schaltflächen über den mobilen oder Web-Client testen oder stattdessen einfach jemand anderen fragen.

### Ich habe CustomRP installiert, aber es startet nicht.

Höchstwahrscheinlich verhindert dein Antivirusprogramm den Start der Anwendung. Füge den Ordner "%appdata%\CustomRP" zu den Ausnahmen hinzu.

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
