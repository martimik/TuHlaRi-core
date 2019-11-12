Tämä on esimerkki testitapauksesta. Testien suunnittelu kannattaa tehdä tarkoitukseen paremmin soveltuvalla testaushallintatyövälineellä esim. [Testlink](http://testlink.org)



### Testitapaus ID  : TCID1234

  * Testitapauksen suunnittelija: Markus Nylund
  * Luontipvm : 12.11.2019

### Päivityshistoria

* versio 0.1 - 12.11.2019 - Make - testitapaus luotu

### Testitapauksen kuvaus

Pyrimme testaamaan uuden tuotteen luomista järjestelmään

### Lähde testille

* [Use case 01 - Tuotteen luonti](https://gitlab.labranet.jamk.fi/digiateam/core/blob/master/dokumentit/02-vaatimusmaarittely/UseCase/use-case-01-tuotteen-luonti.md)
* [Ominaisuus 02 - Tuotteen luonti](https://gitlab.labranet.jamk.fi/digiateam/core/blob/master/dokumentit/02-vaatimusmaarittely/Ominaisuudet/ominaisuus-02-tuotteen-luonti.md)

* Käyttäjällä pitää olla oikeudet luoda tuotteita

### Alkutilanne (Pre-state): 

* Käyttäjän pitää olla kirjautuneena sisään

### Testiaskeleet (Test Steps)


Askel ja odotettu tulos

 1. Käyttäjä kirjautuu sisään oikeilla tunnuksilla 
 2. Käyttäjä painaa nappia "Luo uusi tuote"
 3. Käyttäjä syöttää tuotteelle tarpeelliset tiedot
 4. Käyttäjä painaa hyväksy nappia
 5. Uusi tuote tallentuu tietokantaa
 
### Huomioitava testin aikana

* huomio 1

### PASS/FAIL Kriteerit

* PASS: Uusi tuote tallentuu tietokantaan annetuilla tiedoilla
* FAIL: Uusi tuote ei tallenntu tietokantaan annetuilla tiedoilla




