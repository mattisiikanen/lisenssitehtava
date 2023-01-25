# Lisenssitehtävä
Lukuläksy:</br>
Aiheesta tuli ensin lukea kahdesta eri linkistä ja tiivistää asia ranskalaisin viivoin.
- Ilmaisesta ohjelmistosta voidaan myydä kopioita
- Neljä tärkeintä vapautta:
	- Ohjelman ajon vapaus
	- Vapaus tutkia ohjelman koodia ja muokata sitä mielen mukaan
	- Vapaus jaella kopioita siitä
	- Vapaus jakaa kopioita omasta versiosta
- Ilmainen ohjelmisto voi olla kaupallinen
- Copyleft suojaa lisenssin väärinkäytökseltä
- Rajoituksia voi tulla valtiollisella tasolla
- Tietoa lisensseistä ja lisensoinnista voi pyytää osoitteesta: licensing@gnu.org
- Lisenssien lisäksi myös ilmaiseen ohjelmistoon tulee olla tarjolla ilmainen manuaali

# Ympäristö
Hyper-V kotikoneella (Host):

CPU: i5-9600K
RAM: 16Gb
HDD: 120Gb
Win 11 Pro x64
Virtuaalikoneen speksit:

2 x CPU
4 Gb RAM
50 Gb HDD
Generation 2 (Hyper-V pyytää määrittelemään)

# Lisenssit
Aloitin hommat 25.01.2023 klo 15.00 käynnistämällä virtuaalikoneeni ja kirjautumalla sinne sisään.
Tehtävänä oli tarkastella viime viikolla testattuja vapaavalintaisten ohjelmien lisenssejä / lisenssitietoja.
Löysin lisenssitiedot kansiosta ```/usr/share/doc$```.

## Terminator
Avasin Terminatorin copyright tiedoston kansiossa ```/usr/share/doc/terminator$``` käyttämällä komentoa: ```micro copyright``` </br>
![Kuva1](https://user-images.githubusercontent.com/122887740/214572201-e7352685-b0c6-42f0-8c6e-5322392f11ae.png)</br>
Tietojen mukaan Terminator käyttää GPL-2.0 lisenssiä, eli GNU General Public License, version 2, kyseessä on ilmainen lisenssi.
Lisenssin mukaan käyttäjän tulee hyväksyä lisenssi, mikäli hän haluaa tehdä muutoksia, jaella tai kopioida sitä. </br>
Tarkastelin kyseisen lisenssin tietoja sivulta: https://www.gnu.org/licenses/old-licenses/gpl-2.0.html

Tämän ohjelman lisenssien kanssa ei ollut epäselvyyksiä.

## Terminology
Terminologyn kansiosta ```/usr/share/doc/terminology$``` löytyi copyright-niminen tiedosto, jonka sai auki komennolla: ```less copyright``` </br>
![Kuva2](https://user-images.githubusercontent.com/122887740/214574101-fc456452-7aee-42c9-b699-af148051229d.png)</br>
Copyright tietojen mukaan ohjelma käyttää nykyään BSD-2-clause, public-domain sekä SIL-OFL-1.1 lisenssejä. Lisenssit näyttävät olevan jaoteltu ohjelman eri osien välillä. Tarkastelin BSD-2-clause lisenssiin liittyviä ehtoja sivulta: https://choosealicense.com/licenses/bsd-2-clause/, public-domainista: https://www.idmanagement.gov/license/ ja SIL-OFL-1.1: https://en.wikipedia.org/wiki/SIL_Open_Font_License.

### BSD-2-clause
- Ilmainen
- Päätelty copyright tiedostosta
- Jakaessa, kopioitaessa tai luodessa tulee sisällyttää BSD:n lisenssilauseke ohjelmaan, muuten ei saa julkaista.

### public-domain
- Hylätty / vanhentuneet ehdot
- Päätelty copyright tiedostosta
- Ei ole oikeusvaikutuksia

### SIL-OFL-1.1
- Ilmainen
- Päätelty copyright tiedostosta
- Muokkaukset tulevat olla Open Font License alaisia, muuten voi tulla oikeusvaikutuksia

Tämän ohjelman lisenssien kanssa ei ollut epäselvyyksiä.

## GNOME Terminal
Viimeisenä ohjelmana minulla oli GNOME Terminal ja sen tiedot löytyivät ```/usr/share/doc/gnome-terminal``` copyright-tiedoston alta käyttämällä komentoa: ```micro copyright``` </br>
Ohjelman CopyRightista löytyi jälleen useampaa eri lisenssiä: GPL-3+, GFDL-NIV-1.3, LGPL-3+ </br>


### GPL-3+ (GNU GENERAL PUBLIC LICENSE)
- Ilmainen
- Päätelty copyright tiedostosta
- käyttäjän tulee hyväksyä lisenssi, mikäli hän haluaa tehdä muutoksia, jaella tai kopioida sitä

### GFDL-NIV-1.3 (GNU Free Documentation License v1.3)
- Vanhentunut, ilmainen
- Päätelty copyright tiedostosta
- Kopiointi ja jakaminen on sallittua, mutta muokkaus ei ole

### LGPL-3+
- Ilmainen
- Päätelty copyright tiedostosta
- Kopiointi ja jakaminen on sallittua, mutta muokkaus ei ole

Tämän ohjelman lisenssien kanssa ei ollut epäselvyyksiä.

## Grep komento (Regexp)
Grep komentoa varten testailin etsiä ```/usr/share/doc/gnome-terminal``` kansion copyright-tiedostosta hakusanoja license ja copyright käyttämällä komentoa: ```grep -E -i '^(license|copyright)' copyright```

Tuloksena oli tämä: </br>
![Kuva3](https://user-images.githubusercontent.com/122887740/214582626-a9b6d3f4-c94e-4534-a218-5a6a0469c664.png)</br>

## Pipe käyttö
Tehtävää varten hakeuduin kansioon ```/home/mattis``` ja siellä testailin aiemmin oppitunnilla tehtyyn testi.md tiedostoon seuraavanlaisia komentoja:
```cat testi.md``` ja heti perään ```cat testi.md | sort```, tulokset olivat seuraavanlaiset:</br>
![Kuva4](https://user-images.githubusercontent.com/122887740/214584316-6f682e54-b7d7-4fb4-a7b1-e93c212f8e31.png)</br>

## Regex Crossword
Kävin Regex Crossword tutorialin läpi ja alla kuva yhdestä oikeasta vastauksesta: </br>
![Kuva5](https://user-images.githubusercontent.com/122887740/214585260-cbf4e53e-9e69-4a09-a5a0-8ce7b2469024.png)</br>

## Lopetus
Tehtävän harjoituksiin meni n.1h ja lopettelin ne klo 16.01 aikoihin. Tehtävät olivat opettavaisia lisenssien ja Grepin käytön suhteen. Pipen käyttö on minulle entuudestaan tuttua PowerShellin kautta, joten sen logiikka oli jo mielessä ennen harjoitteita.


# Lähteet
Stack Exchange, How do I find out the license for each of my installed applications/packages?:
https://unix.stackexchange.com/questions/264055/how-do-i-find-out-the-license-for-each-of-my-installed-applications-packages

GNU Operating System, GNU General Public License, version 2:
https://www.gnu.org/licenses/old-licenses/gpl-2.0.html

Choose a license, BSD 2-Clause “Simplified” License:
https://choosealicense.com/licenses/bsd-2-clause/

IDManagement.gov, Public Domain License:
https://www.idmanagement.gov/license/

Wikipedia, SIL Open Font License:
https://en.wikipedia.org/wiki/SIL_Open_Font_License

GNU Operating System, GNU General Public License:
https://www.gnu.org/licenses/gpl-3.0.html

SPDX, GNU Free Documentation License v1.3:
https://spdx.org/licenses/GFDL-1.3.html

GNU Operating System, GNU LESSER GENERAL PUBLIC LICENSE:
https://www.gnu.org/licenses/lgpl-3.0.html

Vivek Gite, Regular expressions in grep ( regex ) with examples:
https://www.cyberciti.biz/faq/grep-regular-expressions/

Regex Crossword: https://regexcrossword.com/
