# Laravel Passport Cache Token

Make [laravel/passport](https://github.com/laravel/passport) token cacheable.

## Installing

```shell
$ composer require richardmichel/passport-cache-token -vvv
```

## Usage

Thanks to Laravel's automatic package discovery mechanism, you don't need to do any additional operations.

Of course, you can also control the cache strategy freely, just need to configure the following in the configuration file:

**config/passport.php**
```php
return [
    //...
    'cache' => [
        // Cache key prefix
        'prefix' => 'passport_',
        
        // The lifetime of token cache,
        // Unit: second
        'expires_in' => 300,
        
        // Cache tags
        'tags' => [],
    ],
];
```
