# CI-CD GitHub Actions
  ![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)
## Description 

This project showcases the use of GitHub actions using Cypress for testing and Render for deployment. These GitHub actions were created for a previously built, fully functioning application. The GitHub actions created, will run automated testing, building and deploying of the application.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [License](#license)
- [Tests](#tests)
- [Contact](#contact)

## Installation

In order to install this application, you will need to clone down the repository to your local machine. Once you have cloned it down, you will need to run an npm install and npm run build. After this has been completed, you will need to set up a MongoDB Atlas account and add your MONGO_DB_URI to a .env file. Next you will need to deploy the application to Render, make sure the build and start scripts are set up correctly. After it has been deployed without any errors, go to your Render settings and turn off automtic deploy. You should be able to test the GitHub actions now!

## Usage

To use the GitHub actions, you will need to create a feature branch and a develop branch. Pushing new code to the feature branch, then creating a pull requet to merge it to the develop branch will run the cypress tests to check to see if your new code is still functioning as intended. After the tests pass, you will be able to create a new pull request to merge the develop branch to your main branch. Here is where the GitHub actions will check to see if your application can still be deployed to Render. If the action also passes, it will automatically redeploy on Render with the new changes.

## Credits

This project was created by Alec Taber

## License
  
  This project uses the MIT License. For more information, visit [license link](https://opensource.org/licenses/MIT).

## Features

- Runs Cypress testing when a pull request is made to merge feature branch to develop branch
- Auto deploys newest commit when pull request is created and develop branch is merged to main branch

## Tests

To test the application using Cypress, first you will need to start the server. Do a npm run start, then open another terminal and do an npm run test-component. This will test the components of the application.

## Contact

- GitHub: [AlecTaber](https://github.com/AlecTaber)
- Email: [alectaber12@gmail.com](mailto:alectaber12@gmail.com)
