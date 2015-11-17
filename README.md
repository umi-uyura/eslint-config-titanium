eslint-config-titanium
======================

ESLint configuration for Appcelerator Titanium.

Usage
-----

### Install

[ESLint](https://github.com/eslint/eslint) must be installed in advance.

```
$ npm install -g https://github.com/umi-uyura/eslint-config-titanium
```

### Configuration

Set `titanium` to `extends` key.

``` javascript
{
  "extends": "titanium",
  ...
}
```

When combined with multiple `extends` , be set in the array.

``` javascript
{
  "extends": [
    "eslint:recommended",
    "titanium"
  ],
  ...
}
```

Linting
-------

Mainly will allow global value specific to Titanium and Alloy.

See *eslintrc.json*

``` javacript
{
  "globals": {
    "Titanium": false,
    "Ti": false,
    "Alloy": false,
    "$": false,
    "_": false,
    "OS_IOS": false,
    "OS_ANDROID": false,
    "OS_MOBILEWEB": false,
    "OS_WINDOWS": false,
    "ENV_DEV": false,
    "ENV_TEST": false,
    "ENV_PRODUCTION": false,
    "DIST_ADHOC": false,
    "DIST_STORE": false,
    "task": false
  }
}
```
