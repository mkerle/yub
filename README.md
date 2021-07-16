# YUB

[![NPM](https://nodei.co/npm/yub-proxy.png)](https://nodei.co/npm/yub-proxy/)

## Introduction

This project is based heavily on Yub by Glyn Bird [Yub](https://github.com/glynnbird/yub)

## Installation

yub-proxy is published as an NPM module:

```
  npm install yub-proxy
```

You'll also need a Yubico API Key from here: [https://upgrade.yubico.com/getapikey/]([https://upgrade.yubico.com/getapikey/). This gives you the
client_id and secret_key that must be passed to "yub.init()", see below.

## More information

Refer to original yub project here [Yub](https://github.com/glynnbird/yub)

## Example code

```
var yub = require('yub-proxy');

// initialise the yub library
yub.init("<client id here>", "<secret here>");

// attempt to verify the key
yub.verify("<otp here>", "<proxy server>", proxy_port, "<proxy username>", "<proxy password>", function(err,data) {
  console.log(err, data)
});
```



## References

* https://github.com/glynnbird/yub
* https://code.google.com/p/yubikey-val-server-php/wiki/GettingStartedWritingClients
* https://code.google.com/p/yubikey-val-server-php/wiki/ValidationProtocolV20

## Disclaimer

This software is open-source and is a personal project, not officially endorsed by Yubico in any way.

