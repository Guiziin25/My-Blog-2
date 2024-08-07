# My NodeJS Application

## Description
This is an application a blog where you can see posts and categories of posts and register and log in as a user, having an administrator user system being able to remove and create new posts,
developed in NodeJS using MongoDB as the database. The application utilizes the following libraries and frameworks:

- [ExpressJS](https://expressjs.com/): Fast, unopinionated, minimalist web framework for Node.js.
- [Handlebars](https://handlebarsjs.com/): Template engine for generating dynamic HTML.
- [Body Parser](https://github.com/expressjs/body-parser): Middleware for parsing the body of HTTP requests.
- [Passport](https://www.passportjs.org/): Simple, unobtrusive authentication for Node.js.

## Prerequisites
Before starting, make sure you have the following tools installed:

- [Node.js](https://nodejs.org/) v14.x or higher
- [MongoDB](https://www.mongodb.com/) v7.x or higher

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/Guiziin25/My-Blog-2.git
    ```
2. Navigate to the project directory:
    ```bash
    cd your-repository
    ```
3. Install the dependencies:
    ```bash
    npm install --save-dev nodemon
    npm install --save express mongoose body-parser handlebars connect-flash express-session passport
    ```
4. Set up the MySQL database. Create a database and configure the credentials in the `.env` file:
    ```dotenv
    PORT=3000
    MONGODB_URI=mongodb://localhost:27017/your-database-name
    SESSION_SECRET=your_secret_key
    ```

## Usage
1. Start the application:
    ```bash
    nodemon start
    ```
2. Access the application in your browser at `http://localhost:3000`.

## Project Structure
```plaintext
.
├── config
│   └── passport.js
├── models
│   └── User.js
├── routes
│   └── index.js
│   └── users.js
├── views
│   └── layouts
│       └── main.handlebars
│   └── index.handlebars
│   └── login.handlebars
├── .env
├── .gitignore
├── app.js
├── package.json
└── README.md
