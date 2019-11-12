Tämä on esimerkki testitapauksesta. Testien suunnittelu kannattaa tehdä tarkoitukseen paremmin soveltuvalla testaushallintatyövälineellä esim. [Testlink](http://testlink.org)



### Testitapaus ID  : TCID07

  * Testitapauksen suunnittelija: Mikko Martikainen
  * Luontipvm : 12.11.2019

### Päivityshistoria

* versio 0.1 - 12.11.2019 - Mikko - testitapaus luotu

### Testitapauksen kuvaus

Pyrimme testaamaan uuden käyttäjän luomista palveluun.

### Lähde testille

* [Use case 06 - Käyttäjän luominen](https://gitlab.labranet.jamk.fi/digiateam/core/blob/master/dokumentit/02-vaatimusmaarittely/UseCase/use-case-06-kayttajan-luominen.md)
* [Ominaisuus 07 - Käyttäjän luominen](https://gitlab.labranet.jamk.fi/digiateam/core/blob/master/dokumentit/02-vaatimusmaarittely/Ominaisuudet/ominaisuus-07-kayttajan-luominen.md)

Pääkäyttäjän tulee pystyä luomaan tunnukset uusille käyttäjille.

### Alkutilanne (Pre-state): 

* Käyttäjän pitää olla kirjautuneena sisään pääkäyttäjän tunnuksilla.

### Testiaskeleet (Test Steps)

Askel ja odotettu tulos

 1. Käyttäjä kirjautuu sisään pääkäyttäjän tunnuksilla. 
 2. Käyttäjä siityy sivulle "luo tunnukset".
 3. Käyttäjä syöttää uuden käyttäjän tiedot.
 4. Käyttäjä painaa "luo tunnukset"-nappia.
 5. Uusi käyttäjä tallentuu tietokantaan.
 6. Uusi käyttäjä kirjautuu palveluun pääkäyttäjän luomilla tunnuksilla.

### Huomioitava testin aikana

* huomio 1

### PASS/FAIL Kriteerit

* PASS: Uuden käyttäjän tiedot päivittyvät tietokantaan ja niillä pystyy kirjautumaan palveluun.
* FAIL: Uuden käyttäjän tiedot eivät tallennu tietokantaan.




