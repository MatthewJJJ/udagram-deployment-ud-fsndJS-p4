# Udagram Overview

This application was built as part of the last section of the Udacity Full Stack JavaScript Developer Nanodegree Program. It's a full stack application (Node.js/Express.js backend and Angular Frontend) that's been hosted on AWS using Elasticbeanstalk for the backend, S3 for the frontend, and RDS (Postgres) for the database.

Backend URL: `http://udagram-api-dev.eba-dqpuc6sp.us-east-1.elasticbeanstalk.com/api/v0/feed`

Frontend URL: `http://udagram-deployment-mjf-udnanodegree.s3-website-us-east-1.amazonaws.com`

Screenshot of Hosted Web App: ![plot](./screenshots/Working%20App%20Screenshot.jpg)

### Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```

### Installation

Provision the necessary AWS services needed for running the application:

1. Export the ENV variables needed or use a package like [dotnev](https://www.npmjs.com/package/dotenv)/.
1. From the root of the repo, navigate udagram-api folder `cd starter/udagram-api` to install the node_modules `npm install`. After installation is done start the api in dev mode with `npm run dev`.
1. Without closing the terminal in step 1, navigate to the udagram-frontend `cd starter/udagram-frontend` to intall the node_modules `npm install`. After installation is done start the api in dev mode with `npm run start`.

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd starter/udagram-frontend`
1. `npm run test`
1. `npm run e2e`

There are no Unit test on the back-end

### Unit Tests:

Unit tests are using the Jasmine Framework.

### End to End Tests:

The e2e tests are using Protractor and Jasmine.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## License

[License](LICENSE.txt)
