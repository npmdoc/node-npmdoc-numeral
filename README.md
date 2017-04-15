# api documentation for  [numeral (v2.0.6)](http://numeraljs.com)  [![npm package](https://img.shields.io/npm/v/npmdoc-numeral.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-numeral) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-numeral.svg)](https://travis-ci.org/npmdoc/node-npmdoc-numeral)
#### Format and manipulate numbers.

[![NPM](https://nodei.co/npm/numeral.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/numeral)

[![apidoc](https://npmdoc.github.io/node-npmdoc-numeral/build/screenCapture.buildCi.browser.apidoc.html.png)](https://npmdoc.github.io/node-npmdoc-numeral/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-numeral/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-numeral/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Adam Draper",
        "url": "http://github.com/adamwdraper"
    },
    "bugs": {
        "url": "https://github.com/adamwdraper/Numeral-js/issues"
    },
    "dependencies": {},
    "description": "Format and manipulate numbers.",
    "devDependencies": {
        "chai": "^3.5.0",
        "grunt": "latest",
        "grunt-contrib-copy": "^1.0.0",
        "grunt-contrib-jshint": "latest",
        "grunt-contrib-nodeunit": "1.0.0",
        "grunt-contrib-uglify": "latest",
        "grunt-karma": "^2.0.0",
        "grunt-mocha-test": "^0.13.2",
        "grunt-saucelabs": "*",
        "grunt-string-replace": "^1.3.1",
        "karma": "^1.3.0",
        "karma-chai": "^0.1.0",
        "karma-chrome-launcher": "^2.0.0",
        "karma-firefox-launcher": "^1.0.0",
        "karma-mocha": "^1.3.0",
        "karma-mocha-reporter": "^2.2.1",
        "karma-sauce-launcher": "^1.1.0",
        "load-grunt-tasks": "^3.5.2",
        "mocha": "^3.1.2",
        "uglify-js": "latest"
    },
    "directories": {},
    "dist": {
        "shasum": "4ad080936d443c2561aed9f2197efffe25f4e506",
        "tarball": "https://registry.npmjs.org/numeral/-/numeral-2.0.6.tgz"
    },
    "ender": "./ender.js",
    "engines": {
        "node": "*"
    },
    "gitHead": "30956925463d19d4cf84488dcd8005da40cf9728",
    "homepage": "http://numeraljs.com",
    "keywords": [
        "numeral",
        "number",
        "format",
        "time",
        "money",
        "percentage"
    ],
    "license": "MIT",
    "main": "./numeral.js",
    "maintainers": [
        {
            "name": "adamwdraper"
        }
    ],
    "name": "numeral",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/adamwdraper/Numeral-js.git"
    },
    "scripts": {
        "test": "grunt"
    },
    "version": "2.0.6"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module numeral](#apidoc.module.numeral)
1.  [function <span class="apidocSignatureSpan"></span>numeral (input)](#apidoc.element.numeral.numeral)
1.  [function <span class="apidocSignatureSpan">numeral.</span>defaultFormat (format)](#apidoc.element.numeral.defaultFormat)
1.  [function <span class="apidocSignatureSpan">numeral.</span>isNumeral (obj)](#apidoc.element.numeral.isNumeral)
1.  [function <span class="apidocSignatureSpan">numeral.</span>locale (key)](#apidoc.element.numeral.locale)
1.  [function <span class="apidocSignatureSpan">numeral.</span>localeData (key)](#apidoc.element.numeral.localeData)
1.  [function <span class="apidocSignatureSpan">numeral.</span>nullFormat (format)](#apidoc.element.numeral.nullFormat)
1.  [function <span class="apidocSignatureSpan">numeral.</span>register (type, name, format)](#apidoc.element.numeral.register)
1.  [function <span class="apidocSignatureSpan">numeral.</span>reset ()](#apidoc.element.numeral.reset)
1.  [function <span class="apidocSignatureSpan">numeral.</span>toString ()](#apidoc.element.numeral.toString)
1.  [function <span class="apidocSignatureSpan">numeral.</span>validate (val, culture)](#apidoc.element.numeral.validate)
1.  [function <span class="apidocSignatureSpan">numeral.</span>zeroFormat (format)](#apidoc.element.numeral.zeroFormat)
1.  object <span class="apidocSignatureSpan">numeral.</span>_
1.  object <span class="apidocSignatureSpan">numeral.</span>fn
1.  object <span class="apidocSignatureSpan">numeral.</span>formats
1.  object <span class="apidocSignatureSpan">numeral.</span>locales
1.  object <span class="apidocSignatureSpan">numeral.</span>options
1.  string <span class="apidocSignatureSpan">numeral.</span>version

#### [module numeral._](#apidoc.module.numeral._)
1.  [function <span class="apidocSignatureSpan">numeral._.</span>correctionFactor ()](#apidoc.element.numeral._.correctionFactor)
1.  [function <span class="apidocSignatureSpan">numeral._.</span>includes (string, search)](#apidoc.element.numeral._.includes)
1.  [function <span class="apidocSignatureSpan">numeral._.</span>insert (string, subString, start)](#apidoc.element.numeral._.insert)
1.  [function <span class="apidocSignatureSpan">numeral._.</span>isNaN (value)](#apidoc.element.numeral._.isNaN)
1.  [function <span class="apidocSignatureSpan">numeral._.</span>multiplier (x)](#apidoc.element.numeral._.multiplier)
1.  [function <span class="apidocSignatureSpan">numeral._.</span>numberToFormat (value, format, roundingFunction)](#apidoc.element.numeral._.numberToFormat)
1.  [function <span class="apidocSignatureSpan">numeral._.</span>reduce (array, callback)](#apidoc.element.numeral._.reduce)
1.  [function <span class="apidocSignatureSpan">numeral._.</span>stringToNumber (string)](#apidoc.element.numeral._.stringToNumber)
1.  [function <span class="apidocSignatureSpan">numeral._.</span>toFixed (value, maxDecimals, roundingFunction, optionals)](#apidoc.element.numeral._.toFixed)

#### [module numeral.fn](#apidoc.module.numeral.fn)
1.  [function <span class="apidocSignatureSpan">numeral.fn.</span>add (value)](#apidoc.element.numeral.fn.add)
1.  [function <span class="apidocSignatureSpan">numeral.fn.</span>clone ()](#apidoc.element.numeral.fn.clone)
1.  [function <span class="apidocSignatureSpan">numeral.fn.</span>difference (value)](#apidoc.element.numeral.fn.difference)
1.  [function <span class="apidocSignatureSpan">numeral.fn.</span>divide (value)](#apidoc.element.numeral.fn.divide)
1.  [function <span class="apidocSignatureSpan">numeral.fn.</span>format (inputString, roundingFunction)](#apidoc.element.numeral.fn.format)
1.  [function <span class="apidocSignatureSpan">numeral.fn.</span>input ()](#apidoc.element.numeral.fn.input)
1.  [function <span class="apidocSignatureSpan">numeral.fn.</span>multiply (value)](#apidoc.element.numeral.fn.multiply)
1.  [function <span class="apidocSignatureSpan">numeral.fn.</span>set (value)](#apidoc.element.numeral.fn.set)
1.  [function <span class="apidocSignatureSpan">numeral.fn.</span>subtract (value)](#apidoc.element.numeral.fn.subtract)
1.  [function <span class="apidocSignatureSpan">numeral.fn.</span>value ()](#apidoc.element.numeral.fn.value)



# <a name="apidoc.module.numeral"></a>[module numeral](#apidoc.module.numeral)

#### <a name="apidoc.element.numeral.numeral"></a>[function <span class="apidocSignatureSpan"></span>numeral (input)](#apidoc.element.numeral.numeral)
- description and source-code
```javascript
numeral = function (input) {
    var value,
        kind,
        unformatFunction,
        regexp;

    if (numeral.isNumeral(input)) {
        value = input.value();
    } else if (input === 0 || typeof input === 'undefined') {
        value = 0;
    } else if (input === null || _.isNaN(input)) {
        value = null;
    } else if (typeof input === 'string') {
        if (options.zeroFormat && input === options.zeroFormat) {
            value = 0;
        } else if (options.nullFormat && input === options.nullFormat || !input.replace(/[^0-9]+/g, '').length) {
            value = null;
        } else {
            for (kind in formats) {
                regexp = typeof formats[kind].regexps.unformat === 'function' ? formats[kind].regexps.unformat() : formats[kind].
regexps.unformat;

                if (regexp && input.match(regexp)) {
                    unformatFunction = formats[kind].unformat;

                    break;
                }
            }

            unformatFunction = unformatFunction || numeral._.stringToNumber;

            value = unformatFunction(input);
        }
    } else {
        value = Number(input)|| null;
    }

    return new Numeral(input, value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral.defaultFormat"></a>[function <span class="apidocSignatureSpan">numeral.</span>defaultFormat (format)](#apidoc.element.numeral.defaultFormat)
- description and source-code
```javascript
defaultFormat = function (format) {
    options.defaultFormat = typeof(format) === 'string' ? format : '0.0';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral.isNumeral"></a>[function <span class="apidocSignatureSpan">numeral.</span>isNumeral (obj)](#apidoc.element.numeral.isNumeral)
- description and source-code
```javascript
isNumeral = function (obj) {
    return obj instanceof Numeral;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral.locale"></a>[function <span class="apidocSignatureSpan">numeral.</span>locale (key)](#apidoc.element.numeral.locale)
- description and source-code
```javascript
locale = function (key) {
    if (key) {
        options.currentLocale = key.toLowerCase();
    }

    return options.currentLocale;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral.localeData"></a>[function <span class="apidocSignatureSpan">numeral.</span>localeData (key)](#apidoc.element.numeral.localeData)
- description and source-code
```javascript
localeData = function (key) {
    if (!key) {
        return locales[options.currentLocale];
    }

    key = key.toLowerCase();

    if (!locales[key]) {
        throw new Error('Unknown locale : ' + key);
    }

    return locales[key];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral.nullFormat"></a>[function <span class="apidocSignatureSpan">numeral.</span>nullFormat (format)](#apidoc.element.numeral.nullFormat)
- description and source-code
```javascript
nullFormat = function (format) {
    options.nullFormat = typeof(format) === 'string' ? format : null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral.register"></a>[function <span class="apidocSignatureSpan">numeral.</span>register (type, name, format)](#apidoc.element.numeral.register)
- description and source-code
```javascript
register = function (type, name, format) {
    name = name.toLowerCase();

    if (this[type + 's'][name]) {
        throw new TypeError(name + ' ' + type + ' already registered.');
    }

    this[type + 's'][name] = format;

    return format;
}
```
- example usage
```shell
...

### 2.0.0

2.0.0 brings a lot of breaking changes and a reorganization of the repo, but also simplifies the api as well as the creating of
custom formats.

Breaking change / Feature: All formats are now separate files.  This makes it easy to create custom formats, and will also allow
 for custom builds with only certain formats.  (Note: The built numeral.js still contains all formats in the repo).

Breaking change / Feature: All formats and locales are now loaded using 'numeral.register(type, name, {})'

Breaking change: All 'language' now renamed to 'locale' and standardized to all lowercase filenames

Breaking change: The 'locale' function no longer loads locales, it only sets the current locale

Breaking change: The 'unformat' function has been removed 'numeral().unformat(string)' and now happens on numeral init 'numeral(
string)'
...
```

#### <a name="apidoc.element.numeral.reset"></a>[function <span class="apidocSignatureSpan">numeral.</span>reset ()](#apidoc.element.numeral.reset)
- description and source-code
```javascript
reset = function () {
    for (var property in defaults) {
        options[property] = defaults[property];
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral.toString"></a>[function <span class="apidocSignatureSpan">numeral.</span>toString ()](#apidoc.element.numeral.toString)
- description and source-code
```javascript
toString = function () {
    return toString;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral.validate"></a>[function <span class="apidocSignatureSpan">numeral.</span>validate (val, culture)](#apidoc.element.numeral.validate)
- description and source-code
```javascript
validate = function (val, culture) {
    var _decimalSep,
        _thousandSep,
        _currSymbol,
        _valArray,
        _abbrObj,
        _thousandRegEx,
        localeData,
        temp;

    //coerce val to string
    if (typeof val !== 'string') {
        val += '';

        if (console.warn) {
            console.warn('Numeral.js: Value is not string. It has been co-erced to: ', val);
        }
    }

    //trim whitespaces from either sides
    val = val.trim();

    //if val is just digits return true
    if (!!val.match(/^\d+$/)) {
        return true;
    }

    //if val is empty return false
    if (val === '') {
        return false;
    }

    //get the decimal and thousands separator from numeral.localeData
    try {
        //check if the culture is understood by numeral. if not, default it to current locale
        localeData = numeral.localeData(culture);
    } catch (e) {
        localeData = numeral.localeData(numeral.locale());
    }

    //setup the delimiters and currency symbol based on culture/locale
    _currSymbol = localeData.currency.symbol;
    _abbrObj = localeData.abbreviations;
    _decimalSep = localeData.delimiters.decimal;
    if (localeData.delimiters.thousands === '.') {
        _thousandSep = '\\.';
    } else {
        _thousandSep = localeData.delimiters.thousands;
    }

    // validating currency symbol
    temp = val.match(/^[^\d]+/);
    if (temp !== null) {
        val = val.substr(1);
        if (temp[0] !== _currSymbol) {
            return false;
        }
    }

    //validating abbreviation symbol
    temp = val.match(/[^\d]+$/);
    if (temp !== null) {
        val = val.slice(0, -1);
        if (temp[0] !== _abbrObj.thousand && temp[0] !== _abbrObj.million && temp[0] !== _abbrObj.billion && temp[0] !== _abbrObj
.trillion) {
            return false;
        }
    }

    _thousandRegEx = new RegExp(_thousandSep + '{2}');

    if (!val.match(/[^\d.,]/g)) {
        _valArray = val.split(_decimalSep);
        if (_valArray.length > 2) {
            return false;
        } else {
            if (_valArray.length < 2) {
                return ( !! _valArray[0].match(/^\d+.*\d$/) && !_valArray[0].match(_thousandRegEx));
            } else {
                if (_valArray[0].length === 1) {
                    return ( !! _valArray[0].match(/^\d+$/) && !_valArray[0].match(_thousandRegEx) && !! _valArray[1].match(/^\d
+$/));
                } else {
                    return ( !! _valArray[0].match(/^\d+.*\d$/) && !_valArray[0].match(_thousandRegEx) && !! _valArray[1].match(/^\d+$/));
                }
            }
        }
    }

    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral.zeroFormat"></a>[function <span class="apidocSignatureSpan">numeral.</span>zeroFormat (format)](#apidoc.element.numeral.zeroFormat)
- description and source-code
```javascript
zeroFormat = function (format) {
    options.zeroFormat = typeof(format) === 'string' ? format : null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.numeral._"></a>[module numeral._](#apidoc.module.numeral._)

#### <a name="apidoc.element.numeral._.correctionFactor"></a>[function <span class="apidocSignatureSpan">numeral._.</span>correctionFactor ()](#apidoc.element.numeral._.correctionFactor)
- description and source-code
```javascript
correctionFactor = function () {
    var args = Array.prototype.slice.call(arguments);

    return args.reduce(function(accum, next) {
        var mn = _.multiplier(next);
        return accum > mn ? accum : mn;
    }, 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral._.includes"></a>[function <span class="apidocSignatureSpan">numeral._.</span>includes (string, search)](#apidoc.element.numeral._.includes)
- description and source-code
```javascript
includes = function (string, search) {
    return string.indexOf(search) !== -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral._.insert"></a>[function <span class="apidocSignatureSpan">numeral._.</span>insert (string, subString, start)](#apidoc.element.numeral._.insert)
- description and source-code
```javascript
insert = function (string, subString, start) {
    return string.slice(0, start) + subString + string.slice(start);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral._.isNaN"></a>[function <span class="apidocSignatureSpan">numeral._.</span>isNaN (value)](#apidoc.element.numeral._.isNaN)
- description and source-code
```javascript
isNaN = function (value) {
    return typeof value === 'number' && isNaN(value);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral._.multiplier"></a>[function <span class="apidocSignatureSpan">numeral._.</span>multiplier (x)](#apidoc.element.numeral._.multiplier)
- description and source-code
```javascript
multiplier = function (x) {
    var parts = x.toString().split('.');

    return parts.length < 2 ? 1 : Math.pow(10, parts[1].length);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral._.numberToFormat"></a>[function <span class="apidocSignatureSpan">numeral._.</span>numberToFormat (value, format, roundingFunction)](#apidoc.element.numeral._.numberToFormat)
- description and source-code
```javascript
numberToFormat = function (value, format, roundingFunction) {
    var locale = locales[numeral.options.currentLocale],
        negP = false,
        optDec = false,
        leadingCount = 0,
        abbr = '',
        trillion = 1000000000000,
        billion = 1000000000,
        million = 1000000,
        thousand = 1000,
        decimal = '',
        neg = false,
        abbrForce, // force abbreviation
        abs,
        min,
        max,
        power,
        int,
        precision,
        signed,
        thousands,
        output;

    // make sure we never format a null value
    value = value || 0;

    abs = Math.abs(value);

    // see if we should use parentheses for negative number or if we should prefix with a sign
    // if both are present we default to parentheses
    if (numeral._.includes(format, '(')) {
        negP = true;
        format = format.replace(/[\(|\)]/g, '');
    } else if (numeral._.includes(format, '+') || numeral._.includes(format, '-')) {
        signed = numeral._.includes(format, '+') ? format.indexOf('+') : value < 0 ? format.indexOf('-') : -1;
        format = format.replace(/[\+|\-]/g, '');
    }

    // see if abbreviation is wanted
    if (numeral._.includes(format, 'a')) {
        abbrForce = format.match(/a(k|m|b|t)?/);

        abbrForce = abbrForce ? abbrForce[1] : false;

        // check for space before abbreviation
        if (numeral._.includes(format, ' a')) {
            abbr = ' ';
        }

        format = format.replace(new RegExp(abbr + 'a[kmbt]?'), '');

        if (abs >= trillion && !abbrForce || abbrForce === 't') {
            // trillion
            abbr += locale.abbreviations.trillion;
            value = value / trillion;
        } else if (abs < trillion && abs >= billion && !abbrForce || abbrForce === 'b') {
            // billion
            abbr += locale.abbreviations.billion;
            value = value / billion;
        } else if (abs < billion && abs >= million && !abbrForce || abbrForce === 'm') {
            // million
            abbr += locale.abbreviations.million;
            value = value / million;
        } else if (abs < million && abs >= thousand && !abbrForce || abbrForce === 'k') {
            // thousand
            abbr += locale.abbreviations.thousand;
            value = value / thousand;
        }
    }

    // check for optional decimals
    if (numeral._.includes(format, '[.]')) {
        optDec = true;
        format = format.replace('[.]', '.');
    }

    // break number and format
    int = value.toString().split('.')[0];
    precision = format.split('.')[1];
    thousands = format.indexOf(',');
    leadingCount = (format.split('.')[0].split(',')[0].match(/0/g) || []).length;

    if (precision) {
        if (numeral._.includes(precision, '[')) {
            precision = precision.replace(']', '');
            precision = precision.split('[');
            decimal = numeral._.toFixed(value, (precision[0].length + precision[1].length), roundingFunction, precision[1].length
);
        } else {
            decimal = numeral._.toFixed(value, precision.length, roundingFunction);
        }

        int = decimal.split('.')[0];

        if (numeral._.includes(decimal, '.')) {
            decimal = locale.delimiters.decimal + decimal.split('.')[1];
        } else {
            decimal = '';
        }

        if (optDec && Number(decimal.slice(1)) === 0) {
            decimal = '';
        }
    } else {
        int = numeral._.toFixed(value, 0, roundingFunction);
    }

    // check abbreviation again after rounding
    if (abbr && !abbrForce && Number(int) >= 1000 && abbr !== locale.abbreviations.trillion) {
        int = String(Number(int) / 1000);

        switch (abbr) {
            case locale.abbreviations.thousand:
                abbr = locale.abbreviations.million;
                break;
            case locale.abbreviations.million:
                abbr = locale.abbreviations.billion;
                break;
            case locale.abbreviations.billion:
                abbr = locale.abbreviations.trillion;
                break; ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral._.reduce"></a>[function <span class="apidocSignatureSpan">numeral._.</span>reduce (array, callback)](#apidoc.element.numeral._.reduce)
- description and source-code
```javascript
reduce = function (array, callback) {
    if (this === null) {
        throw new TypeError('Array.prototype.reduce called on null or undefined');
    }

    if (typeof callback !== 'function') {
        throw new TypeError(callback + ' is not a function');
    }

    var t = Object(array),
        len = t.length >>> 0,
        k = 0,
        value;

    if (arguments.length === 3) {
        value = arguments[2];
    } else {
        while (k < len && !(k in t)) {
            k++;
        }

        if (k >= len) {
            throw new TypeError('Reduce of empty array with no initial value');
        }

        value = t[k++];
    }
    for (; k < len; k++) {
        if (k in t) {
            value = callback(value, t[k], k, t);
        }
    }
    return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral._.stringToNumber"></a>[function <span class="apidocSignatureSpan">numeral._.</span>stringToNumber (string)](#apidoc.element.numeral._.stringToNumber)
- description and source-code
```javascript
stringToNumber = function (string) {
    var locale = locales[options.currentLocale],
        stringOriginal = string,
        abbreviations = {
            thousand: 3,
            million: 6,
            billion: 9,
            trillion: 12
        },
        abbreviation,
        value,
        i,
        regexp;

    if (options.zeroFormat && string === options.zeroFormat) {
        value = 0;
    } else if (options.nullFormat && string === options.nullFormat || !string.replace(/[^0-9]+/g, '').length) {
        value = null;
    } else {
        value = 1;

        if (locale.delimiters.decimal !== '.') {
            string = string.replace(/\./g, '').replace(locale.delimiters.decimal, '.');
        }

        for (abbreviation in abbreviations) {
            regexp = new RegExp('[^a-zA-Z]' + locale.abbreviations[abbreviation] + '(?:\\)|(\\' + locale.currency.symbol + ')?(?:\\))?)?$');

            if (stringOriginal.match(regexp)) {
                value *= Math.pow(10, abbreviations[abbreviation]);
                break;
            }
        }

        // check for negative number
        value *= (string.split('-').length + Math.min(string.split('(').length - 1, string.split(')').length - 1)) % 2 ? 1 : -1;

        // remove non numbers
        string = string.replace(/[^0-9\.]+/g, '');

        value *= Number(string);
    }

    return value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral._.toFixed"></a>[function <span class="apidocSignatureSpan">numeral._.</span>toFixed (value, maxDecimals, roundingFunction, optionals)](#apidoc.element.numeral._.toFixed)
- description and source-code
```javascript
toFixed = function (value, maxDecimals, roundingFunction, optionals) {
    var splitValue = value.toString().split('.'),
        minDecimals = maxDecimals - (optionals || 0),
        boundedPrecision,
        optionalsRegExp,
        power,
        output;

    // Use the smallest precision value possible to avoid errors from floating point representation
    if (splitValue.length === 2) {
      boundedPrecision = Math.min(Math.max(splitValue[1].length, minDecimals), maxDecimals);
    } else {
      boundedPrecision = minDecimals;
    }

    power = Math.pow(10, boundedPrecision);

    // Multiply up by precision, round accurately, then divide and use native toFixed():
    output = (roundingFunction(value + 'e+' + boundedPrecision) / power).toFixed(boundedPrecision);

    if (optionals > maxDecimals - boundedPrecision) {
        optionalsRegExp = new RegExp('\\.?0{1,' + (optionals - (maxDecimals - boundedPrecision)) + '}$');
        output = output.replace(optionalsRegExp, '');
    }

    return output;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.numeral.fn"></a>[module numeral.fn](#apidoc.module.numeral.fn)

#### <a name="apidoc.element.numeral.fn.add"></a>[function <span class="apidocSignatureSpan">numeral.fn.</span>add (value)](#apidoc.element.numeral.fn.add)
- description and source-code
```javascript
add = function (value) {
    var corrFactor = _.correctionFactor.call(null, this._value, value);

    function cback(accum, curr, currI, O) {
        return accum + Math.round(corrFactor * curr);
    }

    this._value = _.reduce([this._value, value], cback, 0) / corrFactor;

    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral.fn.clone"></a>[function <span class="apidocSignatureSpan">numeral.fn.</span>clone ()](#apidoc.element.numeral.fn.clone)
- description and source-code
```javascript
clone = function () {
    return numeral(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral.fn.difference"></a>[function <span class="apidocSignatureSpan">numeral.fn.</span>difference (value)](#apidoc.element.numeral.fn.difference)
- description and source-code
```javascript
difference = function (value) {
    return Math.abs(numeral(this._value).subtract(value).value());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral.fn.divide"></a>[function <span class="apidocSignatureSpan">numeral.fn.</span>divide (value)](#apidoc.element.numeral.fn.divide)
- description and source-code
```javascript
divide = function (value) {
    function cback(accum, curr, currI, O) {
        var corrFactor = _.correctionFactor(accum, curr);
        return Math.round(accum * corrFactor) / Math.round(curr * corrFactor);
    }

    this._value = _.reduce([this._value, value], cback);

    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral.fn.format"></a>[function <span class="apidocSignatureSpan">numeral.fn.</span>format (inputString, roundingFunction)](#apidoc.element.numeral.fn.format)
- description and source-code
```javascript
format = function (inputString, roundingFunction) {
    var value = this._value,
        format = inputString || options.defaultFormat,
        kind,
        output,
        formatFunction;

    // make sure we have a roundingFunction
    roundingFunction = roundingFunction || Math.round;

    // format based on value
    if (value === 0 && options.zeroFormat !== null) {
        output = options.zeroFormat;
    } else if (value === null && options.nullFormat !== null) {
        output = options.nullFormat;
    } else {
        for (kind in formats) {
            if (format.match(formats[kind].regexps.format)) {
                formatFunction = formats[kind].format;

                break;
            }
        }

        formatFunction = formatFunction || numeral._.numberToFormat;

        output = formatFunction(value, format, roundingFunction);
    }

    return output;
}
```
- example usage
```shell
...

### 1.5.1

Bug fix: Make sure values aren't changed during formatting

### 1.5.0

Add defaultFormat(). numeral().format() uses the default to format if no string is provided

.unformat() returns 0 when passed no string

Added languages.js that contains all languages

Bug fix: Fix bug while unformatting ordinals
...
```

#### <a name="apidoc.element.numeral.fn.input"></a>[function <span class="apidocSignatureSpan">numeral.fn.</span>input ()](#apidoc.element.numeral.fn.input)
- description and source-code
```javascript
input = function () {
    return this._input;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral.fn.multiply"></a>[function <span class="apidocSignatureSpan">numeral.fn.</span>multiply (value)](#apidoc.element.numeral.fn.multiply)
- description and source-code
```javascript
multiply = function (value) {
    function cback(accum, curr, currI, O) {
        var corrFactor = _.correctionFactor(accum, curr);
        return Math.round(accum * corrFactor) * Math.round(curr * corrFactor) / Math.round(corrFactor * corrFactor);
    }

    this._value = _.reduce([this._value, value], cback, 1);

    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral.fn.set"></a>[function <span class="apidocSignatureSpan">numeral.fn.</span>set (value)](#apidoc.element.numeral.fn.set)
- description and source-code
```javascript
set = function (value) {
    this._value = Number(value);

    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral.fn.subtract"></a>[function <span class="apidocSignatureSpan">numeral.fn.</span>subtract (value)](#apidoc.element.numeral.fn.subtract)
- description and source-code
```javascript
subtract = function (value) {
    var corrFactor = _.correctionFactor.call(null, this._value, value);

    function cback(accum, curr, currI, O) {
        return accum - Math.round(corrFactor * curr);
    }

    this._value = _.reduce([value], cback, Math.round(this._value * corrFactor)) / corrFactor;

    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.numeral.fn.value"></a>[function <span class="apidocSignatureSpan">numeral.fn.</span>value ()](#apidoc.element.numeral.fn.value)
- description and source-code
```javascript
value = function () {
    return this._value;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
