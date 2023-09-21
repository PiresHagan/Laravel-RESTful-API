# Laravel implementation of FilmDb backend

Laravel application that stores data for movies. This is an educational repo for the graduate software development classes of BMSZC Petrik Lajos Technikum.

## Installation steps

- Let's make a copy of the .env.example file named .env.
  
  ```sh
  cp .env.example .env
  ```

- In the file, rewrite the data of the database connection to the appropriate one!

- Execute the following instructions in the console:

  ```sh
  composer install
  php artisan key:generate --ansi
  php artisan migrate --seed
  ```

- The development server can be started with the following command:

  ```sh
  php artisan serve
  ```

- Let's check that everything is fine, that the following URL test returns JSON data:
  <http://localhost:8000/api/film>
