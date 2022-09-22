# panjs
## Validators
[![Build Status](https://travis-ci.com/ashwinbande/validators.svg?branch=master)](https://travis-ci.com/ashwinbande/validators)
[![](https://data.jsdelivr.com/v1/package/npm/@ashwinbande/validators/badge?style=rounded)](https://www.jsdelivr.com/package/npm/@ashwinbande/validators)
[![codecov](https://codecov.io/gh/ashwinbande/validators/branch/master/graph/badge.svg)](https://codecov.io/gh/ashwinbande/validators)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![npm version](https://badge.fury.io/js/%40ashwinbande%2Fvalidators.svg)](https://badge.fury.io/js/%40ashwinbande%2Fvalidators)
![npm](https://img.shields.io/npm/dm/@ashwinbande/validators.svg)
![npm bundle size (scoped)](https://img.shields.io/bundlephobia/min/@ashwinbande/validators.svg)
![Snyk Vulnerabilities for npm package version](https://img.shields.io/snyk/vulnerabilities/npm/@ashwinbande/validators.svg)
---------------------------------------
#### This package provides validation of PAN Card of an individual. (Made in India)
## Installation

### NodeJS
```javascript
    npm i panjs
```
In your .js file add following code

```javascript
    const isValid = require('panjs')
```

## Usage

#### 1. PAN (Permanent Account Number):
validates => Input must be in format `AAAAA####A`, and have length 10 and fourth character must be either A, B, C, F, G, H, L, J, P, T, E.
```javascript
isValid.pan('AAACT2727Q')  /* returns true  */
isValid.pan('11ACT2727Q')  /* returns false */
```
You can also obtain PAN holder type by -
```javascript
isValid.pan.holder('AAACT2727Q')  /* returns 'Company'  */
```
possible values are -
```
A: Association Of Persons (AOP),
B: Body Of Individuals (BOI),
C: Company,
F: Firm,
G: Government,
H: Hindu Undivided Family (HUF),
L: Local Authority,
J: Artificial Juridical Person,
P: Individual (Proprietor),
T: Trust (AOP),
E: Limited Liability Partnership (LLP),
```

------------------------------------

#### For Feature requests and Error reporting:
create an issue on [github repository](https://github.com/tazimmadre/panjs/issues) or contact directly to [tazimmadre5041@gmail.com](mailto:tazimmadre5041@gmail.com)

##### **Don't Forget to add a star to [github repo](https://github.com/tazimmadre/panjs). Please provide your comments, suggest improvements and other codes which are not covered in this package.
