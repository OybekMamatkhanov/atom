# Atom Framework
[![SensioLabsInsight](https://insight.sensiolabs.com/projects/af681361-67b8-4fd9-b2ab-e7645c2bb63f/mini.png)](https://insight.sensiolabs.com/projects/af681361-67b8-4fd9-b2ab-e7645c2bb63f)

## Installation

The simplest way to install and get started is using the skeleton project:
```bash
$ composer create-project atomwares/atom-project <project dir>
```
Or install Atom standalone using Composer:
```bash
$ composer require atomwares/atom
```

## Usage

Create a bootstrap file with the following contents:
```php
<?php

require 'vendor/autoload.php';

($app = new Atom\App())->router
  ->get(['home' => '/'], function () {
        return 'Hello World!';
    });

$app->run();
```

You may run the script using the built-in PHP server:
```bash
$ php -S localhost:8000
```

## License

The Atom Framework is licensed under the MIT license. See [License File](LICENSE) for more information.
