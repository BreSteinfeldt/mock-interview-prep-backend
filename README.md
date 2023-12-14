# Project Setup and Implementation Guide

This guide will walk you through the process of setting up a PostgreSQL database using ElephantSQL and implementing the backend functionality for posting and retrieving player data in your project.

## 1. Sign Up and Create a Database in ElephantSQL

1. Go to ElephantSQL (https://www.elephantsql.com/) and sign up for a free account.
2. Once you have signed up and logged in, create a new instance for your database.
3. Give your database instance a name and select the free plan (Tiny Turtle).
4. After creating the database, you will be redirected to the details page.

## 2. Find Your Database URL

1. On the details page of your newly created database, you will see a field labeled 'URL'. This is the connection string for your PostgreSQL database.
2. The URL will look something like this: postgres://user:password@host:port/database

## 3. Set Up .env File

1. In your project's root directory, create a new file and name it `.env`.
2. In this `.env` file, add the following line: DATABASE_URL=your_database_url

Replace `your_database_url` with the URL you copied from the ElephantSQL details page. This sets your database connection string as an environment variable which can be accessed in your application.

## 4. Install Project Dependencies

1. Run the following command in your terminal to install all necessary project dependencies: npm install

## 5. Run Database Setup Command

1. Run the following command in your terminal to execute the migration and seed files. This will set up your database structure and populate it with initial data:
npm run db:setup

## 6. Complete Implementation in Player Folder

1. Navigate to the `player` folder in your project. Here, you will find three main files: `players.controller.js`, `players.router.js`, and `players.service.js`.

### Posting a Player

- Open the `players.controller.js` file and complete the implementation for posting a player.

### Getting a Player

- Open the `players.controller.js` file and complete the implementation for getting a player.

## 7. Run the Test Command

1. Run the following command in your terminal to test if you have successfully completed the challenges: npm test

