# Auth0 JWT Dummy

Use this library in your projects to replace the one used by [Auth0 PHP](https://github.com/auth0/auth0-PHP) solving the [Lcobucci namespace problem](https://github.com/auth0/auth0-PHP/issues?q=lcobucci%2Fjwt). This will then allow
you to not have a conflicting namespace with the [Lcobucci JWT](https://github.com/lcobucci/jwt) library.

## Installation

Add this GitHub repository to your composer.json file in the following format.
The [repositories key](https://getcomposer.org/doc/05-repositories.md#vcs) is a top level one that might not be contained in your composer.json
file and will need to be added.

```json
...
"repositories": [
    {
        "type": "git",
        "url": "https://github.com/peterfox/auth0-php-jwt-dummy"
    }
]
...
```

Then install the package:

```shell
composer require auth0/php-jwt:"dev-main as 3.3.4"
```

At the moment [3.3.4](https://github.com/auth0/php-jwt/tree/3.3.4) is the latest release used by Auth0 PHP, but you might need to change
the version depending on if a new release will be made by them.