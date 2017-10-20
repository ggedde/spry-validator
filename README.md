# spry-validator
Default Validator for Spry Params

### Requires
* PHP 5.4^
* Spry-Core https://github.com/ggedde/spry-core

## Usage

```php

$name = Spry::validator()->validate('name'); // No Error on Failure
$id = Spry::validator()->required()->integer()->min(1)->validate('id'); // Spry Stop Error if Empty or not an Integer
$date = Spry::validator()->required()->date()->validate('date');  // Spry Stop Error if Empty or not a Date format
$password = Spry::validator()->required()->minLength(12)->validate('password');  // Spry Stop Error if Length is less then 12

```

## Full Documentation
https://github.com/blackbelt/php-validation
