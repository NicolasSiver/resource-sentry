# Resource Sentry

Bring static resources (SCSS, JSON, XML) to JavaScript.

![Version](https://img.shields.io/npm/v/resource-sentry.svg)
![Dependencies](https://david-dm.org/NicolasSiver/resource-sentry.svg)
![bitHound Score](https://www.bithound.io/github/NicolasSiver/resource-sentry/badges/score.svg)
![Code Climate](https://img.shields.io/codeclimate/github/NicolasSiver/resource-sentry.svg)
[![Coverage Status](https://coveralls.io/repos/github/NicolasSiver/resource-sentry/badge.svg?branch=master)](https://coveralls.io/github/NicolasSiver/resource-sentry?branch=master)

**Work in progress**

## Motivation

Multi-language support? Project variables. Style variables. What if you want utilize power of namespaces in XML to build a collaborative source for multi-language support? What if you want to store style-related variables in SCSS, but you need to make some computation in runtime. Most of the data formats are not supported by browsers, - solution is to compile resources before code will be execute on user's machine and use "resources" as an efficient JavaScript code.

Example:

```
// _vars.scss
$my-padding: 8px;

// main.js
import Rs from './res/rs';

Rs.getResource(Rs.Style.MY_PADDING); // 8
```
