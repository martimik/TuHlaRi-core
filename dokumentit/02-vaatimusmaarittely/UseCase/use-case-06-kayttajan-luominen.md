# Use Case 6 - Käyttäjän luominen

## Use Case 

```plantuml

:Pääkäyttäjä: --> (Käyttäjän luominen) : Luo käyttäjän

```

* Laatija: Reko Meriö   
* Päiväys: 11.11.2019
* Prosessiosa-alue: ?
	
**Käyttäjäroolit**	

1. Pääkäyttäjä

**Esitiedot/ehdot**	

* Vain pääkäyttäjä voi luoda uusia käyttäjiä

**Käyttötapauksen kuvaus**

 1. Pääkäyttäjä menee hallintapaneeliin
 2. Klikkaa "Luo uusi käyttäjä" nappia
 3. Antaa käyttäjän nimen ja sähköpostin
 4. Luo uuden käyttäjän
 5. Käyttäjän sähköpostiin lähetetään 

**Poikkeukset**
 
* Uuden käyttäjän sähköpostiin ei lähde ilmoitusta luoduista tunnuksista
* Tunnusten luonti epäonnistuu
	
**Lopputulos**	

* Uusi käyttäjätunnus luodaan ja käyttäjää on infottu tunnuksista sähköpostilla

**Käyttötiheys** 

* Joitain kertoja kuukaudessa

**Muuta**	

* 

**Lähteet**

Tämä wiki-dokumentin runko pohjautuu [Julkisenhallinnon suosituksiin](http://www.jhs-suositukset.fi/web/guest/jhs/recommendations/173)

Kiitokset alkuperäisen tekijöille!
