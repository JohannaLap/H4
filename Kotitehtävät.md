## x) Lue/katso ja tiivistä.
- Hascatin perus periaatteet ja toiminnan läpikäyminen
- Perus periaatteet ja toiminta John the Ripperistä
- Näissä oli hyvät, selkeät ja toimivat ohjeet
- MSFVenomin käyttö ( Reverse Shell ja Bind Shell, payloadit)

## a) Asenna Hashcat ja testaa sen toiminta murtamalla esimerkkisalasana.
Ensiksi asensin hashcatin.

![hashcat asennus](https://github.com/JohannaLap/H4/blob/main/hashcat%20asennus.png)

Loin kansion.

![mkdir hashed](https://github.com/JohannaLap/H4/blob/main/mkdir%20hashed.png)

Latasin rockyoun.

![rockyou](https://github.com/JohannaLap/H4/blob/main/rockyou.png)

Purin tiedoston.

![purin tiedoston](https://github.com/JohannaLap/H4/blob/main/purin%20tiedoston.png)

Tarrkistin, että saan komennoilla näkymän tiedoston alkuosaan ja tuloksen tiedoston rivien määrästä.

![headrockyou](https://github.com/JohannaLap/H4/blob/main/headrockyou.png)

Ajoin komennon, jolla testattiin rockyou sanakirjan sanat.

![crack the hash](https://github.com/JohannaLap/H4/blob/main/crack%20the%20hash.png)

Tarkistin salasanan.

![salasana](https://github.com/JohannaLap/H4/blob/main/salasana.png)



## c) Asenna John the Ripper ja testaa sen toiminta murtamalla jonkin esimerkkitiedoston salasana.

Asensin tarvittat esiasennuspaketit 'sudo apt-get -y install micro bash-completion git build-essential libssl-dev zlib1g zlib1g-dev zlib-gst libbz2-1.0 libbz2-dev atool zip wget'
Kloonasin John the Ripperin. 

![kloonaus](https://github.com/JohannaLap/H4/blob/main/kloonaus.png)

Tarkistin ' ./configure ' komennolla ohjelman asennuksen valmistelun (riippuvuudet ja konfiguraatiotiedostot jnejne)

![configure](https://github.com/JohannaLap/H4/blob/main/configure.png)

Alla olevalla komennolla tarkoitus kääntää uudelleen ja poistaa vanhat kääännetyt tiedostot. Tässä kohtaa alkoi tulemaan jotakin ihmeellistä ilmoitusta (lilalla)..päätin kuitenkin jatkaa..

![clean && make](https://github.com/JohannaLap/H4/blob/main/clean%20%26%26%20make.png)

Varmistin, että näen tiedostot hakemistossa. 

![runls](https://github.com/JohannaLap/H4/blob/main/runls.png)

John the Ripper käynnistyi siis oikein!

![käynnistys](https://github.com/JohannaLap/H4/blob/main/k%C3%A4ynnistys.png)

Latasin esimerkki tieodston ja yritin avata sitä..siinä onnistumatta.

![ziplatausa jayritys avaus](https://github.com/JohannaLap/H4/blob/main/ziplatausa%20jayritys%20avaus.png)

Zipin kaksi vaiheinen murtamien tapauhtui seuraavast: 
1. Vaihe:
   - uuteen hash uuteen tiedostoon.

![uusitiedosto](https://github.com/JohannaLap/H4/blob/main/uusitiedosto.png)
  
2. Vaihe:
   - Suoritetaan hashia vastaan hyökkäys.

![hyökkäys](https://github.com/JohannaLap/H4/blob/main/hy%C3%B6kk%C3%A4ys.png)

![loppuvaiheet](https://github.com/JohannaLap/H4/blob/main/loppuvaiheetjohn.png)




## d) Fuffme

Asensin tarvittavat esivaatimussysteemit. 

![docker](https://github.com/JohannaLap/H4/blob/main/docker.png)

Kloonasin ffufme:n.

![kloonausffuf](https://github.com/JohannaLap/H4/blob/main/kloonausffuf.png)

Loin ffufme nimisen docker imagen (?)

![buildffufme](https://github.com/JohannaLap/H4/blob/main/buildffufme.png)

Yrittäessä ajaa targettia sain virhe ilmoituksen, että portti on jo käytössä. Tarkistin tilanteen ja vapautin portin. Ajoin dockerin kontin uudelleen, tällöin tämä onnistui.

![dockerrun](https://github.com/JohannaLap/H4/blob/main/dockerrun.png)

Tarkistin curl avulla, että kontti on käynnistynyt oikein. 

![curllocalhost](https://github.com/JohannaLap/H4/blob/main/curllocalhost.png)

Varmistin näkymän selaimella.

![localhostsivu](https://github.com/JohannaLap/H4/blob/main/localhostsivu.png)

Asensin sanalistat.

![sanalistat](https://github.com/JohannaLap/H4/blob/main/sanalistat.png)

Basicdiscovery 

![basicdiscovery]()

Content discovery - recursion

![content discovery](https://github.com/JohannaLap/H4/blob/main/content%20discovery.png)

Content discovery - file extensions

![file extensions ](https://github.com/JohannaLap/H4/blob/main/file%20extensions%20.png)

Content discovery - No 404 status

![nostatus](https://github.com/JohannaLap/H4/blob/main/nostatus.png)

![nostatus2](https://github.com/JohannaLap/H4/blob/main/nostatus2.png)

Content discovery - param mining

![mining](https://github.com/JohannaLap/H4/blob/main/mining.png)

Content discovery - rate limited

![ratelimited](https://github.com/JohannaLap/H4/blob/main/ratelimited.png)

Tämä ei ilmeisesti kuitenkaan toiminut toivotusti..

![ratelimited2](https://github.com/JohannaLap/H4/blob/main/ratelimited2.png)

VIrtualhost 

![localhost](https://github.com/JohannaLap/H4/blob/main/localhost%20.png)

![localhost2](https://github.com/JohannaLap/H4/blob/main/localhost2.png)





## e) Tiedosto

Salasanan ja tiedoston luonti. 
zip
![salasana.txt](https://github.com/JohannaLap/H4/blob/main/salasana.txt.png)

Sitten tein ZIPin, joka on salattu, jossa äsken luotu tiedosto on. Salasanaksi valitsin 1234

![zipinluonti](https://github.com/JohannaLap/H4/blob/main/zipinluonti.png)

Testasin, ettei tiedostoa saa suoriltaan auki (tarkoituksella väärällä salasanalla)

![testi](https://github.com/JohannaLap/H4/blob/main/testi.png)

Tarkistin että zip tiedosto näkyy. 

![ziptarkistus](https://github.com/JohannaLap/H4/blob/main/ziptarkistus.png)

Yrittäessä ajaa zip tiedostoa johnilla, sain virhe ilmoituksen..

![error](https://github.com/JohannaLap/H4/blob/main/error.png)

Tästä jouduin jatkamaan 22.11.



## f) Tiiviste. 

## g) Tee msfvenom-työkalulla haittaohjelma, joka soittaa kotiin (reverse shell). Ota yhteys vastaan metasploitin multi/handler -työkalulla.


## Lähteet:
Karvinen 2022: Cracking Passwords with Hashcat : https://terokarvinen.com/2022/cracking-passwords-with-hashcat/
Karvinen 2023: Crack File Password With John : https://terokarvinen.com/2023/crack-file-password-with-john/
Polop et al 2024: HackTricks: MSFVenom - CheatSheet : https://book.hacktricks.xyz/generic-methodologies-and-resources/reverse-shells/msfvenom

