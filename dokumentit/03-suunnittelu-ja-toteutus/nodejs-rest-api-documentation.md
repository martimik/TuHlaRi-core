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
* Parameters: `{ email, password }` 

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
* Parameters: `{ email, password, userGroup }` 

Luo uuden käyttäjän, jos samalla sähköpostilla ei vielä ole käyttäjää olemassa. Vain admin käyttäjäryhmään kuuluva voi luoda uuden käyttäjän.

### /editPassword
* Method: POST
* Response: `{ message: "New user created" }` or `{ message: "Email already in use.", code: "NUE2" }` or `{ message: "Unauthorized", code: "UAE1" }`
* Parameters: `{ password, oldPassword }` 

Salasana vaihdetaan, jos vanha salasana on oikein.

### /editUser
* Method: POST
* Response: `{ message: "User updated succesfully.", code: "UPS" }` or `{ message: "Couldn't update user", code: "UPE4" }` or `{ message: "Unauthorized, need admin privileges", code: "UAE2" }`
* Parameters: `{ name, reqEmail, email, userGroup }` 

Vain admin käyttäjäryhmään kuuluva voi muokata käyttäjän tietoja. reqEmail on muokattavan käyttäjän nykyinen sähköposti ja email on käyttäjän mahdollinen uusi sähköposti

### /deleteUser
* Method: POST
* Response: `{ message: "User deleted succesfully.", code: "UDS" }` or `{ message: "Couldn't delete user", code: "UDE1" }` or `{ message: "Unauthorized, need admin privileges", code: "UAE2" }`
* Parameters: `{ email }` 

Vain admin käyttäjäryhmään kuuluva voi poistaa käyttäjiä.

### /products
* Method: GET
* Response: `[{product}...]` or `{ message: "Nothing found", code: "PE1" }`
* Parameters: `{ myProducts, isParticipant, isClassified, lifecycleStatus, search }` 

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

### /addProduct
* Method: POST
* Response: `{ message: `Successfully created product <id>`, code: "APS" }` or `{ message: "Couldn't add product, code:"APE3" }`
* Parameters: `{ productName, shortDescription, longDescription, logo, technologies, components, environmentRequirements, customers, productOwner, salesPerson, lifecycleStatus, businessType, pricing, isClassified, isIdea, participants } }` 

Luo uuden tuotteen. Käyttäjän tulee olla kirjautunut sisään. Pakollisia tietoja ovat productName, shortDescription, lifecycleStatus

### /updateProduct
* Method: POST
* Response: `{ message: "Successfully updated product <id>", code "EPS"}` or `{ message: "Couldn't update product", code:"EPE3" }`
* Parameters: Kaikki samat kuin addProductissakin, sekä tuotteen id

Muokkaa olemassa olevaa tuotetta. Käyttäjän tulee olla kirjautunut sisään.

### /restoreProduct
* Method: POST
* Response: `{ message: "Successfully restored product <id>", code "RPS"}` or `{ message: "Couldn't restore product", code:"RPE1" }`
* Parameters: { _id }

Palauttaa poistetun tuotteen. Käyttäjän tulee olla kirjautunut sisään.

### /uploadImage
* Method: POST
* Response: `<image name>` or `{ error }`
* Parameters: { image }

Lataa kuvan palvelimelle kansioon /images ja palauttaa kuvan sijainnin.

### /technologies
* Method: GET
* Response: `[{ technology, id }, ...]` or `{ error }`
* Parameters: { query }

Palauttaa listan teknologioista. Queryyn voi antaa tekstin joka teknologian tulee sisältää.

### /components
* Method: GET
* Response: `[{ component, id }, ...]` or `{ error }`
* Parameters: { query }

Palauttaa listan komponenteista. Queryyn voi antaa tekstin joka komponentin tulee sisältää.

### /environmentRequirements
* Method: GET
* Response: `[{ requirement, id }, ...]` or `{ error }`
* Parameters: { query }

Palauttaa listan ympäristövaatimuksista. Queryyn voi antaa tekstin joka ympäristövaatimuksen tulee sisältää.