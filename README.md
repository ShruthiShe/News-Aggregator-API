# News-Aggregator-API

## News Aggregator


## Setup Instructions
1. Rename the `.env.example` file to `.env` and update your database details:
   1. DB_DATABASE=your_database_name
   2. DB_USERNAME=your_database_user
   3. DB_PASSWORD=your_database_password
2. Run the following commands to set up the project:
   1. composer install
   2. php artisan key:generate
   3. php artisan vendor:publish --provider="Laravel\Sanctum\SanctumServiceProvider"
   4. php artisan migrate
   5. php artisan make:seeder ArticlesTableSeeder
   6. php artisan db:seed --class=ArticlesTableSeeder
   7. php artisan make:factory ArticleFactory
   8. php artisan vendor:publish --provider="L5Swagger\L5SwaggerServiceProvider"
   9. php artisan l5-swagger:generate
   10. php artisan serve


### Prerequisites:
- I am unable to work with Docker. I am getting an error, and even though I tried to solve it, I couldn't find a solution
- I haven’t worked on Docker yet
error msg as : An unexpected error occurred while executing a WSL command.

Either shut down WSL down with wsl --shutdown, and/or reboot your machine. You can also try reinstalling WSL and/or Docker Desktop. If the issue persists,



##Swagger/OpenAPI 
127.0.0.1:8000/api/documentation


Available Endpoints:
POST /api/auth/register - Register a new user
POST /api/auth/login - User login

GET /api/articles - Get all articles
GET /api/articles/{id} - Get a specific article
GET /api/articles/search - search

POST /api/preferences
GET /api/preferences


GET /api/personalized-feed

GET /api/fetch-newsapi
GET /api/fetch-nytimes
GET /api/fetch-guardian


I created a Mailtrap account for the password reset. I will receive the reset password message, then copy the link and paste it into Postman to hit the API and change the password.
