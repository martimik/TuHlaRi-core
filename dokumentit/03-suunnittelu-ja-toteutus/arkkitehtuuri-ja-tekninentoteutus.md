# Arkkitehtuuri ja tekniset ratkaisut

* Versio: 0.1
* Näkyvyys: Julkinen

## Johdatus

Tässä dokumentissa käsitellään projektin arkkitehtuuria sekä teknisiä ratkaisuja. Dokumentti päivittyy projektin edetessä.

## Yleiskuvaus

* Esittele lyhyesti tuote tai kohde
* Dokumentin tehtävä on avata esim. jatkokehittäjälle käsitys siitä miten tuote on toteutettu (Pelkkä lähdekoodi ei riitä)
* Millaisia välineitä/työkaluja ja ympäristöjä tarvitaan, jos aioitaa kehitää tuotetta eteenpäin

## Käytetyt teknologiat

Rajallisten resurssien vuoksi teknologioiksi on valittu sellaiset teknologiat, jotka ovat nopeita kehittää.

NodeJS ja React ovat molemmat ohjelmoitavissa korkean luokan JavaScript kielellä, joka on tiimille jo tuttua.

* Back-end: NodeJS - Helppokäyttöinen ja ominaisuuksiltaan riittävä
* Front-end: React - Monipuolinen ja hyväksi todettu
* Tietokanta: MongoDB - Helppo datan hallinta

## Tuotekehitysympäristöjen kuvaukset

Kuvaa ainakin seuraavat:

* Kehitysympäristö
* Testausympäristö
* Ajo/suoritusympäristö
* Demoympäristö

Eli miten nuo eri ympäristöt on toteutettu ko. projektissa

## Käytetyt työvälineet ja niiden versionumerot

* Visual Studio Code
* NodeJS

## Tärkeimmät tekniset ratkaisut joihin tuote nojaa

* React
* NodeJS
* MongoDB
* Muut jipot ja kikat
* Perustelut miksi! 
  
## Yleinen ohjelmsto arkkitehtuuri

* Back-end pyörii CSC:n Rahti palvelun virtuaalikoneella
* Runneri, joka rakentaa ja puskee uuden imagen, pyörii CSC:n cPouta palvelun virtuaalikoneella

## Palvelujen/n rajapinnat (Interfaces)

* [Esimerkki elävästä elämästä](https://virkailija.opintopolku.fi/koodisto-service/swagger/index.html)

## Suoritysympäristön (tuotanto) kuvaus

* Back-end pyörii CSC:n Rahti palvelun virtuaalikoneella
* Runneri, joka rakentaa ja puskee uuden imagen, pyörii CSC:n cPouta palvelun virtuaalikoneella
* Front-end mahdollisesti GitLab pages?

## Tietokantakuvaukset

![](http://plantuml.labranet.jamk.fi/png/U9nrKarl4p4GFSU_maSeh4Gvb4jLAMbfBmGX0WU4KEHufzjHRO-PiHi2uh_ZtSt7RaXlrdlFCs_UZ3nYY8QDrqmvr9Ou0EktRvJi2O6V6O85_KTDfioqlYP7hEyO87m3vsXTS9k8PyGryBEiiOzDrwHNB29ZQ3hTLd5B8VNSp1Nn05tWRz3dxmR8H-D1Jqs4N-gl6fYrpeYqJe_RpQ76x4TDXtwtLaSJVa0F9qPR7Pdhh5nJPWHMaxtTak5acXBZAYSu377H-frJQEXcfi-gIaUcEjia8p0Bi2ZLJxCZBY_rY_bhlK3t1FnINrtj1BiIdUBJK56IqAym98srgghobjG6e4FnF0BaWJZTWDWHwahd4s13FM2OpUPx3__G2Un3A0ar27AAj-GZ1GZf90lX2Pc2B_pdSd38u9-JsYo9V0cxuzhf7Dw3tLW7YsHIbWEnoe81HBvi8XpGSWIsLEg15P7hpmRl4UfsFNsgtGwwIByUHphAzFzGzmXuWsuBjJ_QadVbAADIowL-7onlOe9QBvT5KMq_nT9yNUwjTV8FzAKq3m00)


