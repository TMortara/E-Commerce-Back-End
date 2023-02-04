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
10. Select `GET` from the dropdown to get data from the database and enter the `http://localhost:3001/api` URL
11. Add the following endpoints to make the `GET` requests:
    1. Product: 
        - endpoints:
            1. `/products`
            2. `/products/:id`
    2. Category: 
        - endpoints:
            1. `/categories`
            2. `/categories/:id`
    3. Tab: 
        - endpoints: 
            1. `/tags`
            2. `/tags/:id`

Sample `GET` requests
<img width="1437" alt="Screen Shot 2023-02-03 at 9 34 28 PM" src="https://user-images.githubusercontent.com/107971753/216746136-5f17aaf0-1957-4203-8ba9-0167a20419c5.png">

<img width="1436" alt="Screen Shot 2023-02-03 at 9 34 48 PM" src="https://user-images.githubusercontent.com/107971753/216746145-af97b8f9-9155-4ea0-ba81-d138e2e1b366.png">

11. Select 'POST' from the dropdown to create a new product, category, or tag and enter the `http://localhost:3001/api` URL
12. Add the following information to make the `POST` requests: 
    1. Product: 
        - endpoint: `/products`
        - request body: 
          {
            "product_name": "Flannel Shirts",
            "price": 40.00,
            "stock": 2,
            "tagIds": [1, 4]
          }
    2. Category: 
        - endpoint: `/categories`
        - request body: 
        {
            "category_name": "hiking gear"
        }
    3. Tab: 
        - endpoint: `/tags`
        - request body: 
        {
            "tag_name": magenta
        }
        
Sample `POST` Request
    <img width="1431" alt="Screen Shot 2023-02-03 at 9 35 58 PM" src="https://user-images.githubusercontent.com/107971753/216746243-2e6b60d9-b01b-4aef-8c02-f60c512a89eb.png">

13. Select `PUT` from the dropdown to update a product, category, or tag and enter the `http://localhost:3001/api` URL
14. Add the following endpoints to make the `PUT` requests: 
    1. Product: 
        - endpoint: `/products/:id`
        - request body: 
          {
            "product_name": "Flannel Shirts",
            "price": 48.00,
          }
    2. Category: 
        - endpoint: `/categories/:id`
        - request body: 
        {
            "category_name": "hiking shoes"
        }
    3. Tab: 
        - endpoint: `/tags/:id`
        - request body: 
        {
            "tag_name": teal
        }
        
Sample `PUT` Request
<img width="1440" alt="Screen Shot 2023-02-03 at 9 36 54 PM" src="https://user-images.githubusercontent.com/107971753/216746265-4e816ee2-29aa-4505-8e32-bc9a77815f24.png">

15. Select `DELETE` from the dropdown to delete a product, category, or tag and enter the `http://localhost:3001/api` URL
16. Add the following endpoints to make the `DELETE` requests
    1. Product: 
        - endpoint: `/products/:id`
    2. Category: 
        - endpoint: `/categories/:id`
    3. Tab: 
        - endpoint: `/tags/:id`

Sample `DELETE` Request
<img width="1440" alt="Screen Shot 2023-02-03 at 9 37 38 PM" src="https://user-images.githubusercontent.com/107971753/216746306-e8ee1ab5-5d68-4725-b8b4-a2cab08c8898.png">

17. Exit Insomnia
18. Close server with command `^C`

## File Structure
The directory for this application is as follows:
- /config: configuration file for database
- /db: database schema
- /models: contains the Category, Product, and Tags models
- /routes: route files for Category, Product, and Tags
- /seeds: seed data for the database

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

### GET Requests
[Untitled_ Feb 3, 2023 9_27 PM.webm](https://user-images.githubusercontent.com/107971753/216745771-5cab2265-8e84-4533-8c8d-fbc8feaeb899.webm)

### POST and PUT Requests
[Untitled_ Feb 3, 2023 8_54 PM.webm](https://user-images.githubusercontent.com/107971753/216745269-27cad631-682f-4d40-930c-3cdafb002be4.webm)

### DELETE Requests
[Untitled_ Feb 3, 2023 9_02 PM.webm](https://user-images.githubusercontent.com/107971753/216744733-d258bc48-e284-43a2-bde9-bedce6d9074a.webm)


