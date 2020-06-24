# Getting started

## Installation

Please check the official Lumen installation guide for server requirements before you start. [Official Documentation](https://lumen.laravel.com/docs/5.5/installation)


Clone the repository

    git clone https://github.com/zagalvelozo/Lumen-JWT.git

Switch to the repo folder

    cd Lumen-JWT

Install all the dependencies using composer

    composer install

Copy the example env file and make the required configuration changes in the .env file

    cp .env.example .env

Generate a new application key

Since Lumen doesn't have the `php artisan key:generate` command, there's a custom route `http://localhost:8000/appKey` to help you generate an application key.

Generate a new JWT authentication secret key

    php artisan jwt:secret

Run the database migrations (**Set the database connection in .env before migrating**)

    php artisan migrate

Start the local development server

    php -S localhost:8000 -t public

You can now access the server at http://localhost:8000
