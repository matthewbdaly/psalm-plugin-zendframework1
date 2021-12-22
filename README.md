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

# DISCLAIMER

The stub files for this plugin were generated automatically, and I have noticed that the access levels for properties and methods aren't always accurate, leading to false errors when the implemented access level differs from that defined in the stub. For an example of a fix for this, see https://github.com/matthewbdaly/psalm-plugin-zendframework1/commit/1a83a78b805ad4430e04f454a819605f56efb996#diff-25a6634263c1b1f6fc4697a04e2b9904ea4b042a89af59dc93ec1f5d44848a26

If you see an error along those lines, please try running Psalm with this plugin disabled. If it then no longer flags the issue, it's likely the definition of that method or property in the stub file has a different access level to the one in the code base. If this is the case, please submit a pull request to correct the access level.
