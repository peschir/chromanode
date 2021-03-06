# chromanode

[![build status](https://img.shields.io/travis/chromaway/chromanode.svg?branch=master&style=flat-square)](http://travis-ci.org/chromaway/chromanode)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat-square)](https://github.com/feross/standard)

*Chromanode* is open source bitcoin blockchain API (http and websocket support) writeen on JavaScript and uses PostgreSQL for storage.

## Requirements

  * [Bitcoin](https://bitcoin.org/en/download) with txindex=1
  * [node.js](http://www.nodejs.org/download/) (testned with v0.12, v4.0?)
  * [PostgreSQL](http://www.postgresql.org/download/)

## Installation

  *Master* is under development, if you want use stable please checkout to one of the stable branches. (v1.0.0, v2.0, etc..)

  Clone repository:

    $ git clone https://github.com/chromaway/chromanode.git && cd chromanode

  Install dependencides:

    $ npm install

  Edit configs:

    $ vim config/master.yml config/slave.yml

  Run master node:

    $ ./bin/chromanode-master.js -c config/master.yml

  Run slave node (only one slave instance supported now):

    $ ./bin/chromanode-slave.js -c config/slave.yml

## API

  * [API v1](docs/API_v1.md)
  * [API v2](docs/API_v2.md) \**WIP*\*

To get latest version of supported API make request to `/version`

## Other open source blockchain apis

  * [bitcoin-abe](https://github.com/bitcoin-abe/bitcoin-abe)
  * [bitcore-node](https://github.com/bitpay/bitcore-node)
  * [electrum-server](https://github.com/spesmilo/electrum-server)
  * [insight-api](https://github.com/bitpay/insight-api)
  * [mychain](https://github.com/thofmann/mychain)
  * [toshi](https://github.com/coinbase/toshi)

## License

Code released under [the MIT license](https://github.com/chromaway/chromanode/blob/master/LICENSE).
