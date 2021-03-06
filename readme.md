## Steps for application first running

- Run command
```
composer install
```
- edit .env.example to setup environment
- setup environment for database. Example: open config/database.php, set 'default' => 'sqlite', then run
```
touch storage/database.sqlite
```
- then run migrations
```
php artisan migrate
```
- then add some tags, for example:
```
php artisan tinker
$tags = ['personal', 'work', 'food', 'coding'];
foreach($tags as $tag){\App\Tag::create(['name' => $tag]);}
```

## Laravel PHP Framework

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable, creative experience to be truly fulfilling. Laravel attempts to take the pain out of development by easing common tasks used in the majority of web projects, such as authentication, routing, sessions, queueing, and caching.

Laravel is accessible, yet powerful, providing powerful tools needed for large, robust applications. A superb inversion of control container, expressive migration system, and tightly integrated unit testing support give you the tools you need to build any application with which you are tasked.

## Official Documentation

Documentation for the framework can be found on the [Laravel website](http://laravel.com/docs).
Video tutorial [laravel 5 fundamental](https://laracasts.com/series/laravel-5-fundamentals).

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](http://laravel.com/docs/contributions).

### License

The Laravel framework is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT)
