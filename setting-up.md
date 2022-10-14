---
description: LVM
---

# 🛠 Järjestely

Jos koet ongelmia, katso [UKK](faq.md#questions).

Ennen kuin aloitat, tarkista että olet valtuuttanut Discordin näyttämään toimintasi tilaviestinä.

<figure><img src=".gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

## Järjestely prosessi

* Mene [https://discord.com/developers/applications/.](https://discord.com/developers/applications/)
* Paina **New Application** oikeassa yläkulmassa.

![image](https://user-images.githubusercontent.com/2225711/161050202-c796103d-6712-401e-be96-3f3712512375.png)

* Valitse applikaation nimi, se esiintyy "Pelaa Peliä" jälkeen; paina **Create**.
* Kopioi **Application ID** ja liitä se customRP'n **ID** Kohtaan ja paina **Yhdistä**. Jos tehty oikein, Toimintasi Discordissa pitäisi nyt lukea "Pelaa: **\[nimi jonka valitsit {esim; 2022}]**".
  *   Huomaa: Jos sinulla on mukautettu tila (se jossa on emoji), se tulee CustomRP tilan päälle. Mutta näkyy profiilin toiminta kohdassa.

      <figure><img src=".gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>
* Applikaatiosi sivulla, mene Rich Presence -> Art Assets ja lisää ainakin yksi kuva Rich Preseesenssin alle. Jos haluat käyttää niitä CustomRP'ssä, Siellä on kätevä Lähetä Tiedostoja nappi **Tiedosto** valikossa. (Voit myös käyttää Ctrl+U) joka vie sinut sinne jos ID kohtasi on aseteltu oikein.
  * Vaihtoehtoisesti, voit myös vain liittää URL'n kuvaan **Key** Kohdassa
  * Muista: Vaikka voitkin nimetä kohdan 999 symbooliin asti, API Hyväksyy nimiä jossa on vain 256 symboolia maksimissaan.
* Navigoi Visualizer sivulle asetellaaksi kohdat; **State, Details, Large Image Key, Large Image Text, Small Image Key, Small Image Text, Party Size, Party Max**. Kaikki näistä on valinnaisia.
* Kun olet löytänyt asetuksen josta tykkäät, Kopioi kaikki kohdat CustomRP's vastaaviin kohtiin.
  * Vihje: Voit laittaa hiiresi melkein minkä vaan päälle (mukaan lukien **Details**) ja se antaa sinulle ohjeita!
* Jos haluat asetella painikkeet myös, täytä molemmat Text ja URL kentät.
  * Muista: Kun painat omia painikkeitasi, ne eivät toimi, mutta älä huoli!, ne toimii muille, tämä on ongelma Discordin puolella.
* Paina **Päivitä läsnäoloa** (tai **Yhdistä** jos et ole jo yhdistänyt.)
* Onnittelut, olet mahtava!

### Käytän enemmän kuin yhtä Discord ohjelmaa. Mitä teen?

Jos käytät enemmän kuin yhtä Discord ohjelmaa, ja toivoisit että tilasi näkyisi jollain muulla ohjelmalla kun se jonka CustomRP automaattisesti valitsi, paina **Disconnect** ja pidä pohjassa **Ctrl + Shift** nappeja näppäimistölläsi ja paina **Yhdistä**. Sovellus jossa on numero syöttö tulee näkymään, laita numero 0, sulje, ja paina **Yhdistä**, ilman Ctrl+Shift. Jos se oli väärä tili uudestaan, yritä numero 1, sitten 2 ja jatka numero 9 asti.

Muista että jos sinun monta Discord ohjelmaa käynnistyy tietokoneesi mukana, pipe numero valittu joka ohjelmaan ei välttämättä pysy samana uudelleen käynnistyksen jälkeen. Ja voi vaihtua sen mukaisesti mikä ohjelmista käynnistyi ensin. Varoaksesi tätä, voit joko käynnistää monta ohjelmaa manuaalisesti, tai käyttää Windows Task Scheduleria jotta voit hidastaa tiettyjen ohjelmien käynnistysaikoja.

Jos sinulla on 2 tiliä jota käytät samaan aikaan ja haluat jokaisen niistä käyttämään eri tilaa, tee nämä askeleet;

* Asettele oma pää-tilisi ensin näillä ohjeilla.
* Lataa uusin **portable (.zip)** versio CustomRP'stä (joko  [nettisivulta](https://www.customrp.xyz) tai [GitHub julkaisu sivulta](https://github.com/maximmax42/Discord-CustomRP/releases/latest)) ja pura se minne vaan.
  * Tämä vain toimii versioilla 1.16 ja vanhemmilla.
* Avaa `Start Second Instance.bat` tai tee oikotie CustomRP.exe en argumentilla `--second-instance` (tai `-2`).
* Asettele sovellus samalla tavalla mitä teit pää-instanssilla.
  * Vihje: Jos sinulla on jo esiasetus jota haluat käyttää toisella instanssillasi, voit editoida .bat tiedostoa tai oikotietäsi to sisällyttämään reitin esiasetukseesi. Example: `CustomRP.exe -2 "C:\Joku Kansio\esiasetuksesi.crp"` (sitaatit reitin ulkopuolella on tarvittuja jos reitissä on välilyöntejä).
* Ennen kuin yhdistät, vaihda pipe kuten kuvattu aiemmin ja yhdistä.

Jos käytät 3 tai enemmän tiliä samaan aikaan, sitten... miksi? Mutta jos tarpeeksi teistä valittaa tarpeeksi, mahdollistan sen.

## Muistiinpanot

* Jos et halua kuvia, jätä kaikki kuvakentät tyhjäksi.
* Jos isoa kuvaa ei ole, pientä kuvaa ei myöskään tule näkymään.
