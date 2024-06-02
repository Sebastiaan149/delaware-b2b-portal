# 2023-backend-gent16

## Contents

- [Introduction](#introduction)
- [Requirements](#requirements)
- [Start the API](#start-the-api)
- [Testing](#testing)

## Introduction

This repository contains the backend of the web application for the SDP2 assignment 2023.
The application was made by Yani Degrande, Thomas Odvart, Sebastiaan Delodder, Jente Coppejans and Warre Vandenhoucke.

## Requirements

We expect the following software to be installed:

- [NodeJS](https://nodejs.org)
- [Yarn](https://yarnpkg.com)
- [MySQL Community Server](https://dev.mysql.com/downloads/mysql/)

## Start the API

To start the API, a .env file is needed. This file must contain the following variables:

- NODE_ENV=development
- JWT_SECRET="yourJWTsecret"
- DATABASE_URL="mysql://janedoe:mypassword@localhost:3306/mydb" [(Create database URL)](https://www.prisma.io/docs/reference/database-reference/connection-urls)

To start the API, run the following commands:

- yarn install
- yarn start

To set up the database, run the following commands:

- npx prisma db push
- npx prisma generate

## Testing

To test the application, a .env.test file is needed. This file must contain the following variables:

- NODE_ENV=test
- JWT_SECRET="yourJWTsecret"
- DATABASE_URL="mysql://janedoe:mypassword@localhost:3306/mydb" [(Create database URL)](https://www.prisma.io/docs/reference/database-reference/connection-urls)

To run the tests, run the following commands:

- yarn install
- yarn test

To set up the database, run the following commands:

- npx prisma db push
- npx prisma generate
