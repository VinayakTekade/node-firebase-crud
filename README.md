# Node Firebase CRUD Application

<!-- PROJECT LOGO -->
<br />

<!-- ABOUT THE PROJECT -->

## About The Project

This repository contains the source code for a dummy student record application made with NodeJS and Firebase Firestore.

### Built With

This web application uses the following technology

- [NodeJS](https://nodejs.org)
- [ExpressJS](https://expressjs.com/)
- [Firebase](https://firebase.google.com/)

<!-- GETTING STARTED -->

## Getting Started

To run this application use the following steps

1. Clone the repo

   ```sh
   git clone https://github.com/VinayakTekade/node-firebase-crud.git
   ```

2. Install NPM packages in client directory and server directory
   ```sh
   cd node-firebase-crud
   npm install
   ```
3. Create a firebase firestore database
4. Add your firebase service account API key as `./serviceAccountToken.json`

### Prerequisites

You need to have the following Prerequisite to get started

- NodeJS
- Firebase Account

## Project Structure

| Path       | Description                                                                            |
| ---------- | -------------------------------------------------------------------------------------- |
| controller | This directory contains all the files that add functionality with your database.       |
| models     | This directory contains the schemas of all the database documents                      |
| routes     | This directory contains all the files that deal with api endpoints                     |
| config.js  | This file contains all the configuration definitions for the project                   |
| db.js      | This file connects with the database and provides all the firebase database operations |
| index.js   | This file contains the code to run the server                                          |

## List of APIs

| API Routes    | Parameters | Description                                                                                                                                                                                                                              |
| ------------- | ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| /api/students | none       | Sends a json with records of all the students if it exists or sends status code 404.                                                                                                                                                     |
| /api/student  | id         | For a POST request, sends a json with record of a student if it exists or sends status code 404. <br /> For a PUT request, updates the student record.<br /> For a DELETE request deletes the student record based on id sent as a param |

<!-- CONTRIBUTING -->

## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
