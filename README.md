# Faceable Middleware

#### Faceable middleware API's for client desktop app and Dashboard

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites
- [Node.JS](https://nodejs.org/en/) - Node.js is a JavaScript runtime built on Chrome's V8 JavaScript engine.

#### Node.JS installation for Windows

- Download and install the latest version of Node.JS from [here](https://nodejs.org/en/) 
- After installing, open command prompt and type ```node --version```
- You will see output like ```v10.15.3```
- Version might be different in your case.

#### Node.JS installation for Linux

- Open your terminal or press Ctrl + Alt + T and use the following commands to update and upgrade the package manager
```bash
$ sudo apt-get update
$ sudo apt-get upgrade
```
- Install Python software libraries using the following command
```bash
$ sudo apt-get install python-software-properties
```

- Add Node.js PPA to the system
```bash
$ curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash –
```
Note: Here, we are installing node.js version 10, if you want to install version 11, you can replace setup_10.x with setup_11.x.

- To Install Node.js and NPM to your Ubuntu machine, use the command given below
```bash
sudo apt-get install nodejs
```

- Once installed, verify it by checking the installed version using the following command
```bash
$ node –version
$ npm –version
```

### Installing

##### 1) Clone the repository.
##### 2) cd into root folder
##### 3) edit the ```config.env.env``` file

##### You will need an Azure Subscription (trial/paid) to create the following resources:
- Azure Storage account
- Azure Cosmos DB (SQL API)
- Azure Face API
- Azure Logic Apps
##### *All the services mentioned above are available in free trial. We will need the subscription keys to put into the env file.

##### 4) Create one container under your Azure storage account and name that container as ```events``` and put the blob URL of this container as the value of ```EVENTS_BLOB_URL``` inside ```config.env.env``` file

##### 5) Put other keys also in the repective places inside ```config.env.env``` file

##### 6) logic app ------------

##### 7) Create a database inside your Azure Comosdb and put the name of that DB inside ```config.env.env``` file as well.

##### 8) Create the following collections inside this DB.
- employees
- assetmanagement
- wfhrecords
- events
- otpauth

##### 9) Install all the dependencies. Open your CMD/terminal and type the command
```bash
$ npm install
```
##### 10) run the application
Run in dev mode
```bash
$ npm run dev
```
Run in production mode
```bash
$ npm run dev
```
