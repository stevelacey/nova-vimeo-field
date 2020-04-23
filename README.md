# Laravel Nova Vimeo Field

[![Latest Version on Packagist](https://img.shields.io/packagist/v/stevelacey/nova-vimeo-field.svg?style=flat-square)](https://packagist.org/packages/stevelacey/nova-vimeo-field)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE.md)
[![Total Downloads](https://img.shields.io/packagist/dt/stevelacey/nova-vimeo-field.svg?style=flat-square)](https://packagist.org/packages/stevelacey/nova-vimeo-field)

Laravel Nova Vimeo field stores the id out of any given Vimeo link/embed, and renders a player.

## Installation

```bash
composer require stevelacey/nova-vimeo-field
```

## Usage

Define the following fields in your resource in the `fields` method:

```php
use Steve\NovaVimeoField\Vimeo;

...

Vimeo::make('Video')
    ->withMeta([
        'options' => [
            'width' => 640,
            'height' => 360,
        ]
    ]);
```

## Screenshot

![Vimeo player](https://raw.githubusercontent.com/stevelacey/nova-vimeo-field/master/screenshot.png)
