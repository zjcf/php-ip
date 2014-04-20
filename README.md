# PHP IP Library

IPv4/IPv6 manipulation library for PHP inspired by Python [ipaddress](https://docs.python.org/dev/library/ipaddress.html).

## Requirements

- PHP >= 5.2
- IPv6 support enabled
- GMP extension (www.php.net/manual/en/book.gmp.php)

## Installation

### Option 1 (PHP <= 5.2)

- [Download the single-file version](https://raw.githubusercontent.com/rlanvin/php-ip/master/ip.lib.php)
- `include` or `require` it
- Enjoy!

### Option 2 (PHP >= 5.3)

The recommend way is to install the lib [through Composer](http://getcomposer.org/).

Just add this to your `composer.json` file:

```JSON
{
    "require": {
        "rlanvin/php-ip": "dev/master"
    }
}
```

Then run `composer install` or `composer update`.

Now you can use the autoloader, and you will have access to the library:

```php
<?php
require 'vendor/autoload.php';
````

Caution: This library is compatible with PHP 5.2, therefore it is not namespaced.

## Documentation

Complete doc is available in [the wiki](https://github.com/rlanvin/php-ip/wiki).

## Disclaimer

I built this library for a project running PHP 5.2 (yep that's old). PHP 5.2 doesn't support late static binding, traits, namespaces and the like. So that explains some of the quirks of the design.

## License

This library is released under the MIT License.