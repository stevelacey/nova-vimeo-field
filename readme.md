# Laravel Nova Vimeo Field

[![Packagist License](https://poser.pugx.org/stevelacey/nova-vimeo-field/license.png)](http://choosealicense.com/licenses/mit/)
[![Latest Stable Version](https://poser.pugx.org/stevelacey/nova-vimeo-field/version.png)](https://packagist.org/packages/stevelacey/nova-vimeo-field)
[![Total Downloads](https://poser.pugx.org/stevelacey/nova-vimeo-field/d/total.png)](https://packagist.org/packages/stevelacey/nova-vimeo-field)

Laravel Nova Vimeo field stores the id out of any given Vimeo link/embed, and renders a player.

![Vimeo player](https://raw.githubusercontent.com/stevelacey/nova-vimeo-field/master/screenshot.png)

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
