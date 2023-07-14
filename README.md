# Associate users with permissions and roles

## About
This package is forked from [laravel-permission](https://github.com/spatie/laravel-permission/tree/main) developed by [spatie](https://spatie.be)

## What It Different?
In additional main package, this package allows you to block user from permissions

Once installed you can do stuff like this:

```php
$user->blockedPermissions // all permissions are blocked for user

// Block user from permission
$user->blockFromPermission('edit articles');
$user->blockFromPermission(['edit articles','view post']);

$user->hasBlockFromPermission('edit articles'); // return true
$user->hasDirectPermission('edit articles'); // return false
$user->hasPermissionTo('edit articles'); // return false
$user->can('edit articles'); // return false

$user->hasBlockFromAnyPermission(['edit article','view post']) // return true if any of passing permissions array are blocked

$user->unblockFromPermission('view post')
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
