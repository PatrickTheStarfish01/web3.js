# web3-core-method

[![NPM Package][npm-image]][npm-url] 

This is a sub-package of [web3.js][repo].

This method package is used within most [web3.js][repo] packages.

Please read the [documentation][docs] for more.

## Installation

### Node.js

```bash
npm install web3-core-method
```

## Usage

```js
const Web3Method = require('web3-core-method');

const method = new Web3Method({
    name: 'sendTransaction',
    call: 'eth_sendTransaction',
    params: 1,
    inputFormatter: [inputTransactionFormatter]
});
method.attachToObject(myCoolLib);

myCoolLib.sendTransaction({...}, function(){ ... });
```

## Types

All the TypeScript typings are placed in the `types` folder.

[docs]: http://web3js.readthedocs.io/en/1.0/
[repo]: https://github.com/ethereum/web3.js
[npm-image]: https://img.shields.io/npm/v/web3-core-method.svg
[npm-url]: https://npmjs.org/package/web3-core-method

