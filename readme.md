# Update

Updated in order to allow you to also keep commas with the spaces, as well as comma with spaces and period.

# String Sanitizer

An intuitive & tiny string sanitizer to remove any special characters or convert strings to create filename or url 🎉🎉

# Use Case

Converting or sanitizing string is easier than ever with the help of this package. You can use this utility package to sanitize even foreign languages other than English. Under the hood, regex is heavily used in this library. You can convert your string to url or filename frindly string.
🎉🎉

## Installation

You can download this package from here - [string-sanitizer npm](https://www.npmjs.com/package/string-sanitizer)

```bash
npm i string-sanitizer
```

Yarn installation

```bash
yarn add string-sanitizer
```

## Usage 👀👀👀

Just pass your string as the argument. The method will return a sanitized or converted string instantly.

```js
var string = require("string-sanitizer");
let someString = "@abcde$f$gh";
string.sanitize(someString); // abcdefgh
```

# Other Use Cases

```js
var string = require("string-sanitizer");

string.sanitize("a.bc@d efg#h"); // abcdefgh
string.sanitize.keepSpace("a.bc@d efg#h"); // abcd efgh
string.sanitize.keepSpaceAndComma("a,bc@d efg#h"); // a,bcd efgh
string.sanitize.keepSpaceCommaAndPeriod("a,b.c@d efg#h"); // a,b.cd efgh
string.sanitize.keepUnicode("a.bc@d efg#hক"); // abcd efghক
string.sanitize.addFullstop("a.bc@d efg#h"); // abcd.efgh
string.sanitize.addUnderscore("a.bc@d efg#h"); // abcd_efgh
string.sanitize.addDash("a.bc@d efg#h"); // abcd-efgh
string.sanitize.removeNumber("@abcd efgh123"); // abcdefgh
string.sanitize.keepNumber("@abcd efgh123"); // abcdefgh123
string.addFullstop("abcd efgh"); // abcd.efgh
string.addUnderscore("@abcd efgh"); // @abcd_efgh
string.addDash("@abcd efgh"); // @abcd-efgh
string.removeSpace("@abcd efgh"); // @abcdefgh
```

## Show Me the Code

![string-sanitizer](https://i.ibb.co/y44bXBb/Screenshot-275.png)

## Typescript compatitibility

Thanks to @kewitz

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate. 🏃‍🏃‍

## License

[MIT](https://github.com/fazlulkarimweb/string-sanitizer/blob/master/license)
