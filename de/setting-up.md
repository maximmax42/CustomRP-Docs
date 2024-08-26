---
description: RTFM
---

# 🛠️ Einrichtung

{% hint style="warning" %}
Diese Seite könnte veraltet sein. Bitte lesen Sie die [englische Version dieser Seite](https://app.gitbook.com/s/5gJfBQC2iWNK0J953fo2/setting-up) für die aktuellen Informationen.
{% endhint %}

Wenn du irgendwelche Fehler hast, lese bitte das [FAQ](faq.md).

Vergewisser dich vor dem Einrichten, dass du den Aktivitätsstatus in den Discord-Einstellungen aktiviert hast:

<figure><img src="https://user-images.githubusercontent.com/115729033/195649622-ab1f09fc-4499-4421-a515-ba869fc40470.PNG" alt=""><figcaption></figcaption></figure>

## Einrichtungsvorgang

* Gehe zu https://discord.com/developers/applications/.
* Drücke **New Application** in der oberen rechten Ecke.

![image](https://user-images.githubusercontent.com/2225711/161050202-c796103d-6712-401e-be96-3f3712512375.png)

* Wähle den Namen für die Anwendung, er wird nach "Spielt" im Status angezeigt; drücke **Create**.
* Kopiere die **Application ID** und füge sie in das Feld **ID** in Custom RP ein, dann drücke **Verbinden**. Wenn du das richtig gemacht hast, sollte dein Status in Discord jetzt "Spielt **\[Name der app]** anzeigen".
  * Hinweis: Wenn du einen benutzerdefinierten Status eingestellt hast (der mit dem Emoji), hat dieser Vorrang vor deinem CustomRP-Status. Er wird jedoch im Profil-Popup angezeigt.

![image](https://user-images.githubusercontent.com/2225711/161050341-8169af53-5d3f-44d6-b745-cc711e8d1476.png)

* Auf deiner Anwendungsseite, gehe zu Rich Presence -> Art Assets und lade mindestens ein Bild unter Rich Presence Assets hoch, wenn du dieses verwenden möchtest. In CustomRP gibt es eine praktische Schaltfläche **Assets Hochladen** im Menü (Du kannst auch Ctrl+U verwenden), das wird dich auf die richtige Seite bringen, insofern deine ID richtig eingestellt ist.
  * Alternativ kannst du auch einfach eine URL zu dem Bild in das Feld **Key** eingeben.
  * Hinweis: Du kannst deinen Assets zwar einen beliebigen Namen mit bis zu 999 Symbolen geben, die API akzeptiert jedoch nur Namen mit maximal 256 Symbolen.
* Navigiere zur Seite Visualizer, um die Felder **State, Details, Large Image Key, Large Image Text, Small Image Key, Small Image Text, Party Size, Party Max** einzurichten. Alle diese Angaben sind optional.
* Wenn du die für dich passende Einstellung gefunden hast, kopiere die Werte in die entsprechenden Felder von CustomRP.
  * Tipp: Du kannst mit dem Mauszeiger über fast jedes Steuerelement in der App hovern (einschließlich der Label-Zeile **Details**) und du erhälten einen Tooltip!
* Wenn du auch Knöpfe einrichten möchtest, fülle die beiden Felder Text und URL aus.
  * Hinweis: Wenn du in deiner eigenen Aktivität auf die Schaltflächen klickst, funktionieren sie nicht, aber keine Sorge, sie funktionieren für alle anderen. Das ist ein Problem von Discord.
* Klicke auf **Aktualisiere Präsenz** (oder **Verbinden**, wenn du noch nicht verbunden bist).
* Herzlichen Glückwunsch, du bist wunderbar!

### Ich verwende mehr als einen Discord-Client, was soll ich tun?

Wenn du mehr als einen Discord-Client hast und du möchtest, dass deine Anwesenheit auf einem anderen Konto als dem von der App automatisch ausgewählten angezeigt wird, drücke bitte **Trennen**, halte dann Strg+Umschalttaste auf deiner Tastatur und drücke **Verbinden**. Es öffnet sich ein Fenster mit einer Zahleneingabe, gebe hier die Zahl 1 ein, schließe das Fenster und drücken Sie erneut **Verbinden**, ohne Strg+Umschalttaste. Falls es sich wieder um ein falsches Konto handelt, versuche es mit der Zahl 0, dann mit der 2 und so weiter bis zur 9.

Bitte beachte, dass wenn du mehrere Discord-Clients beim Start ausführen lässst, die jedem Client zugewiesene Pipe-Nummer möglicherweise nicht von Start zu Start erhalten bleibt und sich ändern kann, je nachdem, welcher Client zuerst gestartet wurde. Um dies zu verhindern, kannst du entweder zusätzliche Clients manuell starten oder den Windows Task Scheduler verwenden, um den Start der Clients zu verzögern.

Wenn du 2 Konten hast, die du gleichzeitig verwendst und für jedes eine andere Aktivität haben möchtest, gehe wie folgt vor:

* Richte zunächst dein Hauptkonto gemäß den obigen Anweisungen ein.
* Hole dir die neueste **portable (.zip)** Version von CustomRP (entweder von der [Website](https://www.customrp.xyz) oder der [GitHub-Releaseseite](https://github.com/maximmax42/Discord-CustomRP/releases/latest)) und entpacke sie irgendwo.
  * Dies funktioniert nur mit den Versionen 1.16 und älter.
* Öffne die `Start Second Instance.bat` oder erstelle eine Verknüpfung zu CustomRP.exe mit dem Argument `--second-instance` (oder `-2`).
* Richte das Programm auf die gleiche Weise ein wie die erste Hauptinstanz.
  * Tipp: Wenn du bereits eine Voreinstellung hast, die du mit deiner zweiten Instanz verwenden möchten, kannst du die Bat-Datei oder die Verknüpfung so bearbeiten, dass sie den Pfad zur Voreinstellung enthält. Beispiel: `CustomRP.exe -2 "C:\Some Folder\preset.crp"` (Anführungszeichen um den Pfad sind notwendig, wenn der Pfad Leerzeichen enthält).
* Änder vor dem Anschluss die pipe wie zuvor beschrieben und schließe sie an.

Wenn du 3 oder mehr Konten gleichzeitig verwendest, dann... warum? Aber auch wenn genug von euch mich nerven werden, werde ich Unterstützung für die Verwendung von mehr Instanzen hinzufügen.

## Hinweise

* Wenn du kein kleines oder großes Bild einrichten möchtest, lasse alle entsprechenden Felder im Programm leer.
* Wenn kein großes Bild eingestellt ist, werden die Einstellungen für das kleine Bild ignoriert.
