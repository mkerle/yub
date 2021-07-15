# YUB

[![NPM](https://nodei.co/npm/yub.png)](https://nodei.co/npm/yub-proxy/)

## Introduction

This project is based heavily on Yub by Glyn Bird [Yub](https://github.com/glynnbird/yub)

## Installation

Yub is published as an NPM module for your convenience:

```
  npm install yub
```

You'll also need a Yubico API Key from here: [https://upgrade.yubico.com/getapikey/]([https://upgrade.yubico.com/getapikey/). This gives you the
client_id and secret_key that must be passed to "yub.init()", see below.

## Example code

```
var yub = require('yub');

// initialise the yub library
yub.init("<client id here>", "<secret here>");

// attempt to verify the key
yub.verify("<otp here>", function(err,data) {
  console.log(err, data)
});
```



## References

* https://code.google.com/p/yubikey-val-server-php/wiki/GettingStartedWritingClients
* https://code.google.com/p/yubikey-val-server-php/wiki/ValidationProtocolV20

## Disclaimer

This software is open-source and is a personal project, not officially endorsed by Yubico in any way.

