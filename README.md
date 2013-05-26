FancyBox Bundle for Symfony2
=======================

## Current Version

fancyBox 2.1.4

## Installation

### Add bundle to your composer.json file

``` js
// composer.json

{
    "require": {
		// ...
        "uran1980/fancybox-bundle": "*"
    }
}
```

### Add bundle to your application kernel

``` php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Uran1980\FancyBoxBundle\Uran1980FancyBoxBundle(),
        // ...
    );
}
```

### Download the bundle using Composer

``` bash
$ php composer.phar update uran1980/fancybox-bundle
```

### Install assets

Given your server's public directory is named "web", install the public vendor resources

``` bash
$ php app/console assets:install web
```

Optionally, use the --symlink attribute to create links rather than copies of the resources 

``` bash
$ php app/console assets:install --symlink web
```

## Usage

Refer to the desired files in your HTML template, e.g.

``` html
<script type="text/javascript" src="{{ asset('bundles/uran1980fancybox/js/fancybox/source/jquery.fancybox.pack.js') }}"></script>
```

## Licenses

Refer to the source code of the included files for license information

## References

1. http://www.fancyapps.com/fancybox/
2. http://symfony.com
