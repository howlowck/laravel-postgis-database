# laravel-postgis-database
Forked from [this laravel-postgis-database](https://github.com/greglamb/laravel-postgis-database) (that seems to be abandoned)

Provides an extended Postgres driver for Laravel 4 that provides support for PostGIS features

# features

- Adds schema grammer for point
- Adds schema grammer for polygon

# install

## composer.json

Add a requirement for the package

```javascript
{
    "require": {
        "howlowck/laravel-postgis-database": "dev-master"
    }
}
```

## config/app.php

Add it to the list of providers

```php
'providers' => array(
  'Lamb\LaravelPostgisDatabase\PostgisDatabaseServiceProvider'
)
```

## config/database.php

Add a connection using the postgis driver instead of pgsql

```php
  'pgsql' => array(
    'driver'   => 'postgis',
    'host'     => 'localhost',
    'database' => 'database',
    'username' => 'root',
    'password' => '',
    'charset'  => 'utf8',
    'prefix'   => '',
    'schema'   => 'public',
  ),
```

# license

Released under the [MIT license](http://opensource.org/licenses/MIT)
