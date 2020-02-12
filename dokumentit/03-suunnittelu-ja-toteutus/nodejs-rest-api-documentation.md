# NodeJS REST API

## Reitit

### /
* Method: GET  
* Response: `Ok`

### /session
* Method: GET
* Response: `{ name, email, userGroup }`  

Jos sessiota ei ole olemassa, propertyt ovat null

### /login
* Method: POST
* Response: `{ name, email, userGroup }` or `{ message: "Invalid credentials", code: "LIF1" }` 
* Parameters `{ email, password }` 

Palauttaa käyttäjän sähköpostin, salasanan ja käyttäjäryhmän, jos sähköposti ja salasana täsmäävät.

### /logout
* Method: POST
* Response: `{ name: null, email: null, userGroup: null }` or `{ error: "Session does not exist" }` 

Tuhoaa session eli kirjaa käyttäjän ulos, mikäli sessio on olemassa.

### /logout
* Method: POST
* Response: `{ name, email, userGroup }` or `{ error: "Session does not exist" }` 

Tuhoaa session eli kirjaa käyttäjän ulos, mikäli sessio on olemassa.

### /users
* Method: GET
* Response: `[{email, userGroup, name, createdAt}...]` or `{ error: "Nothing found" }` or `{ message: "Unauthorized", code: "UAE1" }`

Palauttaa listan käyttäjistä, jos sessio on olemassa, eli käyttäjä on kirjautunut.
Vain admin voi nähdä muut admin ryhmään kuuluvat käyttäjät.

### /newUser
* Method: POST
* Response: `{ message: "New user created" }` or `{ message: "Email already in use.", code: "NUE2" }` or `{ message: "Unauthorized", code: "UAE1" }`
* Parameters `{ email, password, userGroup }` 

Luo uuden käyttäjän, jos samalla sähköpostilla ei vielä ole käyttäjää olemassa. Vain admin käyttäjäryhmään kuuluva voi luoda uuden käyttäjän.

### /editPassword
* Method: POST
* Response: `{ message: "New user created" }` or `{ message: "Email already in use.", code: "NUE2" }` or `{ message: "Unauthorized", code: "UAE1" }`
* Parameters `{ password, oldPassword }` 

Salasana vaihdetaan, jos vanha salasana on oikein.

### /editUser
* Method: POST
* Response: `{ message: "User updated succesfully.", code: "UPS" }` or `{ message: "Couldn't update user", code: "UPE4" }` or `{ message: "Unauthorized, need admin privileges", code: "UAE2" }`
* Parameters `{ name, reqEmail, email, userGroup }` 

Vain admin käyttäjäryhmään kuuluva voi muokata käyttäjän tietoja. reqEmail on muokattavan käyttäjän nykyinen sähköposti ja email on käyttäjän mahdollinen uusi sähköposti

### /deleteUser
* Method: POST
* Response: `{ message: "User deleted succesfully.", code: "UDS" }` or `{ message: "Couldn't delete user", code: "UDE1" }` or `{ message: "Unauthorized, need admin privileges", code: "UAE2" }`
* Parameters `{ email }` 

Vain admin käyttäjäryhmään kuuluva voi poistaa käyttäjiä.

### /products
* Method: GET
* Response: `[{product}...]` or `{ message: "Nothing found", code: "PE1" }`
* Parameters `{ myProducts, isParticipant, isClassified, lifecycleStatus, search }` 

Palauttaa kaikki hakukriteereihin osuvat tuotteet. 
* myProducts: Palauttaa tuotteet, jotka käyttäjä on luonut
* isParticpant: Palauttaa tuotteet, joissa käyttäjä on osallisena
* isClassified: Palauttaa myös ns. salatut tuotteet, jotka käyttäjä on oiketettu näkemään.
* search: Palauttaa tuotteet joiden otsikosta tai lyhyestä- tai pitkästä kuvauksesta löytyy annettu merkkiyhdistelmä
* lifecycleStatus: Palauttaa tuotteet, jotka ovat samalla lifecycleStatuksella, tai jos lifecycleStatus on 0, palautetaan kaikki

### /product/:id
* Method: GET
* Response: `{ product }` or `{ message: "Not found" }`

Palauttaa tuotteen annetulla id:llä

### /product/:id
* Method: DELETE
* Response: `{ message: "Deleted :id" }` or `{ message: "Not found" }` or `{ message: "Unauthorized" }` 

Poistaa tuotteen annetulla id:llä, jos lähettäjä on sama kuin tuotteen luoja.

### /deletedProducts
* Method: GET
* Response: `[{product}...]` or `{ message: "Nothing found", code:"PE1" }`

Palauttaa listan kaikista ns. "poistetuista tuotteista".