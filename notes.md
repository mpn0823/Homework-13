#Develop/config/middleware/isAuthenticated.js
    No Dependencies.
    Middleware that express uses to check that a user is logged in (i.e. user has a valid session token stored locally) before
    serving restricted routes.

#Develop/config/config.json
    No Dependencies.
    File contains an object with all the data necessary for sequelize to establish a connection with local database.

#Develop/config/passport.js
    Dependencies are passport, passport-local, and models.  
    File configures passport to handle authentication using passport-local strategy.

#Develop/models/index.js
    Dependencies are sequelize, config.json.
    This file is provided when you install and setup Sequelize.  It creates corresponding tables that app author has defined in a file(s) in the models directory.

#Develop/models/user.js
    Dependencies are bcrypt.
    This file defines the table 'user' for sequelize to use in storing user's email and password.  The bcrypt library is used to hash passwords so that it isn't necessary to store the plain text.

#Develop/node-modules/*
    It's huge!

#Develop/public/js/login.js
    This file contains the logic the log in page.

#Develop/public/js/members.js
    This file just does a GET request to figure out which user is logged in and updates the HTML on the page.

#Develop/public/js/signup.js
    This file contains the logic for the signup page

#Develop/public/stylesheets/style.css
    CSS styling rules utilized by HTML files.

#Develop/public/login.html
    HTML document that presents a login form and then runs login.js

#Develop/public/members.html
    HTMl landing page for logged in user; runs members.js

#Develop/public/signup.html
    Nearly the same as login.html except that it runs signup.js instead.

#Develop/routes/api-routes.js
    Dependencies are passport.js and models directory.
    Defines all the api routes that interact with the database using sequelize.

#Develop/routes/html-routes.js
    Dependencies are isAuthenticated.js
    Defines all the routes that are used to serve static html files.

#Develop/package.json
    JSON object that contains all the data required to install necessary app dependencies via npm

#Develop/package-lock.json
    Dependencies for our dependencies for our dependencies for our dependencies.

#Develop/server.js
    Dependencies are express, express-session, our passport.js.
    This is the server app.  It is configured to pass data as JSON, intereact with the database using sequelize, and track user's logged in status with session tokens.










