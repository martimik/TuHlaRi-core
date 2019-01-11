# Suunnitteludokumentaatio


# 1.JOHDANTO
Luku antaa yleiskuvan suunnittelusta.
### 1.1		Tarkoitus ja kattavuus
Esitetään dokumentin tarkoitus, miksi se on tehty ja mihin tarkoituk-seen ja kenelle se on tarkoitettu (oman firman toteutusporukka vai ali-hankkija vai kuka).
Luetellaan, mitä asioita dokumentissa kuvataan; varsinkin jos lukija ei ole tottunut lukemaan suunnitteludokumentteja.
Määritetään suunnittelun kattavuus suhteessa määrittelyyn. Mikäli suunnittelu ei kata koko määrittelyä tulee se mainita tässä (eli mitä muita suunnitteluvaiheen dokumentteja on olemassa, esim. jos käyttö-liittymän tai tietokannan suunnittelu on irrotettu omiksi dokumenteik-seen).
### 1.2		Tuote ja ympäristö
Mainitaan tuotteen nimi, tarkoitus ja tavoitteet. Tuotteen toimintaym-päristö yleisesti: esimerkiksi PC, Windows98 ja lähiverkko.
### 1.3		Määritelmät, merkintätavat ja lyhenteet 
Selitetään aakkosjärjestyksessä sanat ja käsitteet, jotka eivät ole lukijal-le tuttuja, tai joiden voidaan ajatella tuottavan sekaannuksia erikoisella käytöllään tai jotka eivät yleisesti ole tiedossa. Nämä kannattaa esittää aakkosjärjestyksessä. Esim. ASCII-merkistöstä ilmoitetaan, onko se 7-bittinen (esim. ISO 10646) tai 8-bittinen (esim. ISO 8859-1).
### 1.4		Viitteet
Luetellaan viittaukset muihin lähteisiin (dokumentit, standardit, käsi-kirjat, tyyliohjeet, jne.) viitteen mukaan aakkosjärjestyksessä. Viitteistä ilmoitetaan nimi, versio, päiväys ja mistä ne ovat löydettävis-sä. Viitteiksi voidaan laittaa esimerkiksi:

  * dokumentit, joihin on viitattu (esim. määrittely)
  * dokumentit, jotka liittyvät systeemiin tai sen rakentamiseen
  * lisätiedot
  * (koodaus)tyyliohjeet. 
  * Mikäli suunnittelu ei kata koko määrittelyä, se mainitaan tässä. Samalla selvitetään, mitä muita suunnitteluvaiheen dokumentteja on olemassa. 
  * Esimerkiksi tietokannan tai käyttöliittymän suunnittelu on voitu irrot-taa omaksi dokumentikseen).

### 1.5		Yleiskatsaus dokumenttiin 

Kohdassa kuvataan dokumentin rakenne, sisältö ja organisointi; mitä missäkin luvussa käsitellään. Tämä on tärkeää varsinkin jos lukija ei ole tottunut lukemaan suunnitteludokumentteja.
Mikäli ensimmäinen luku on kokonaisuudessaan samalla sivulla kuin tämä kohta (1.5 yleiskatsaus) tai se on kovin lyhyt, ei sitä tarvitse tässä kohdassa mainita, vaan voidaan aloittaa luvun 2 asioista.
Kunkin luvun sisältöä kuvataan enemmän kuin mitä pelkkä sisällysluet-telon selaaminen kertoo.
Myös mahdolliset liitteet kuvaillaan tässä, esim. liitteet 1-4 sisältävät järjestelmän pääosien luokkakaaviot.

## 2.		JÄRJESTELMÄN YLEISKUVAUS
Luvussa esitetään toteutettavan järjestelmän yleiskuvaus, johdatus asi-akkaan ympäristöön ja sovellusalueeseen.

### 2.1		Sovellusalueen kuvaus
Kuvataan ympäristö, johon tuote tai järjestelmä liittyy. Esimerkiksi TUT:n opintotoimiston salivarausjärjestelmä.

### 2.2		Järjestelmän liittyminen ympäristöönsä

Määritetään, mitä järjestelmä tässä ympäristössä tekee, ja käyttääkö kuvattu järjestelmä muita ohjelmia tai järjestelmiä, eli onko se jonkin suuremman järjestelmän osa.

### 2.3		Laitteistoympäristö

Kuvataan laitteistoympäristö, jossa järjestelmä toimii. Esimerkiksi mitä oheislaitteita tarvitaan, mitä keskusyksiköltä odotetaan, mitä laitteiden ominaisuuksia ohjelma hyödyntää, mitkä laitteiston ominaisuudet ra-joittavat teknisiä ratkaisuja ja millaiset ovat liittymät muihin tietoko-neisiin.

### 2.4		Ohjelmistoympäristö

Esitetään järjestelmän ohjelmistoympäristö tarkkoine versioineen: käyt-töjärjestelmä, kääntäjä, muut apuvälineet, tietokantaohjelmisto, tieto-liikenneohjelmisto, www-selain, liittymät muihin ohjelmistoihin ja so-velluksiin sekä muut laitteistossa yhtä aikaa ajettavat ohjelmat. Tarvit-taessa voidaan selittää myös kehitys- ja testausympäristö. 

### 2.5		Toteutuksen keskeiset reunaehdot

Mainitaan tärkeät reunaehdot. Ne ovat usein asiakkaalta vaatimuksia.  Niitä voivat olla esimerkiksi toteutuslaitteisto, ohjelmisto, lait tai ase-tukset, vasteajat, kriittisyys, oikeellisuus, turvallisuus ja ohjelmointikie-li.
Tässä voidaan mainita myös ohje dokumentin sekä koodin komment-tien, muuttujien ja funktioiden yms. kielisyydestä.

### 2.6		Sopimukset ja standardit

Jos käytetään standardien ja/tai eri sopimusten mukaisia suunnittelu-menetelmiä, kuvaustapoja, dokumentointimalleja tms., niin ne maini-taan. Kuvataan myös mahdollisesti valmisosien käyttö ja niiden ni-meämissäännöt (tarvittaessa viittaus liitteeseen tai omaan dokument-tiinsa).
Myös erilaiset direktiivit, viranomaismääräykset ja ohjeistot mainitaan, mikäli ne vaikuttavat suunnitteluun. Tässä ne voi mainita nimeltä ja kohdassa 1.5 esitetään koko lähde tarkasti.
Otetaan kantaa myös projektin aineiston luottamuksellisuuteen mikäli siitä on aiheellista mainita. Luottamuksellisuuteen liittyviä asioita ovat esimerkiksi: jakelu, säilytys, vanhojen versioiden hävittäminen jne.

## 3.		ARKKITEHTUURIN KUVAUS

Tämä on suunnitteludokumentin tärkein kohta. Luku sisältää asiat, jot-ka kaikkien järjestelmän toteutusta tekevien täytyy tietää ja ymmärtää. Luvussa kuvataan (perusteluineen) mm. suunnittelu¬periaatteet, tekno-logiavalinnat ja ohjelmiston arkkitehtuuri yleisesti.  Jaottelua alilukui-hin ei välttämättä kannata tehdä tässä esitetyllä tavalla, vaan kannattaa miettiä, mikä on kulloisessakin tapauksessa järkevin esitysjärjestys lu-vun asioille. Esimerkiksi kohdat 3.1 ja 3.2 kannattaa joskus yhdistää.
### 3.1		Suunnitteluperiaatteet
Tässä kohdassa esitetään kehitettävän järjestelmän toteutuksen  ”pe-rusfilosofia”. Filosofia määrittelee mahdollisimman suppean ja yksin-kertaisen joukon peruskäsitteitä ja sääntöjä, joiden mukaan suunnittelu-päätöksiä nyt ja tulevaisuudessa tehdään. Peruskäsitteet ja säännöt voivat liittyä kohdan 3.2 arkkitehtuurikuvauksen joihinkin keskeisiin moduuleihin niin kiinteästi, että niiden kuvaus kannattaa siirtää tähän (tai jopa yhdistää kohdat 3.1 ja 3.2). Myös tehdyt teknologiavalinnat voivat olla osa ”sääntöjä”. Filosofian voi ajatella sisältävän järjestelmän toteutuksesta sellaiset asiat, jotka säilyvät (todennäköisesti) muuttu-mattomina koko elinkaaren ajan. Filosofia helpottaa toteuttajien keski-näistä kommunikointia ja yhdenmukaistaa suunnitteluratkaisuja järjes-telmän eri osissa. Esimerkkejä: 
  * Ohjausjärjestelmä toteutetaan mikrokontrollerissa ilman käyttö-järjestelmätukea.
  * Järjestelmä jakaantuu osiin seuraavasti: laitteisto¬abstraktio-kerros, käyttöjärjestelmäkerros ja sovellusmoduulikerros.
  * Laitteistoabstraktiokerroksen tarkoituksena on piilottaa käytet-tävän piirikortin ominaisuudet, jotta toteutusalusta on myö-hemmin tarvittaessa vaihdettavissa.
  * Käyttöjärjestelmä toteuttaa sovellusmoduulikerroksen proses-sien skeduloinnin ja keskeytyskäsittelyn ohjauksen sovellusmo-duulikerrokselle.
  * Sovellusmoduulikerroksen moduulit ovat joko passiivisia (kirjas-toja) tai aktiivisia (prosesseja). Molempien tyyppien koodirun-goista on esimerkki liitteessä x.
  * Kutakin ulkoista keskeytyslähdettä kohti määritellään ko. kes-keytyksen käsittelevä aktiivinen sovellusmoduuli.
Esimerkiksi luokka- ja tapahtumasekvenssikaavioita voi käyttää ku-vauksen selkeyttämiseksi.

### 3.2	 	Ohjelmistoarkkitehtuuri, moduulit ja prosessit

Tässä kohdassa esitetään yksityiskohtaisesti ohjelmiston jako osajärjes-telmiin, ohjelmiin, prosesseihin, moduuleihin, pakkauksiin ja/tai luok-kiin. Lisäksi kuvataan moduulinen välistä kommunikointia esimerkiksi tapahtumasekvenssikaavioiden avulla.
Moduuleista erotellaan "valmisosat", eli muualta sellaisenaan tai muo-katen napatut osat. Nämä seikat voi kuvata esim. moduulikaaviossa erilaisilla korostuskeinoilla.  
Tässä voidaan myös esittää nimeämiskäytäntöjä, viittauksia tyylioppai-siin yms. kaikkien moduulien toteutukseen liittyviä asioita.
### 3.3		Tietokanta-arkkitehtuuri
Tässä kohdassa kuvataan tiedostot ja tietokannat, mm. jako tiedostoi-hin ja/tai tietokantoihin, tiedostojen ja tietokantojen väliset liittymät, tiedostojen ja tietokantojen organisointi, käytettävät tietokantaohjel-mistot (jos on), suojaukset, toipuminen, varmistukset, huolto, ylläpito. 
Tiedostoista ja tietokannoista esitetään rakenne (esim. taulut eli relaa-tiokuvaukset, mikäli toteutus tehdään relaatiotietokannalla). Suunnitte-ludokumentissa määrittelydokumentin tietosisältökuvaukset muunne-taan fyysisen tietokannan kuvauksiksi. Esimerkiksi relaatio¬tieto¬kantaa käytettäessä määrittelydokumentin tietosisältökuvauksessa mahdolli-sesti olevat periytymissuhteet ja monta-moneen –yhteydet puretaan. Lisäksi määritellään navigointia varten tarvittavat indeksit. Kuvauksen perusteella pitäisi pystyä kirjoittamaan tietokantaa luotaessa tarvittavat SQL-kielen create table- ja create index -lauseet. 
Tietokantaratkaisusta ja tiedostoista kuvataan:
  * ratkaisun yleiskuva, tietokannat, tiedostot ja niiden väliset liittymät
  * tietokantaa käyttävät muut ohjelmistot tai järjestelmät
  * tietokannan tukiohjelmisto (esim. varmistukset, toipuminen, testaus)
  * tietokannoista ja tiedostoista
  * tietokannan rakenne (luokkakaavio selityksineen)
  * tiedoston tietueiden kenttien ja tietokannan taulujen sarakkeiden kuvaukset:
  * kentän nimi tai tunniste
  * kentän merkitys
  * kentän pituus ja muoto
  * sallitut arvot tyyppi
  * käsittely- tai laskentasäännöt
  * suhteet muihin tietoihin
  * päivityskriteerit ja -tavat
  * tilavaatimukset
  * ylläpitonäkökohdat
  * varmistusnäkökohdat
  * suojausnäkökohdat.
	
### 3.4	Virhe- ja poikkeusmenettelyt

Virhe- ja poikkeusmenettelyt yleisellä (arkkitehtuuri) tasolla. Luvussa 4 kuvataan tarkemmin moduulitasolla. 
Virheilmoitusten tekstit tulee kiinnittää viimeistään suunnittelussa (oli-si parempi miettiä ne jo määrittelyvaiheessa). Virheenkäsittelystä ote-taan huomioon seuraavanlaisia asioita:
  * yleiset virhekäsittelysäännöt
  * yleiset moduulit virheiden käsittelemiseksi
  * virheilmoitusten tunnistaminen
  * virheilmoitusten tallettaminen (muistiin, levylle)
  * virheilmoitusten ryhmittely (vakavuus, käyttäjän vai jär-jestelmän)
  * virheilmoitustekstit.
Toiminta epänormaaleissa tilanteissa kuuluu määrittelydokumenttiin, mutta viimeistään suunnittelussa on asiaan otettava kantaa. Esimerkiksi miten järjestelmä käyttäytyy virtakatkoksissa: "nouseeko itse pystyyn" vai "jääkö jumiin".
. 
## 4.		MODUULI /LUOKKA/PROSESSI-KUVAUKSET

Tämän luvun lukurakenne suunnitellaan ohjelman arkkitehtuurin mukaiseksi: Jos yksitasoinen jaottelu riittää, käytetään tässä esitettyä tapaa (4.1 Moduuli X, 4.2 Moduuli Y…). Jos ohjelma jakaantuu esi-merkiksi pakkauksiin, joiden sisällä on useita luokkia, kannattaa kulle-kin pakkaukselle tehdä oma kohtansa, jonka alakohdissa kukin luokka kuvataan. Pakkauksen kaikille luokille yhteiset asiat kuvataan luvun alussa, ja jos pakkauksella on rajapinta, myös se kuvataan tässä. Laa-joissa hankkeissa kunkin pakkauksen tai osajärjestelmän sisäisestä ra-kenteesta kirjoitetaan erillinen suunnitteludokumentti.
Jokaisesta moduulista kuvataan sen tehtävä, liittymät muihin osiin, ra-japinta sekä toteutusnäkökohdat. Tekniset yksityiskohdat täytyy selit-tää niin tarkasti, että kuvauksen perusteella pystytään suorittamaan moduulin testaus mustalaatikkotestauksena.

### 4.1		Moduuli X (kustakin moduulista oma alakohtansa 4.i)

### 4.1.1		Yleiskuvaus 
Moduulin nimi:
Moduulin tyyppi: (luokka, funktio, prosessi, pakkaus, alijärjestelmä, kirjasto)
Yleiskuvaus: Lyhyt kuvaus moduulista – miksi se on olemassa, mitä se tekee.
Asiakkaat: mitkä/minkä tyyppiset osat järjestelmästä tarvitsevat tämän osan palveluita (yleiskäyttöisen komponentin tapauksessa tämä kohta puuttuu).
Riippuvuudet ja liittymät muihin moduuleihin: Kuvataan lyhyesti, mi-ten moduuli käyttää hyväkseen muita moduuleita ja palveluita ympä-ristössään (voi usein yhdistää yleiskuvaukseen).
### 4.1.2		Rajapinta yleisesti
Kuvataan yleisesti moduulin tarjoamat palvelut ja rajapintafunktioiden yhteiset ominaisuudet (esimerkiksi virhetilanteiden käsittely). Joissain tapauksissa kannattaa antaa esimerkkejä moduulin käytöstä kuvaamalla asiakkaan ja moduulin välinen kommunikointi esimerkiksi tapahtuma-sekvenssikaaviona. Tässä mainitaan myös rajapinnasta mahdollisesti ulos näkyvät vakiot yms. määrittelyt, mahdolliset kapasiteettirajoituk-set ja niiden muuttaminen, moduulin tallettamat tilatiedot jne.

### 4.1.3	 	Rajapintafunktiot

Tässä kuvataan erikseen omassa alakohdassaan jokainen rajapintafunk-tio:
  * Funktion nimi
  * Funktion parametrit ja paluuarvo
  * Toiminta: mitä funktio tekee
  * Esiehdot: kuvataan, mikä ohjelman tilan pitää olla ennen funk-tion kutsua.
  * Jälkiehdot: kuvataan, mikä ohjelman tila on funktion kutsun jäl-keen (mm. sivuvaikutukset).
  * Virhetilanteet: poikkeukset ja muut virhetilanteet, toiminta kun esiehdot eivät kutsuttaessa pidä paikkaansa

### 4.1.4	 	Moduulin toteutus

Tarvittaessa voidaan antaa ohjeita toteutusta varten, esimerkiksi:
  * Ajatuksia moduulin sisäisten tietorakenteiden toteutuksesta.
  * Ajatuksia käytettävistä algoritmeista. 
  * Tiedossa olevat mahdollisesti uudelleenkäytettävät komponen-tit.
  * Mikäli moduuli on monimutkainen, voidaan käyttää pseudokoodia, ak-tiviteettikaavioita yms. Tarvittaessa voidaan tehdä erillinen moduuli-suunnitteludokumentti.

### 4.1.5	 	Virhekäsittely

Kuvataan virheiden ja poikkeusten käsittely moduulitasolla.

## 5.		VALMISOSAT JA ERITYISET TEKNISET RATKAISUT

Mikäli on valmisosia eli ulkopuolisia komponentteja, niin sellaisista se-lostetaan:
  * mistä ne saadaan 
  * mihin ne sijoitetaan 
  * käyttö 
  * muuta olennaista (jotta joku toinen osaisi koota sovelluksen tai lisätä ne mukaan). 
Mikäli jotkin asiat poikkeavat projektin tavanomaisista työtavoista. "Alan tavanomaisista käytännöistä poikkeavat ratkaisut", joita alan työntekijä ei ehkä heti arvaisi. 
Esimerkiksi seuraavia asioita, mikäli tarpeellista:
  * suojaukset, turvallisuus
  * varmistukset
  * toipumiset
  * ylläpidettävyys
  * joustavuus
  * siirrettävyys tai kannettavuus.
Varsinkin jos on jokin erityinen tai poikkeava tapa tehdä jotakin. 
Myös toteutusvälineet voidaan mainita tässä, mikäli se on todellakin oleellista kertoa jo tässä (suunnittelu) vaiheessa (harvinaista eikä suosi-teltavaa, esimerkiksi B-kääntäjän versio 2.77 joka tukee D-kirjastoa 4.56). Projektisuunnitelmassahan on tarkat tiedot toteutusvälineistä. 
Esimerkiksi pystyykö ohjelma toipumaan automaattisesti sähkökatkois-ta tai käyttöjärjestelmän "kaatumisista"?

	
## 6.	HYLÄTYT RATKAISUVAIHTOEHDOT

Mietityt, mutta hylätyt, ratkaisuvaihtoehdot kannattaa kirjata peruste-luineen johonkin sopivaan lukuun tai kohtaan päivämäärineen. Siten seuraava dokumentin lukija näkee, että tuotakin asiaa on mietitty. Sa-moin jos itse lukee suunnitteludokumenttia puolen vuoden päästä, voi olla vaikea muistaa, mitä asioita on mietitty järjestelmää tehtäessä.

Projektin lopussa hylätyt ratkaisuvaihtoehdot kerätään projektisuunni-telman loppuun.

## 7.	JATKOKEHITYSAJATUKSIA

Kerätään matkan varrella mieleen tulleita hyödyllisiä ajatuksia, joita ei tämän projektin puitteissa kuitenkaan suunnitella tarkemmin tai toteu-teta; esimerkiksi ajan puutteen, rahan puutteen, resurssien puutteen tai taitojen ja osaamisen takia.
Jatkokehitysajatukset kannattaa esimerkiksi numeroida, jotta niihin viittaaminen olisi helpompaa myöhemmin. Päiväys ja ehdottajan ni-mi(kirjaimet) auttavat jälkitarkastelussa, varsinkin jos lähde on projek-tin ulkopuolinen, jos vuoden kuluttua projekti saa yllättäen rahoitusta jatkokehitystä varten.
Projektin lopussa tämä luku kerätään projektisuunnitelman loppuun. Jatkokehitysajatukset voi esittää myös omana liitteenään, joka voi tar-vittaessa kulkea muidenkin projektin dokumenttien liitteenä. 

## 8.	VIELÄ AVOIMET ASIAT

Luku on epävirallinen ja sitä ei pitäisi olla enää projektin lopussa. Tä-hän voidaan merkitä dokumentin elinkaaren aikana avoinna olevia eli ratkaisua vaativia asioita, jotta ne muistettaisiin selvittää ennen doku-mentin lopullista valmistumista.


# Lähde

Tämä dokumentin runko pohjautuu http://www.cs.tut.fi/ohj/dokumenttipohjat/pohjat/suunnittelu/hytt_drsuunnittelu.doc

Kiitokset alkuperäisen tekijöille!

