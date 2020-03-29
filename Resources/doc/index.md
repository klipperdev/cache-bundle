Getting Started
===============

## Prerequisites

This version of the bundle requires Symfony 3.1+.

## Installation

Installation is a quick, 2 step process:

1. Download the bundle using composer
2. Enable the bundle
3. Configure the bundle (optional)


### Step 1: Download the bundle using composer

Tell composer to download the bundle by running the command:

```bash
$ composer require klipper/cache-bundle
```

Composer will install the bundle to your project's `vendor/klipper` directory.

### Step 2: Enable the bundle

Enable the bundle in the kernel:

```php
<?php
// app/AppKernel.php

public function registerBundles()
{
    $bundles = array(
        // ...
        new Klipper\Bundle\CacheBundle\KlipperCacheBundle(),
    );
}
```

### Step 3: Configure the bundle (optional)

You can override the default configuration adding `klipper_cache` tree in `app/config/config.yml`.
For see the reference of Klipper Cache Configuration, execute command:

```bash
$ php app/console config:dump-reference KlipperCacheBundle 
```

### Next Steps

Now that you have completed the basic installation and configuration of the
Klipper CacheBundle.
