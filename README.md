# ZF2 Debugger ported from Nette Framework
Provides user friendly error and exception handling.

## Features

- User friendly errors and exceptions
- Can write error log
- Can notify by email
- Discrete production server error page

## Setup

Following steps are necessary to get this module working (considering a zf2-skeleton or very similar application)

  1. Run `php composer.phar require webino/zf2nette-debug:1.*`
  2. Add `ZF2NetteDebug` to the enabled modules list

## Showcase

![local error](http://files.nette.org/2398/debugger2.png "Errors & Exceptions")
![public error](http://files.nette.org/2398/debugger3.png "Title")

## Changelog

### 1.1.1

- Fix error/index Can only throw objects Fatal Error.

### 1.1.0

- Nette bar disabled by default + toggle option.

## About Nette Debugger

- homepage: http://doc.nette.org/cs/debugging

This component is initially provided by the Nette Framework.

- homepage: http://nette.org
- repository: http://github.com/nette/nette
