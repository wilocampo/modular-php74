# Fork Notice

This is a PHP 7.4 compatible fork of [InterNACHI/modular](https://github.com/InterNACHI/modular).

## Why This Fork Exists

The original [InterNACHI/modular](https://github.com/InterNACHI/modular) package requires PHP >= 8.0. This fork was created to provide PHP 7.4 and Laravel 8.x compatibility while maintaining the same functionality.

## Changes Made

1. **PHP Version Support**: Changed from PHP >= 8.0 to PHP >= 7.4
2. **Laravel Support**: Compatible with Laravel 8.x (original supports Laravel 9+)
3. **Syntax Compatibility**:
   - Removed constructor property promotion (converted to traditional property assignments)
   - Replaced `str_contains()` with `strpos()` checks
   - Replaced `str_starts_with()` with `Str::startsWith()`
   - Fixed union types in return types
   - Fixed catch blocks without variables
   - Replaced dynamic `::class` with `get_class()`

## Installation

```bash
composer require internachi/modular-php74:@dev
```

Or add to your `composer.json`:

```json
{
    "repositories": [
        {
            "type": "vcs",
            "url": "https://github.com/YOUR_USERNAME/modular-php74"
        }
    ],
    "require": {
        "internachi/modular-php74": "@dev"
    }
}
```

## Credits

- Original package: [InterNACHI/modular](https://github.com/InterNACHI/modular) by [Chris Morrell](http://www.cmorrell.com)
- Fork maintained for PHP 7.4 / Laravel 8.x compatibility

## License

Same as the original: MIT License
