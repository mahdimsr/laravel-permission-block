# Associate users with permissions and roles

## About
This package is forked from [laravel-permission](https://github.com/spatie/laravel-permission/tree/main) developed by [spatie](https://spatie.be)

## What It Different?
In additional main package, this package allows you to block user from permissions

Once installed you can do stuff like this:

```php
// Block user from permission
$user->blockFromPermission('edit articles');

$user->hasBlockFromPermission('edit articles');
```

in main repo all permissions will be registered on [Laravel's gate](https://laravel.com/docs/authorization), you can check if a user has a permission with Laravel's default `can` function, but it not checking the blocked permissions.
we will handle it in next releases.

```php

$user->blockFromPermission('edit articles');

$user->hasBlockFromPermission('edit articles'); // return true

$user->can('edit articles'); // return true: it not check blocked permissions
```

## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.


### Testing

``` bash
composer test
```

### Security

If you discover any security-related issues, please email [mahdi.msr4@gmail.com](mailto:mahdi.msr4@gmail.com).

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
