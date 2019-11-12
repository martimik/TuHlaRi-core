Tämä on esimerkki testitapauksesta. Testien suunnittelu kannattaa tehdä tarkoitukseen paremmin soveltuvalla testaushallintatyövälineellä esim. [Testlink](http://testlink.org)



### Testitapaus ID  : TCID05

  * Testitapauksen suunnittelija: Mikko Martikainen
  * Luontipvm : 12.11.2019

### Päivityshistoria

* versio 0.1 - 12.11.2019 - Mikko - testitapaus luotu

### Testitapauksen kuvaus

Pyrimme testaamaan uuden tuotteen tietojen päivittämistä järjestelmään.

### Lähde testille

* [Use case 04 - Tuotteen muokkaus](https://gitlab.labranet.jamk.fi/digiateam/core/blob/master/dokumentit/02-vaatimusmaarittely/UseCase/use-case-04-tuotteen-muokkaus.md)
* [Ominaisuus 06 - Tuotteen muokkaaminen](https://gitlab.labranet.jamk.fi/digiateam/core/blob/master/dokumentit/02-vaatimusmaarittely/Ominaisuudet/ominaisuus-06-tuotteen-muokkaaminen.md)

Käyttäjän tulee pystyä päivittämään tuotetietoja.

### Alkutilanne (Pre-state): 

* Käyttäjän pitää olla kirjautuneena sisään.
* Käyttäjällä pitää olla oikeus tuotteen näkemiseen sekä tuotetietojen muokkaamiseen.

### Testiaskeleet (Test Steps)

Askel ja odotettu tulos

 1. Käyttäjä kirjautuu sisään voimassaolevilla tunnuksilla. 
 2. Käyttäjä etsii haluamansa tuotteen ja painaa nappia "muokkaa tuotteen tietoja".
 3. Käyttäjä syöttää tuotteelle päivitettävät tiedot.
 4. Käyttäjä painaa hyväksy nappia.
 5. Tuotteen uudet tiedot päivittyvät tietokantaan.
 
### Huomioitava testin aikana

* huomio 1

### PASS/FAIL Kriteerit

* PASS: Tuotteen uudet tiedot päivittyvät tietokantaan.
* FAIL: Tuotteen tiedot eivät päivity tietokantaan.




