# Sequelize ORM POC

The code in this repo demonstrates use of [sequelize](https://sequelize.org/v5/) as an ORM using two tables with geography data sets (continents and countries).

This proof of concept uses a repository to get data from database and uses [express](https://expressjs.com/).

## Get Started

You will need to change directory into the "server" folder to install and run the application

To get started perform the following steps:

### 1) Install PostGre SQL

https://www.postgresql.org/download/

### 2) Create PostGre SQL database to use in this POC

After installing locally you should have database server and you need to enable credentials from Database.ts with access empty database named "orm_poc"

### 3) Install npm packages

You will need to change directory into the server folder to install and run the application

Install the required packages after changing directory into the "server" folder

```npm install```

### 4) Create database schema using sequelize migrations

run the following command - see more: https://sequelize.org/master/manual/migrations.html

```npx sequelize-cli db:migrate```

### 5) Populate database with data using sequelize data seeding

```npx sequelize db:seed:all --debug```

### 6) run the application

The application is configured to use nodemon to monitor for file changes and you can run command to start the application using it. You will see console information with url and port.

```npm run start```

### 7) exercise the application via postman

Download and install https://www.getpostman.com and then import the collection in the "postman" folder and run the requests to see api data and responses