## number-to-bn

<div>
  <!-- NPM Version -->
  <a href="https://www.npmjs.org/package/@metamask/number-to-bn">
    <img src="http://img.shields.io/npm/v/@metamask/number-to-bn.svg"
    alt="NPM version" />
  </a>
</div>

<br />

A simple method to convert integer or hex integer numbers to BN.js object instances. Does not support decimal numbers.

## Install

```
npm install --save @metamask/number-to-bn
```

## Usage

```js
const numberToBN = require('@metamask/number-to-bn');

console.log(numberToBN('-1'));

// result <BN ...> -1

console.log(numberToBN(1));

// result <BN ...> 1

console.log(numberToBN(new BN(100)));

// result <BN ...> 100

console.log(numberToBN(new BigNumber(10000)));

// result <BN ...> 10000

console.log(numberToBN('0x0a'));

// result <BN ...> 10

console.log(numberToBN('-0x0a'));

// result <BN ...> -10

console.log(numberToBN('0.9')); // or {}, [], undefined, 9.9

// throws new Error(...)

console.log(numberToBN(null)); // or {}, [], undefined, 9.9

// throws new Error(...)
```

## Important documents

- [Changelog](CHANGELOG.md)
- [License](https://raw.githubusercontent.com/MetaMask/number-to-bn/main/LICENSE)

## Licence

This project is licensed under the MIT license, Copyright (c) 2016 Nick Dodson. For more information see LICENSE.md.

```
The MIT License

Copyright (c) 2016 Nick Dodson. nickdodson.com

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```
