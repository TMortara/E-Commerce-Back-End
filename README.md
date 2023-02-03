# E-Commerce-Back-End

## Description
Back end e-commerce application that allows a company to manage their product inventory.

## Table of Contents
- [Installation Steps](#installation-steps)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Built With](#built-with)
- [Resources Used to Complete Project](#resources-used-to-complete-project)
- [License](#license)
- [Recording](#recording)
- [Screenshots of Application](#screenshots-of-application)

## Installation Steps
Before using this application you must [install Node.js](https://nodejs.org/en/).

After installing Node.js, open the integrated terminal in VS Code and run `npm install`.  This will install all of the dependencies listed in the package.json file. 

<u>Installation Resources</u>:
- [Install Express.js](https://expressjs.com/en/starter/installing.html)
- [Install Sequelize](https://sequelize.org/docs/v6/getting-started/)
- [Install Insomnia](https://docs.insomnia.rest/insomnia/install)


## Usage
1. Before beginning make sure you have completed the [Installation Steps](#installation-steps)
2. Open integrated terminal in VS Code
3. Sign into your MySQL database by running `mysql -u root -p` then enter your password
4. From the Command Line run `SOURCE db/schema.sql;` 
5. Next run `USE ecommerce_db;`
6. Next you will need to seed your database.  Exit MySQL and run `node seeds/index.js`
7. Once you database is seeded you can run `node server.js` to start your server.
8. Open Insomnia
9. From the Insomnia Dashboard select `Debug`
10. Select `GET` from the dropdown and enter the `http://localhost:3001/api/` URL
11. Make the following `GET` requests:
    1. 
12. Make the following `POST` requests: 
13. Make the following `PUT` requests: 
14. Make the following `DELETE` requests
 

## File Structure
The directory for this application is as follows:
- 

## Built With:
![JavaScript](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white) ![Insomnia](https://img.shields.io/badge/Insomnia-5849be?style=for-the-badge&logo=Insomnia&logoColor=white) ![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white) ![Sequelize](https://img.shields.io/badge/Sequelize-52B0E7?style=for-the-badge&logo=Sequelize&logoColor=white)

## Resources Used to Complete Project
### Sequelize Documentation
 - [Model Querying Basics](https://sequelize.org/docs/v6/core-concepts/model-querying-basics/)
 - [Sub Queries](https://sequelize.org/docs/v7/core-concepts/validations-and-constraints/#note-about-allownull-implementation)
 - [Advanced M:N Associations](https://sequelize.org/docs/v6/advanced-association-concepts/advanced-many-to-many/#through-tables-versus-normal-tables-and-the-super-many-to-many-association)
 - [Associations](https://sequelize.org/docs/v6/core-concepts/assocs/)

## License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Recording

## Screenshots of Application




