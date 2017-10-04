Btc BIP39 Mnemonics
=======

[![Greenkeeper badge](https://badges.greenkeeper.io/owstack/btc-mnemonic.svg)](https://greenkeeper.io/)

[![NPM Package](https://img.shields.io/npm/v/btc-mnemonic.svg?style=flat-square)](https://www.npmjs.org/package/btc-mnemonic)
[![Build Status](https://img.shields.io/travis/owstack/btc-mnemonic.svg?branch=master&style=flat-square)](https://travis-ci.org/owstack/btc-mnemonic)
[![Coverage Status](https://img.shields.io/coveralls/owstack/btc-mnemonic.svg?style=flat-square)](https://coveralls.io/r/owstack/btc-mnemonic)

A module for [btc](https://github.com/owstack/btc) that implements [Mnemonic code for generating deterministic keys](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki).

## Attribution

This repository was created by copy forking [bitcore-mnemonic commit 532fbe1](https://github.com/bitpay/bitcore-mnemonic/commit/532fbe1010502fee3f25bdd93cb8dde66fb1386e).

## Getting Started

This library is distributed in both the npm and bower packaging systems.

```sh
npm install btc-mnemonic
bower install btc-mnemonic
```

There are many examples of how to use it on the developer guide [section for mnemonic](http://btc.io/guide/module/mnemonic/index.html). For example, the following code would generate a new random mnemonic code and convert it to a `HDPrivateKey`.

```javascript
var Mnemonic = require('btc-mnemonic');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString(); // natal hada sutil año sólido papel jamón combate aula flota ver esfera...
var xpriv = code.toHDPrivateKey();
```

## Contributing

See [CONTRIBUTING.md](https://github.com/owstack/btc/blob/master/CONTRIBUTING.md) on the main btc repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/owstack/btc/blob/master/LICENSE).

Copyright 2017 Open Wallet Stack.
