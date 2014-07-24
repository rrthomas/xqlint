#XQLint
[![Build Status](http://img.shields.io/travis/wcandillon/xqlint/master.svg?style=flat)](https://travis-ci.org/wcandillon/xqlint) [![NPM version](http://img.shields.io/npm/v/xqlint.svg?style=flat)](http://badge.fury.io/js/xqlint) [![Code Climate](http://img.shields.io/codeclimate/github/wcandillon/xqlint.svg?style=flat)](https://codeclimate.com/github/wcandillon/xqlint)

## XQuery & JSONiq Code Quality Tool

XQLint parses XQuery & JSONiq files and returns errors and warnings based on static code analysis.

## Installation

Install Node.js and NPM for your system (Mac, Windows or Linux). And install the command line tool using:

```bash
$ npm install xqlint -g
```
## Usage

### Lint

```bash
$ xqlint lint <path> [-s, --style-check <yes, no>]
```
![result](https://dl.dropboxusercontent.com/u/1487285/Screenshot%202014-04-07%2011.06.31.png)

### Print AST as XML

```bash
$ xqlint ast <path>
```

### Syntax Highlighting

```bash
$ xqlint highlight <path>
```

## Development

If you'd like to hack on xqlint itself:

```bash
git clone git@github.com:wcandillon/xqlint.git
cd xqlint
npm install
grunt
```

### Run tests

```bash
grunt vows
```

### Generate Parsers

```bash
grunt parsers
```

##Who is using this project?
* [28.io cli tool](https://github.com/28msec/28)
* [ACE, aka the Cloud9 editor](https://github.com/ajaxorg/ace), [view demo](http://try.zorba.io).
* [XQLint Grunt Task](https://github.com/wcandillon/grunt-xqlint)

##Changelog
Version 0.1.2
* Fix bug on quantifier expressions

Version 0.1.1
* Improve "built-in" function resolving

Version 0.1.0
* Bug fixes

Version 0.0.9
* Add built-in schema types

Version 0.0.8
* Improve marker output in the cli.
* Improve function resolving
* Several bug fixes

Version 0.0.7
* Bug fixes.
* Make style check false by default.

Version 0.0.6
* Add code completion.
* Bug fixe with XQST0048.

Version 0.0.5
* Add code formatting command.

Version 0.0.4
* Add warnings for untyped module variables and functions.
* Fix syntax highlight bug for JSONiq.
* Add highlight command.

Version 0.0.3
* Exports XQLint module.
* Add code formatting checks.
