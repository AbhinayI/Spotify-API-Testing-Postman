# Spotify API Testing using Postman and Newman

## Overview
This project is aimed at testing the Spotify API using Postman and Newman. It provides a collection of test cases to verify the functionality of the Spotify API endpoints. The collection can be run using Newman and can be integrated with Jenkins for continuous integration.

## Features
- Postman collection with tests for Spotify API endpoints
- API Chaining
- Set Global,Collection and Environment Variables 
- Tests are run using Newman, the Postman command-line tool
- Integration with Jenkins for continuous integration

## Prerequisites
- Postman
- Node.js installed
- Newman Package
- Newman htmlextra
- Jenkins

## Installation and Execution
1. Clone the repository
2. Import the `Spotify API Tests.postman_collection.json` file into Postman
3. Import the `Spotify API Tests.postman_environment.json` file into Postman and set the necessary variables
4. Start the tests by running "newman run Spotify API Tests.postman_collection.json -r htmlextra"

## Integration with Jenkins
1. Set up a Jenkins job to run the tests using Newman
2. Add a build step to run the command "newman run Spotify API Tests.postman_collection.json -r htmlextra"
3. Configure the job to publish the test results using the Postman plugin

## Variables
![Screenshot (13)](https://user-images.githubusercontent.com/122073049/218938936-c79e079e-c15e-4b19-a102-ca36f5f45eda.png)

## Reports
Reports are generated by Newman with htmlextra plugin.

![Screenshot (16)](https://user-images.githubusercontent.com/122073049/218939610-793af3aa-0d0c-4dac-902c-7d42ea5b6494.png)
![Screenshot (17)](https://user-images.githubusercontent.com/122073049/218939635-457009f0-e1c1-4b2d-818f-0d56b8ef9406.png)
