Devtestask

This project is deployed from the repository:

https://git.roky.rocks/roky-team/context-frontend/-/tree/master

Prerequisites
Node.js
npm
Installation
Clone the repository
Install dependencies

npm install
Build the project
bash

Copy code

npm run build
Start the server
bash

Copy code

npm start
Testing
Run tests

bash

Copy code

npm test
Deployment
The project is deployed on server:

95.142.45.204

in directory:

/opt/Devtest

It uses PM2 process manager to run the Node.js process in the background.

Configuration
Server configuration is located in:

/opt/Devtest/config

App configuration is located in:

/opt/Devtest/src/config.js