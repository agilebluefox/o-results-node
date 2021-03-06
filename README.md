# O-Results Node JS Server

The server and database portion for the O-Results application. It provides data models, RESTful API's for various routes, data validation and a customizable logging system.

## Technical Skills

Express, Git/Github, Gulp, Mocha and Chai, MongoDB, Mongoose, Node, Node-Validator, Winston

## Breakdown

This project is the backend portion of the O-Results App which tracks students participating on various courses at an orienteering event. The RESTful API is setup using the Express JS library providing routes for each of the data models mirrored as collections in the MongoDB NoSQL database. The database models are built using Mongoose and provide server-side validation rules in combination with the node-validator library using both default and custom-designed validators. The project includes mock data which can be added to the database by running a Gulp task that targets the test classes built using Mocha and Chai.

## Notable Features

I'm very interested in including testing and logging features into my applications. In this application, I used the Winston JS logging library to provide a sophisticated logging system that can be easily configured to allocate runtime messages that are based upon the logging level requested. These messages are useful in monitoring the server operations for debugging purposes in development mode and informational purposes when the Node JS server is running in production mode.

## Run the Code

To begin, use `npm install` to download the packages and dependencies required by the server. Next, edit the 'mongod' script in  package.json to point to the location of the MongoDb database on your machine. To populate the database required for the app, run `npm tests` to ensure the data is ready and all the associated tests are passing. Finally, run `npm start` to activate the server instance.