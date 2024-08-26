---
description: RTFM
---

# 🛠️ Configurare

{% hint style="warning" %}
Această pagină ar putea fi depășită. Vă rugăm să consultați [versiunea în limba engleză a acestei pagini](https://app.gitbook.com/s/5gJfBQC2iWNK0J953fo2/setting-up) pentru informații actualizate.
{% endhint %}

Dacă întâmpinați erori, consultați [FAQ](faq.md).

Înainte de configurare, asigurați-vă că ați activat starea activității în setările Discord:

<figure><img src="https://user-images.githubusercontent.com/2225711/188219661-49713f90-fa76-4645-b04a-fc1bc0f029bd.png" alt=""><figcaption></figcaption></figure>

## Procesul de instalare

* Mergeți la https://discord.com/developers/applications/.
* Click **New Application** în colțul din dreapta sus.

![image](https://user-images.githubusercontent.com/2225711/161050202-c796103d-6712-401e-be96-3f3712512375.png)

* Alegeți numele aplicației, acesta va fi afișat după statusul "Playing"; apasați **Create**.
* Copiați **Application ID** și lipiți-l în câmpul **ID** din Custom RP, după apăsați **Connect**. Dacă este făcut corect, starea ta în Discord ar trebui să spună acum "Playing **\[numele aplicatiei]**".
  * Notă: Dacă aveți un custom status setat (cel cu emoji), acesta va fi prioritizat față de cel din CustomRP. Totuși, va fi văzut în profilul pop-up.

![image](https://user-images.githubusercontent.com/2225711/161050341-8169af53-5d3f-44d6-b745-cc711e8d1476.png)

* Pe pagina aplicației, navigați la Rich Presence -> Art Assets și încărcați cel puțin o imagine sub Rich Presence Assets dacă doriți să le utilizați. În CustomRP, există un buton util **Upload Assets** in meniul File (puteți utiliza și Ctrl+U) care vă va duce acolo dacă câmpul ID este configurat corect.
  * Alternativ, puteți insera doar un link direct la imagine în câmpul **Key**.
  * Notă: Deși vă puteți denumi resursa cu orice nume de până la 999 de simboluri, API-ul va accepta doar nume cu maximum 256 de simboluri.
* Navigați la pagina Vizualizer pentru a configura câmpurile **State, Details, Large Image Key, Large Image Text, Small Image Key, Small Image Text, Party Size, Party Max**. Toate acestea sunt opționale.
* După ce ați găsit configurarea care vă place, copiați valorile în câmpurile corespunzătoare CustomRP.
  * Sfat: Puteți trece cu mouse-ul peste aproape orice control din aplicație (inclusiv linia de etichete **Details**) și vă va oferi un sfat!
* Dacă doriți să configurați și butoane, completați atât câmpurile Text, cât și URL.
  * Notă: Când veți face clic pe butoane în propria prezență, acestea nu vor funcționa, dar nu vă faceți griji, vor funcționa pentru toți ceilalți. E o problemă în partea de Discord.
* Apăsați **Update Presence** (sau **Connect** dacă nu sunteți deja conectat).
* Felicitări, ați terminat!

### Folosesc mai mult de un client Discord, ce fac?

Dacă aveți mai mult de un client Discord și doriți ca prezența dumneavoastră să apară pe un cont diferit de cel ales automat, vă rugăm să apăsați **Disconnect**, apoi țineți apăsat Ctrl+Shift de pe tastatură și apăsați **Connect**. O fereastră cu o intrare de număr va apărea, puneți un număr 1, închideți fereastra și apăsați **Connect** din nou, fără Ctrl+Shift. În cazul în care este un cont greșit din nou, încercați numărul 0, apoi 2 și așa mai departe până la 9.

Vă rugăm să rețineți că, dacă aveți mai mulți clienți Discord care rulează la pornire, numărul pipe atribuit fiecarui client este posibil să nu fie persistent de la boot to boot și se poate schimba în funcție de clientul care a început prima dată. Pentru a preveni acest lucru, aveți posibilitatea să porniți clienții suplimentari manual sau să utilizați Windows Task Scheduler pentru a întârzia pornirea clienților.

Dacă aveți 2 conturi pe care le utilizați în același timp și doriți ca fiecare dintre ele să aibă o prezență diferită, urmați acești pași:

* Configurați-vă mai întâi contul principal cu instrucțiunile de mai sus.
* Descărcați cea mai recentă versiune **portable (.zip)** de CustomRP (fie de pe [Pagina de Web](https://www.customrp.xyz) sau [Pagina de lansări GitHub](https://github.com/maximmax42/Discord-CustomRP/releases/latest)) și dați extract oriunde.
  * Acest lucru funcționează numai cu versiunile 1.16 și mai vechi.
* Deschideți `Start Second Instance.bat` sau creați o comandă rapidă la CustomRP.exe cu un argument `--second-instance` (sau `-2`).
* Configurați programul în același mod în care ați făcut instanța principală.
  * Sfat: Dacă aveți deja o presetare pe care doriți să o utilizați cu a doua instanță, puteți edita fișierul bat sau comanda rapidă pentru a include calea către presetare. Exemplu: `CustomRP.exe -2 "C:\Nume Folder\preset.crp"` (ghilimelele din jurul traseului sunt necesare dacă traseul are spații în el).
* Înainte de conectare, schimbați pipe-ul așa cum este descris mai devreme și conectați-vă.

Mesaj de la Creator: Dacă utilizați 3 sau mai multe conturi în același timp, atunci ... de ce? Dar și dacă mulți dintre voi mă certați, Voi adăuga suport pentru utilizarea mai multor instanțe.

## Notițe

* Dacă nu doriți să configurați imagini mici sau mari, lăsați necompletate toate câmpurile asociate din program.
* Dacă imaginea mare nu este setată, setările mici ale imaginii vor fi ignorate.
