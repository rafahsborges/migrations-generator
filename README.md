# Laravel Migrations Generator Laravel 10 +

Generate Laravel Migrations from an existing database, including indexes and foreign keys!

# Contact

https://t.me/rafahsborges

## Laravel 10 installation

The recommended way to install this is through composer:

```bash
composer require rafahsborges/migrations-generator --dev
```

In Laravel 10 the service providers will automatically get registered.

## Usage

To generate migrations from a database, you need to have your database setup in Laravel's Config.

Run `php artisan migrate:generate` to create migrations for all the tables, or you can specify the tables you wish to generate using `php artisan migrate:generate table1,table2,table3,table4,table5`. You can also ignore tables with `--ignore="table3,table4,table5"`

Laravel Migrations Generator will first generate all the tables, columns and indexes, and afterwards setup all the foreign key constraints. So make sure you include all the tables listed in the foreign keys so that they are present when the foreign keys are created.

You can also specify the connection name if you are not using your default connection with `--connection="connection_name"`

Run `php artisan help migrate:generate` for a list of options.

Check out Chung Tran's blog post for a quick step by step introduction: [Generate Migrations from an existing database in Laravel 4](http://codingtip.blogspot.com/2014/04/laravel-4-generate-migration-existed-dabase-laravel-4.html)

## Changelog

Changelog for Laravel Migrations Generator

### Ago 2023: v3.0.0
* Minimum supported versions: PHP 8.0 and Laravel 10

## Thank You

Thanks to Jeffrey Way and OscarDev for their unique packages. This package depends significantly on their work.

## Contributors

Rafah S Borges ([@rafahsborges](https://www.linkedin.com/in/rafael-souza-borges-92995426/))

rafahsborges@outlook.com

## License

The Laravel Migrations Generator is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT)
