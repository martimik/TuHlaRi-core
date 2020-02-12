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
* Response: `[{email, userGroup, name, createdAt}]` or `{ error: "Nothing found" }` or `{ message: "Unauthorized", code: "UAE1" }`

Palauttaa listan käyttäjistä, jos sessio on olemassa, eli käyttäjä on kirjautunut.
Vain admin voi nähdä muut admin ryhmään kuuluvat käyttäjät.
