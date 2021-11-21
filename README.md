# E-commerce Backend

## Description
This is code for a back end ecommerce site. This setup utilizes Express, sequelize, mysql2, and dotenv npm packages. The API endpoints will allow you to perform CRUD operations on Categories, Products, and Tags within the database.

## Installation Instructions
See the instructional video here: [Instructional Video](https://youtu.be/7mMPFUTNeNI)

> Required Software
- Node
- MySQL

> Optional Software
- VS Code, with the MySQL extension
- Insomnia

> Instructions
1. Clone this repository, then enter it
2. Install Node modules by running `npm i`
3. Create a `.env` file in the root directory and populate it with the following, adding in the corresponding info between the single quotes:
    - DB_NAME=''
    - DB_USER=''
    - DB_PW=''
4. At the command line, log in to mysql by entering `mysql -u <username> -p`, where `<username>` is the username above.
5. At the prompt, enter the database password for the user.
6. Once logged in, run the command `source db/schema.sql` to create the database, then run `exit`
7. At the command line, run `node seeds/index.js` to seed the database
8. At this point, you're ready to go!


## Usage Instructions
To start the server, run `npm start` at the command line. When you see `App listening on port ####` you're up and running!

Use the models in the `models` folder to see the object structure for each object, and use the endpoints below to perform CRUD operations.


## API Endpoints
See the Models folder for object structure.

- `/api/categories`
    - `GET` gets all categories
    - `POST` creates a new category
- `/api/categories/<id>` where `<id>` is the id number of the category
    - `GET` gets the information on the category with the matching ID
    - `PUT` updates the category with the corresponding ID
    - `DELETE` removes the category with the corresponding ID
- `/api/products`
    - `GET` gets all products
    - `POST` creates a new product
- `/api/products/<id>` where `<id>` is the id number of the product
    - `GET` gets the information on the product with the matching ID
    - `PUT` updates the product with the corresponding ID
    - `DELETE` removes the product with the corresponding ID
- `/api/tags`
    - `GET` gets all tags
    - `POST` creates a new tag
- `/api/tags/<id>` where `<id>` is the id number of the tag
    - `GET` gets the information on the tag with the matching ID
    - `PUT` updates the tag with the corresponding ID
    - `DELETE` removes the tag with the corresponding ID


## Author
Elliott Kvamme, 2021


