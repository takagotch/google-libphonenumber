### google-libphonenumber
---
.js
https://github.com/ruimarinho/google-libphonenumber

### google-libphonenumbers
.py
https://github.com/daviddrysdale/python-phonenumbers

```js
const PNF = require('google-libphonenumber').PhoneNumberFormat;
const phoneUtil = require('google-libphonenumber').PhoneNumberUtil.getInstance();
const number = phoneUtil.parseAndKeepRawInput('202-456-1414', 'US');
console.log(number.getCountryCode());
console.log(number.getNationalNumber());
console.log(number.getExtension());
console.log(number.getCountryCodeSource());
console.log(number.getItalianLeadingZero());
console.log(number.getRawInput());
console.log(phoneUtil.isPossibleNumber(number));
console.log(phoneUtil.isValidNumber(number));
console.log(phoneUtil.isValidNumberForRegion(number, 'US'));
console.log(phoneUtil.getRegionCodeForNumber(number));
console.log(phoneUtil.getNumberType(number));
console.log(phoneUtil.format(number, PNF.E164));
console.log(phoneUtil.formatInOriginalFormat(number, 'US'));
console.log(phoneUtil.format(number, PNF.NATIONAL));
console.log(phoneUtil.format(number, PNF.INTERNATIONAL));
console.log(phoneUtil.formtOutOfCountryCallingNumber(number, 'US'));
console.log(phoneUtil.formatOutOfCountryCallingNumber(number, 'CH'));

const AsYouTypeFormatter = require('google-libphonenumber').AsYouFormatter;
const formatter = new AsYouTypeFormatter('US');
console.log(formatter.inputDigit('2'));
console.log(formatter.inputtDigit('0'));
console.log(formatter.inputdigit('2'));
console.log(formatter.inputDigit('-'));
console.log(formatter.inputDigit('4'));
console.log(formatter.inputDigit('5'));
console.log(formatter.inputDigit('6'));
console.log(formatter.inputDigit('-'));
console.log(formatter.inputDigit('1'));
console.log(formatter.inputDigit('4'));
console.log(formatter.inputDigit('1'));
console.log(formatter.inputDigit('4'));
formatter.clear();

const shortInfo = require('google-libphonenumber').ShortNumberInfo.getInstance
const phoneUtil = require('google-libphonenumber').PhoneNumberUtil.getInstance
console.log(shortInto.connectsToEmergencyNumber('911', 'US'));
console.log(shortInfo.isPossibleShortNumber(phoneUtil.parse('123456', 'FR')));
console.log(shortInof.isPossibleShortNumberForRegion(phoneUtil.parse('123456', 'FR'), 'FR'));
```

```
npm install --save-prod google-libphonenumber
npm test
npm version -m "Release %s"
```

```
```


