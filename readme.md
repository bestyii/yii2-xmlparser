
[![Build Status](https://img.shields.io/travis/bestyii/yii2-xmlparser.svg?style=flat-square)](http://travis-ci.org/bestyii/yii2-xmlparser)
[![version](https://img.shields.io/packagist/v/bestyii/yii2-xmlparser.svg?style=flat-square)](https://packagist.org/packages/bestyii/yii2-xmlparser)
[![Download](https://img.shields.io/packagist/dt/bestyii/yii2-xmlparser.svg?style=flat-square)](https://packagist.org/packages/bestyii/yii2-xmlparser)
[![Issues](https://img.shields.io/github/issues/bestyii/yii2-xmlparser.svg?style=flat-square)](https://github.com/bestyii/yii2-xmlparser/issues)

## Overview

This is a library help you to handle the xml request. As we all know, [Yii2](https://github.com/yiisoft/yii2) provided an built-in request parser for `json` like requests, it's `yii\web\JsonParser`. Sometimes, we need to handle the request of xml, so this library is birthed.

## Install

Add `bestyii/yii2-xmlparser` to composer.json, you can assign version as `*`:

```sh
$ composer install
//or run
$ composer update
```

also we can do like this:

```sh
$ composer require bestyii/yii2-xmlparser --prefer-dist
```

## Usage

```
# file app/config/main.php [your configuration file]
<?php

return [
    'components' => [
    'request' => [
        'parsers' => [
	        	'text/xml' => 'bestyii\xml\parser\XmlParser',
	            'application/xml' => 'bestyii\xml\parser\XmlParser',
	        ],
        ],
    ],
];

```

## Test

```
$ phpunit
```
## LICENSE

![MIT](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)
