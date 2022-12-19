### Udagram Pipeline

The Udagram pipeline manages the implementation of the code on AWS. Here are the general steps it takes:

## Build

- Installs all Node dependencies and configures Nodejs for running the application for the frontend
- Installs backend Node dependencies
- Lints the frontend code utilizing ESLint configuration
- Builds the frontend code using the Iconic build command
- Builds the backend API by transpiling Typescript source into JavaScript

## Approval

- Awaits approval from user to deploy to AWS
- This step only executes on the deploy branch

## Deploy

- Sets up the AWS CLI and EB CLI with env variables
- Runs same steps as in build stage for API and then the deploy scripts for the API which will bundle the compiled JavaScript code and zip it for EB CLI and then run the EB deploy command to deploy to environment
- Runs same steps as in build stage for frontend then uploads the build static web app to S3 using AWS CLI
- This step is only executed on the deploy branch (given approval)
