# psalm-plugin-zendframework1

[![Build Status](https://travis-ci.org/matthewbdaly/psalm-plugin-zendframework1.svg?branch=master)](https://travis-ci.org/matthewbdaly/psalm-plugin-zendframework1)

Psalm plugin for Zend Framework 1

## Quickstart
Please refer to the [full Psalm documentation](https://psalm.dev/quickstart) for a more detailed guide on introducing Psalm
into your project.

First, start by installing Psalm if you have not done so already:
```bash
composer require --dev vimeo/psalm
./vendor/bin/psalm --init
```

Next, install this package and enable the plugin
```bash
composer require --dev matthewbdaly/psalm-plugin-zendframework1
./vendor/bin/psalm-plugin enable matthewbdaly/psalm-plugin-zendframework1
```

Finally, run Psalm to analyze your codebase
```bash
./vendor/bin/psalm
```
