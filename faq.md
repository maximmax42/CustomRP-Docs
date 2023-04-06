---
description: Întrebări frecvente
---

# ❓ FAQ

## Întrebări

### Pot să adaug mai mult de 2 butoane?

Nu, este o limitare de la Discord.

### Pot folosi un alt tip de activitate (e.g. listening, watching, streaming)?

Nu, este tot o limitare de la Discord.

### De ce dacă setez un marcaj temporal de câteva zile în viitor, Discord arată doar câte ore au mai rămas?

Ai ghicit, este tot o limitare de la Discord.

### Va exista o versiune Linux / Mac?

Aplicația este construită folosind o bibliotecă doar pentru Windows, prin urmare, sprijinirea Linux și Mac ar însemna rescrierea întregii aplicații într-o altă bibliotecă / limbaj de codificare pe care nu se poate planifica încă.

### O fereastră numită "Pipe" s-a deschis dintr-un motiv oarecare, ce este aceasta?

S-a deschis deoarece ați apăsat Ctrl+Shift și ați făcut clic pe butonul Connect (sau Ctrl si Connect sau Reconnect în meniul pictogramei pe versiunile mai vechi). Lăsați-l la -1 și închideți-l. Este folosit pentru situațiile în care aveți mai mult de un client Discord care rulează în același timp. Schimbarea numărului de pipe alege în mod eficient clientul în care doriți să vă aflați prezența.

## Rezolvarea Problemelor

Înainte de a încerca ceva, asigurați-vă că sunteți pe cea mai recentă versiune de CustomRP!

### Când fac clic pe butoanele de prezență din profilul meu, acestea nu funcționează.

Butoanele nu vor funcționa pentru tine pe clientul desktop cu care folosești CustomRP, este o ciudatenie a Discord-ului. Puteți testa butoanele de la clientul mobil sau web sau pur și simplu întrebați pe altcineva în schimb.

### Am instalat CustomRP, dar nu pornește.

Acesta este cel mai probabil antivirusul care împiedică lansarea aplicației. Adaugați folderul `%appdata%\CustomRP` la excepții.

### Am instalat CustomRP, am permis analytics și aplicația nu mai funcționează.

Închideți aplicația în Task Manager, ștergeți folderul `%localappdata%\maximmax42` , porniți din nou aplicația și nu permiteți analytics.

### Aplicația s-a conectat, dar nu văd starea în profilul meu.

Asigurați-vă că ați activat starea activității în setările Discord:

<figure><img src="https://user-images.githubusercontent.com/2225711/188219661-49713f90-fa76-4645-b04a-fc1bc0f029bd.png" alt=""><figcaption></figcaption></figure>

### Aplicația funcționa, dar acum se conectează la nesfârșit.

Este posibil să fi obținut un timeout de la Discord din cauza conectării / schimbării prezenței foarte mult. Deconectați-vă, așteptați 5-10 minute, încercați să vă conectați din nou. Repornirea Discord-ului ar putea ajuta.

### Aplicația spune "ID greșit?" /"Discord rulează?" sau se conectează la nesfârșit, chiar dacă sunt sigur că am făcut totul bine și Discord rulează.

Uneori, acest lucru este cauzat de BetterDiscord. Dacă îl aveți instalat, dezinstalați-l, lăsați CustomRP să se conecteze la Discord cel puțin o dată și apoi instalați BD înapoi.

Dacă nu aveți BD sau nu v-a ajutat, încercați să rulați CustomRP ca administrator. Dacă acest lucru nu vă ajută, încercați să adăugați `%appdata%\CustomRP` sau, în cazul în care utilizați o versiune portabilă, folderul în care ați extras CustomRP (sau poate Discord), la excepțiile firewall/antivirus, și apoi reporniți întregul PC (ați putea încerca să reporniți doar Discord și CustomRP, dar în 95% din cazuri nu funcționează). Un alt lucru pe care îl puteți încerca este să renunțați temporar la toți clienții Discord, dar nu la cel principal. În cazul în care nu ajută, niciodată nu am putut da seama ce cauzează acest lucru, îmi pare rău.

### Aplicația funcționa înainte, dar apoi s-a oprit și acum nu se lansează deloc.

Poate că ați introdus un șir lung de fancy text (sau text într-o limbă care utilizează litere non-latine) într-un câmp și care a oprit aplicația. Pentru a remedia acest lucru, apăsați Win+R, scrieți `%localappdata%\maximmax42` și ștergeți sau redenumiți folderele cu CustomRP în nume, apoi porniți aplicația. Rețineți că acest lucru resetează complet aplicația.

### Aplicația continuă să se oprească atunci când se actualizează / încearcă să se conecteze / etc.

Dacă reușiți să lansați aplicația și să obțineți un raport de oprire și se spune `System.IO.FileNotFoundException: Could not load file or assembly...`, vă rugăm să reinstalați aplicația.

Dacă nu găsiți un răspuns la întrebarea/problema dvs., trimiteți un mesaj către canalul `#support` în [Server-ul de Discord CustomRP](https://www.customrp.xyz/discordserver), scrieți creatorului maximmax42#5572 pe Discord sau [deschideți o problemă pe GitHub](https://github.com/maximmax42/Discord-CustomRP/issues/new/choose).
