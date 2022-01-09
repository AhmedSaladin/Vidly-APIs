# Project Goals

- Implement CRUD operations
- Store complex, relational data in MongoDB using Mongoose
- Implement data validation
- Implement authentication and authorization
- Handle and log errors effectively
- Set up configuration for various environments (dev, test, prod)
- Write unit and integration tests
- Build features using test-driven development

## About Project

Video rental APIs

## Setup

Make sure to follow all these steps exactly as explained below. Do not miss any steps or you won't be able to run this application.

### Install MongoDB

To run this project, you need to install the latest version of MongoDB Community Edition first.

`https://docs.mongodb.com/manual/installation/`

Once you install MongoDB, make sure it's running.

### Install MongoDB

To run this project, you need to install the latest version of MongoDB Community Edition first.

https://docs.mongodb.com/manual/installation/

Once you install MongoDB, make sure it's running.

### Install the Dependencies

Next, from the project folder, install the dependencies:

    npm i

### Populate the Database

    node seed.js

### Run the Tests

You're almost done! Run the tests to make sure everything is working:

    npm test

All tests should pass.

### Start the Server

    node index.js

This will launch the Node server on port 3900. If that port is busy, you can set a different point in config/default.json.

Open up your browser and head over to:

http://localhost:3900/api/genres

You should see the list of genres. That confirms that you have set up everything successfully.

### Environment Variables

You need to create `default.json` file in `config` folder in project root folder and setup default enviroment variables.

- `jwtPrivateKey` : used to encrypt JSON web tokens
- `db` : used to hold mongoDB connection string

  On Windows:

      set jwtPrivateKey = yourSecureKey
      set db = yourDBconnectionString

  Powershell:

      New-Item -Path '.\config\default.json' -ItemType File -Force
