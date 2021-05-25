# bearer-auth

## Author: As-har Abuhelweh

* [Tests Report]()

* [Heroku Deployment]()

* [Pull Request]()

<hr>

### Setup

1. Clone the repo

2. npm init -y.

3. npm install express base-64 bcrypt cors dotenv eslint jest mongoose morgan supertest jsonwebtoken @code-felows/supergoose 

4. Create .env file with PORT=5000 ,SECRET,EXPIRESIN=900000.

5. Test --> `npm test`


<hr>

### Run the app

npm start

<hr>

### End points

* **/signup**: POST Method

  received 
  ```js{
    "user": {
        "_id": "60ad52266c65ff3c439d5448",
        "username": "ashar",
        "password": "$2b$10$R6.z/JsX.AcJVhQfl3M9quRi/A6hPH7vCaYuidH8LLrxdko3d9x.C",
        "__v": 0
    },
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6ImhhZGVlbCIsImlhdCI6MTYyMTk3MTQ5NH0.5kHaD5HxNbankXIhTVq6hsmODvuPVjdPBTOXI5yg6zo"
   }
   ```
    
    You can Sign-up by sending post request using postman.



* **/signin**: POST Method
  
  received 

   ```js
   {
    "user": {
        "_id": "60ad52266c65ff3c439d5448",
        "username": "hadeel",
        "password": "$2b$10$R6.z/JsX.AcJVhQfl3M9quRi/A6hPH7vCaYuidH8LLrxdko3d9x.C",
        "__v": 0
    },
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VybmFtZSI6ImhhZGVlbCIsImlhdCI6MTYyMTk3MTc3NX0.m7Mvut0WPoAhopDfNCRX9H-9T6WuYnFk30ayRqf7nzQ"
  }
  ```

   

    You can signin by sending post request using postman.

* **/users**: get Method
  ```js
  {
    "user": "ashar"
  }
  ```
  

    enter the token and sending get request using postman. 

* **/secret** :get Method
   ```js
   Welcome to the secret area!
   ```

    enter the token and sending get request postman.

<hr>

### UML


![uml](uml.png)