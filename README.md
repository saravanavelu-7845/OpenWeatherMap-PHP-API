OpenWeatherMap PHP API
======================
A PHP 7.0+ API to retrieve and parse global weather data from
[OpenWeatherMap.org](http://www.OpenWeatherMap.org).
This project aims to normalise the provided data and remove inconsistencies.
It is not maintained by OpenWeatherMap and not an official API wrapper.

[![Build Status](https://travis-ci.org/cmfcmf/OpenWeatherMap-PHP-Api.svg?branch=master)](https://travis-ci.org/cmfcmf/OpenWeatherMap-PHP-Api)
[![license](https://img.shields.io/github/license/cmfcmf/OpenWeatherMap-PHP-Api.svg)](https://github.com/cmfcmf/OpenWeatherMap-PHP-Api/blob/master/LICENSE)
[![release](https://img.shields.io/github/release/cmfcmf/OpenWeatherMap-PHP-Api.svg)](https://github.com/cmfcmf/OpenWeatherMap-PHP-Api/releases)
[![codecov](https://codecov.io/gh/cmfcmf/OpenWeatherMap-PHP-Api/branch/master/graph/badge.svg)](https://codecov.io/gh/cmfcmf/OpenWeatherMap-PHP-Api)
[![Scrutinizer Quality Score](https://scrutinizer-ci.com/g/cmfcmf/OpenWeatherMap-PHP-Api/badges/quality-score.png?s=f31ca08aa8896416cf162403d34362f0a5da0966)](https://scrutinizer-ci.com/g/cmfcmf/OpenWeatherMap-PHP-Api/)
<br>
[![SensioLabsInsight](https://insight.sensiolabs.com/projects/0addfb24-e2b4-4feb-848e-86b2078ca104/big.png)](https://insight.sensiolabs.com/projects/0addfb24-e2b4-4feb-848e-86b2078ca104)

Documentation
=============

You can find the latest documentation, including installation and usage instructions at https://cmfcmf.github.io/OpenWeatherMap-PHP-API.

Contributing
============
I'm happy about every **pull request** you open and **issue** you find to help make this API **more awesome**. Please note that it might sometimes take me a while to get back to you. Feel free to ping me if I don't respond.

## Vagrant

You can use [Vagrant](https://vagrantup.com) to kick-start your development.
Simply run `vagrant up` and `vagrant ssh` to start a PHP VM with all
dependencies included.

## Docker

You can also use Docker to start developing this library. First install dependencies:

    docker run --rm --interactive --tty \
        --volume $PWD:/app \
        --user $(id -u):$(id -g) \
        composer install

And then execute an example:

    docker run --rm --interactive --tty \
        --volume $PWD:/app -w /app \
        php bash

    > php Examples/CurrentWeather.php

## Documentation

The documentation is built using [Docusuaurs v2](https://v2.docusaurus.io/).
To run a local developnment server for the docs, execute

```bash
cd docs
yarn install
yarn start
```

License
=======

This project is licensed under the MIT license.
Please see the [LICENSE file](https://github.com/Cmfcmf/OpenWeatherMap-PHP-Api/blob/master/LICENSE)
distributed with this source code for further information regarding copyright and licensing.

Be aware that the OpenWeatherMap data is **not licensed under the MIT**.
**Check out the following official links to read about the terms, pricing and license of OpenWeatherMap before using their service:**

- [OpenWeatherMap.org/terms](http://OpenWeatherMap.org/terms)
- [OpenWeatherMap.org/appid](http://OpenWeatherMap.org/appid)
