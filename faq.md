---
description: Usein Kysyttyjä Kysymyksiä
---

# ❓ UKK

## Kysymyksiä

### Voinko lisätä yli kaksi painiketta?

Ei, Discord ei anna sinun tehdä näin.

### Voinko käyttää erilaista tila tyyppiä (esim Kuuntelee, katsoo, striimaa?

Ei, Discord ei anna sinun tehdä tätä myöskään.

### Miksi jos teen ajasta monta päivää tulevaisuuteen, Discord vain näyttää monta tuntia on jäljellä?

Arvasit, Discord ei anna sinun tehdä sitäkään.

### Tuleeko Linux/Mac versiota?

Sovellus on tehty ohjelmakirjostolla pelkästään Windowsille, joten Linux tai Mac versio tarkoittaa koko sovelluksen uudelleen koodamista toisella koodauskielellä. Tästä en ole vielä ajatellut.

### "Pipe" sovellus aukesi jostakin syystä, mikä tämä on?

Se aukesi koska painoit Ctrl+Shift kun painoit yhdistä painiketta. (Tai Ctrl ja yhdistä painiketta tai Yhdistä uudelleen oikeassa alakulmassa olevassa CustomRP'ssä). Jätä se -1 ja sulje se. [Mitä tämä tekee](faq.md#voinko-lisaetae-yli-kaksi-painiketta)?

## Vianetsintä

Ennen kuin yrität mitään, tarkista että käytät CustomRP'n uusinta versiota!

### Kun painan painikkeita tilassani, ne ei toimi.

Painikkeet eivät toimi samalla Discord ohjelmalla johon olet yhdistänyt CustomRP'n, ne kyllä toimii ja voit tarkistaa sen käyttämällä toista Discord ohjelmaa tai Discordin nettisivu versiota.

### Asensin CustomRP'n ja se ei käynnisty.

Tämä yleensä tarkoittaa että antiviiruksesi estää sitä. Lisää `%appdata%\CustomRP` kansio poikkeukseesi.

### Asensin CustomRP'n, sallin analyytikat ja sovellus ei toimi enään.

Tapa sovellus tehtävänhlalinnassa, poista `%localappdata%\maximmax42` kansio, käynnistä sovellus uudestaan ja älä salli analyytikoita.

### Sovellus on yhdistetty, mutta en nää tilaa Discord tililläni.

Tarkista että olet valtuuttanut Discordin näyttämään toimintasi tilaviestinä. &#x20;

<figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

### Sovellus toimi ennen, mutta nyt se yhdistää loputtomiin.

Sinä ehkä sait aikakatkaisun Discordilta sen takia että yhdistit ja katkaisit likaa, odota 5-10 minuuttia, ja yritä uudestaan. Discordin uudelleenkäynnistäminen voi myös auttaa.

### Sovellus sanoo "väärä ID?/Onko Discord käynnissä?" Tai yhdistää loputtomiin vaikka olen varma että tein kaiken oikein ja Discord on käynnissä.

BetterDiscord usein tekee tämän. Jos sinulla on se, poista se, anna CustomRP'n yhdistää Discordiin ainakin kerran, ja asenna BetterDiscord uusiksi. Jos et, käynnistä CustomRP järjestelmänvalvojana. Jos se ei auta, lisää  `%appdata%\CustomRP` tai, jos käytät portable-versiota, kansio johon pursit BetterDiscordin (ja ehkä Discord) palomuurin tai antiviiruksesi poikkeuksiin, ja käynnistä tietokoneesi uudestaan (voit myös yrittää käynnistää vain Discordin ja CustomRP'n uudelleen, Mutta yli 95% ajasta se ei toimi. Voit myös yrittää sulkea kaikki Discord ohjelmasi paitsi pää versiosi. Jos se ei auta, minulla ei ole mitään hajua miten korjata sitä, anteeksi.

### Sovellus toimi ennen, sammui virheen takia ja ei enään käynnisty.

Ehkä olet laittanut paljon tekstiä hienolla fontilla (tai kielessä joka ei ole latitan kirjaimissa {äö myös}) kohtaan ja se aiheutti tämän. Korjaattaaksesi, paina win+r, kirjoita `%localappdata%\maximmax42` ja poista tai vaihda kansioiden nimiä jossa on CustomRP niiden nimiss, ja käynnistä CustomRP. Huomaa että tämä poistaa kaiken jota kirjoitit.

### Sovellus sammuu kun yhdistän, päivitän jotain, jne.

Jos voit käynnistää sovelluksen, ja saat virheraportin; `System.IO.FileNotFoundException: Could not load file or assembly...`, käynnistä sovellus uudestaan

Jos et löydä vastausta kysymykseesi, lähetä viesti `#support` kanavalle [CustomRP Discordissa](https://www.customrp.xyz/discordserver), tai laita yksityisviestiä jes#8137, tai (ei englantia puhuva) maximmax#5572 or [avaa ongelma](https://github.com/maximmax42/Discord-CustomRP/issues/new/choose).
