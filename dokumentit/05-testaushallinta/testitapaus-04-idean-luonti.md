### Idean luonti  : TCID1234

  * Testitapauksen suunnittelija: Elias Kautto
  * Luontipvm : 12.11.2019

### Päivityshistoria

* versio 0.1 - 12.11.2019 - Elias Kautto - testitapaus luotu

### Testitapauksen kuvaus

Testataan tuleeko käyttäjälle error-viesti, jos käyttäjä ei ole antanut tarvittavia tietoja uutta tuoteidaa/tuotetta luodessaan.

### Lähde testille

Eli minkä pohjalta testi on suunniteltu?

* [Tuotteen luonti - Feature](https://gitlab.labranet.jamk.fi/digiateam/core/blob/master/dokumentit/02-vaatimusmaarittely/Ominaisuudet/ominaisuus-02-tuotteen-luonti.md)
* [Tuotteen luonti - Use case](https://gitlab.labranet.jamk.fi/digiateam/core/blob/master/dokumentit/02-vaatimusmaarittely/UseCase/use-case-01-tuotteen-luonti.md)

### Alkutilanne (Pre-state): 

* Käyttäjän tulee olla kirjautuneena.
* Käyttäjällä tulee olla oikedet uuden tuotteen/tuote idan luontiin.

### Testiaskeleet (Test Steps)


Askel ja odotettu tulos

 1. Paina lisää uusi tuote
 2. Jätä lisäämättä nimi
 3. Paina lisää-nappia


### PASS/FAIL Kriteerit

* PASS: Error-viesti näkyy
* FAIL: Tuote lisääntyy tietokantaan, error-viestiä ei näy




