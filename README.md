conventional-bump
====================

[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)

bump `package.json` version according to [conventional-changelog](https://github.com/conventional-changelog/conventional-changelog).


`conventional-bump` is built on [conventional-recommended-bump](https://github.com/conventional-changelog/conventional-changelog/tree/master/packages/conventional-recommended-bump).


Purpose of this library is to automatically bump the package.json version number.

## Installation
```bash
npm install --save-dev conventional-bump
```

## Usage
```bash
$ conventional-bump --help

Usage: index.js [-p preset]

Options:
  --version     Print current version                                  [boolean]
  -h, --help    Show help                                              [boolean]
  -p, --preset  conventional-changelog preset to use        [default: "angular"]
```

## Configuration
in your package.json :
```json
{
  "scripts": {
    "bump": "conventional-bump -p angular",
    "version": "conventional-changelog -p angular -i CHANGELOG.md -s -r 0 && git add CHANGELOG.md"
  }
}
```
