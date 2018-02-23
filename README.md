# Drupal Finder

[![Travis](https://img.shields.io/travis/webflo/drupal-finder.svg)](https://travis-ci.org/webflo/drupal-finder) [![Packagist](https://img.shields.io/packagist/v/webflo/drupal-finder.svg)](https://packagist.org/packages/webflo/drupal-finder)

Drupal Finder provides a class to locate a Drupal installation in a given path.

## Usage

```PHP
$drupalFinder = new \DrupalFinder\DrupalFinder();
if ($drupalFinder->locateRoot(getcwd())) {
    $drupalRoot = $drupalFinder->getDrupalRoot();
    $composerRoot = $drupalFinder->getComposerRoot();
    ...
}
```

## Usage on Drupal 7 sites not built with composer

Copy ```d7-no-composer.composer.json``` to ```composer.json``` . Defaults assume your Drupal installation is in a subdirectory of your project directory, and that this subdirectory is named ```docroot```.

## Examples

- [Drupal Console Launcher](https://github.com/hechoendrupal/drupal-console-launcher)
- [Drush Launcher](https://github.com/drush-ops/drush-launcher)

## License

GPL-2.0+
