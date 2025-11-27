# PHP Sandbox Environment

For quickly hoisting a PHP proof of concept (POC) or prototype with quality checks and tests, this repository provides a ready-to-use sandbox environment.

- Uses PHP 8.3
- Scan your POC/prototype with PHPStan level 8.
- Scan your POC/prototype phpcs using PSR-12 standard.
- Test with PHPUnit.

![test status](https://github.com/johnsonoriginals/php_sandbox/actions/workflows/php.yml/badge.svg)

After checkout, installing the project is simple:
```bash
composer install
```

How to run the tests:
```bash
user@container:/var/www/html# composer run-script test 
```
See the composer.json file for more scripts and details.

If you want to see test results in a more detailed format, run:
```bash
./vendor/bin/phpunit --testdox
```

Expected directory structure for your POC/prototype:
```
/project-root
├── src
│   └── Your PHP source files here
├── tests
│   └── Your PHPUnit test files here
├── composer.json
└── phpunit.dist.xml
...and other files as needed
```

For contribution guidelines, see
[CONTRIBUTING.md](CONTRIBUTING.md)

License information can be found in
[MIT.md](MIT.md)