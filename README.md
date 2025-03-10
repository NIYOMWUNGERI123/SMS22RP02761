Laravel E-Commerce API
Introduction
This project is a Laravel-based e-commerce API that allows users to manage products, orders, sellers, and categories using RESTful API endpoints. The API supports authentication, CRUD operations, and category management using the nested set model.
Features
•	User authentication (Register, Login, Logout)
•	Product management (CRUD operations)
•	Order management
•	Seller dashboard for managing products
•	Category management using Laravel's nested set model
Requirements
•	PHP 8.0 or later
•	Composer
•	Laravel 10
•	MySQL database
•	Postman or Swagger for API testing
Installation Steps
1. Clone the Repository
 git clone https://github.com/your-username/ecommerce-api.git
 cd ecommerce-api
2. Install Dependencies
composer install
3. Configure Environment
Copy the .env.example file to .env and update database credentials:
cp .env.example .env
Edit the .env file to match your database settings:
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=online_store
DB_USERNAME=root
DB_PASSWORD=
4. Generate Application Key
php artisan key:generate
5. Run Migrations
php artisan migrate --seed
6. Start the Development Server
php artisan serve
Your API will be available at http://127.0.0.1:8000
API Endpoints
Authentication
•	POST /register - Register a new user
•	POST /login - Login and get API token
•	POST /logout - Logout
Product Management
•	GET /products - Retrieve all products
•	POST /products - Add a new product
•	GET /products/{id} - Get product details
•	PUT /products/{id} - Update a product
•	DELETE /products/{id} - Delete a product
Category Management
•	GET /categories - Retrieve all categories (XML format)
•	POST /categories - Create a new category
•	PUT /categories/{id} - Update a category
•	DELETE /categories/{id} - Delete a category
Testing the API
You can test the API using:
•	Postman: Import the API collection and send requests.
•	Swagger: Add API documentation using Laravel Swagger.
Deployment
To deploy the API, set up a production server with Apache/Nginx and run:
php artisan config:cache
php artisan route:cache
php artisan migrate --force
Contribution
Feel free to fork the repository and contribute by creating pull requests.
Contact
For any issues, contact: niyomwungerijean2022@gmail.com

