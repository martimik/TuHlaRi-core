# Arkkitehtuuri ja tekniset ratkaisut

* Versio: 1.0
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

### Kirjastot
---------------------
### NodeJs

* Express

### React


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

![](http://plantuml.labranet.jamk.fi/png/U9nrairl4p4GnS_nN-4ZNoi11xXKbP8KAYI24843GYXolDFjgBPdcR4R0k9_hxsRZzsGtbQ_zzRpvjboXw4rRBncIg6sn05Oltwfv208_4eGBEY_QZ9bfisS7B6-Pe3m7PoZJUOs4i-8Q-17LMFlccv8xrYsZA7fV3l7UmgnrsOkcmTqYNz0ltex89-C1pqrBVnM_zGWh7L6f2Gz7RU06fCV3HtctKKTRVWHFPnPRNqIheiofyG8h2Q7kBd3oJH6ndMAS5pYJScxeD3GrKm_gohTCjN9HXd19C2YLB_DNhYuq4yMB_GItJtmKtrvkJViZ-WSduUEt8H-ZY5gh5LLvM-9fG0TSkOHa5lYU0LYHzJboMTWGpqmp6RxeyS_TGHx6t933OASqotvbWA4U5Q5S8zCmMVzItvmoE0VizeaaNmkkzFATWvlm6wjWsKqCSbHM2V1029VjoqSQNu4Df_KWpMHqoZpqYJU8DGZ_A46KswiBxgxbgxbRwSjZsh-l-S30M_GxL3vennvdTzfgzHgfTy5ozisGgrNg-oeTZ-rUVWcFy6Iv07kdZcV)

## Arkkitehtuuri

```plantuml

skinparam databaseBackgroundColor SpringGreen

skinparam interface {
  backgroundColor MediumPurple
  borderColor Purple
}

skinparam component {
	backgroundColor Lime
	borderColor Green
	ArrowColor DarkViolet
}

skinparam frame {
	backgroundColor GreenYellow
}

skinparam entity { 
    backgroundColor MediumSpringGreen
    borderColor GreenYellow
}

skinparam node {
	borderColor Green
	backgroundColor MediumSpringGreen
    backgroundColor<<API>> SpringGreen
}

interface dbAccess as "Database access"
interface apiAccess as "HTTPS"
  
node API <<API>> as "API (NodeJS)"

node product
node user
node login
node logout

entity  get as getU
entity  create as createU
entity  delete as deleteU
entity  edit as editU

entity  get as getP
entity  create as createP
entity  delete as deleteP
entity  edit as editP

API -- product
API -- user
API -- login
API -- logout

user -- getU
user -- createU
user -- deleteU
user -- editU

product -- getP
product -- createP
product -- deleteP
product -- editP


node "App (React)" {
   [Axios]
}
  

database "MongoDB" {
    frame "Users" {
        
    }
    frame "Products" {
        
    }
    frame "Technologies" {
        
    }
    frame "Components" {
        
    }
    frame "EnvironmentRequirements" {
        
    }
}
  
API <-left- dbAccess
MongoDB <--up- dbAccess

API <-up- apiAccess  
Axios <-down- apiAccess


  
```