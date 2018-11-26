# Pipers-Seekers-Backend Documentation
### Contents
* [Build Status](#Build-Status)

* [Getting Started](#getting-started)
* [Authors & Credits](#Authors)
* [Test Coverage](#Tests)
* [Architecture](##Architecture)

## Version

1.0.0

## Description
Piper's Seekers backend is a fork of the Finders Keepers backend at  https://github.com/spyosaurus/finders-keepers-backend
This fork was created by Finders Keepers team member Jennifer Piper, to allow her to freely modify and upgrade her own version of the original Finders Keepers game.

## Build Status
[![Build Status](https://travis-ci.org/jenwill-pipers-seekers-backend.svg?branch=master)](https://travis-ci.org/jenwill-pipers-seekers-backend)


## Architecture
Piper's Seekers is a full-stack application, utilizing the following:

- Code Style: Airbnb
- Test Suite: Jest
- Transpiling: Babel
- Ajax Requests: Superagent
- Continuous Integration: Travis CI
- Misc: Eslint, dotenv
## Backend
- Framework: Express
- Database: MongoDB
- Logging: Winston
- CORS: cors

## Frontend
- View Library: React
- State Management: Redux
- Bundler: Webpack
- Style: Sass
### Misc 
- Css-loader,
- Enzyme, Prop-Types,
- mini-css-extra-plugin, html-webpack-plugin


## ENV Files
- In your BACK END .env file, enter the following:
```

NODE_ENV=development
PORT=3000
DEBUG=true
CORS_ORIGIN=http://localhost:8080

MONGODB_URI=mongodb://localhost/testing

FINDERS_SECRET=yoursecretcodegoeshere
```
- In your FRONT END .env file, enter the following:
```
NODE_ENV=development
API_URL=http://localhost:3000
```

## Getting Started:
1. Fork both FRONTEND AND BACKEND repositories from GitHub.
2. Clone the repo to your local machine.
3. Run the ```npm i``` command in the frontend and backend to install all required dependencies.
4. IN THE BACKEND, Run the ```node index.js``` command in your terminal.
5. IN THE BACKEND, Run the ```npm run test``` command in your terminal.
6. IN THE FRONTEND run the ```npm run test``` command to run testing on frontend.
7. IN THE FRONTEND run the ```npm run watch``` command to render application to the browser. 

## socket.IO
This application uses Socket.io in order to have multiplayer functionality in real time!
Players join a socket when they click "host" or "join" and after they have signed in or registered if they do not have an account. Once all the players are in the waiting room, the host will start the game.

## Tests
## Load Testing
####  All times are in miliseconds
 - Created 100 virtual users every second for 5 seconds
```
All virtual users finished
Summary report @ 12:49:09(-0700) 2018-06-21
  Scenarios launched:  500
  Scenarios completed: 500
  Requests completed:  500
  RPS sent: 90.74
  Request latency:
    min: 20.3
    max: 58.6
    median: 21.8
    p95: 24.8
    p99: 37
  Scenario counts:
    0: 500 (100%)
  Codes:
    409: 500
    
```
- Created 200 virtual users every second for 10 seconds.
```
All virtual users finished
Summary report @ 13:02:15(-0700) 2018-06-21
  Scenarios launched:  2000
  Scenarios completed: 2000
  Requests completed:  2000
  RPS sent: 189.75
  Request latency:
    min: 20.9
    max: 91.5
    median: 44.3
    p95: 71.1
    p99: 80.5
  Scenario counts:
    0: 2000 (100%)
  Codes:
    409: 2000
```
- Created 250 virtual users every second for 5 seconds
```
All virtual users finished
Summary report @ 13:05:32(-0700) 2018-06-21
  Scenarios launched:  3750
  Scenarios completed: 3750
  Requests completed:  3750
  RPS sent: 202.16
  Request latency:
    min: 30.3
    max: 3096.5
    median: 1403.2
    p95: 2926.1
    p99: 3055.8
  Scenario counts:
    0: 3750 (100%)
  Codes:
    409: 3750
```
- Test Suite: Jest
- npm run test
- Backend Coverage:
- Frontend Coverage:

## Authors

Cara Ottmar, Collin Meredith, Jennifer Piper and Wyatt Pefley

## Credits 
- Heath Smith
- Sockit to me 401 team
- Thank you to all TAs and instructor Vinicio!

License: MIT