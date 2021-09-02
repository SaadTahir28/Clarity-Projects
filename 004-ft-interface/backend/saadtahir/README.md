## Overview

This project is a web application that interacts with the Fungible Token created in Task#3. The front end contains plain html buttons to interact with the back end. The backend is built on express js server. Routes are defined and user can press buttons to call backend functions.

1. Say Hello --> Prints Hello World
2. Reveal Author Name --> Prints Author Name
3. Reveal Private Key --> Reveals private key of Hiro Wallet
4. Reveal Public Key --> Reveals public key generated from private key
5. Send Stx --> Transfer 12345 stx to a valid address e.g not ST5HYHBZ6CH0DHENSVCRTGKJ0CGTDFN09DRT38YK
6. Get Random Number --> Returns a random number by calling app contract's get-random-number read-only function
7. Goal Score --> Sends Fungible Token to valid address by calling app contract's goal-score public function. If the generated number is greater than 200, the player gets tokens in its wallet

## How to run it

run **node app.js** to start the server http://localhost:3000 and open **index.html** to run all the routes.

## index.html

View to interact with app.js

## app.js

Uses express js server and calls stack transactions based on routes

## myroutes.js

Definition for all valid routes

1. http://localhost:3000/
2. http://localhost:3000/user
3. http://localhost:3000/privateKey
4. http://localhost:3000/publicKey
5. http://localhost:3000/stx/send
6. http://localhost:3000/readonly/get-random-number
7. http://localhost:3000/public/goal-score

## constants.js

Contains all constants that are being used in the app
