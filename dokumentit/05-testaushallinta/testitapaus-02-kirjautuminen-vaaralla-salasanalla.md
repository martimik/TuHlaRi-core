### Testitapaus ID  : TCID2

  * Testitapauksen suunnittelija: Reko Meriö
  * Luontipvm : 12.11.2019

### Päivityshistoria

* versio 0.1 - 12.11.2019 - Reko Meriö - testitapaus luotu

### Testitapauksen kuvaus

Testataan, että käyttäjää ei kirjata sisään, jos hän käyttää väärää salasanaa 

### Lähde testille

* [Käyttötapaus - Use Case](https://gitlab.labranet.jamk.fi/digiateam/core/blob/master/dokumentit/02-vaatimusmaarittely/UseCase/use-case-05-kirjautuminen.md)
* [Ominaisuus - Feature](https://gitlab.labranet.jamk.fi/digiateam/core/blob/master/dokumentit/02-vaatimusmaarittely/Ominaisuudet/ominaisuus-01-kirjautuminen.md)

Minkä pohjalta testi on suunniteltu?

* Käyttäjän pitää pystyä kirjautumaan omilla tunnuksillaan

### Alkutilanne (Pre-state): 

* Käyttäjällä on toimivat tunnukset
* Käyttäjä ei ole kirjautunut sisään

### Testiaskeleet (Test Steps)

 1. Syötä toimiva sähköposti
 2. Syötä väärä salasana
 3. Klikkaa kirjaudu sisään 
 
### Huomioitava testin aikana

* 

### PASS/FAIL Kriteerit

* PASS: Käyttäjää ei kirjata sisään

* FAIL: Käyttäjän kirjataan sisään