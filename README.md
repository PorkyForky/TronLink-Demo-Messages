## TRON Message Board

This is a simple DApp demo built for TRON. It allows you to post messages,
tip messages and receive tips on your messages. It's powered by [TronWeb](https://github.com/tronprotocol/tron-web)
and integrated using [TronLink](https://github.com/TronWatch/TronLink).

Whilst you do not need TronLink installed to view the site, we recommend installing
it if you want to interact with any messages. You can [install TronLink from the Chrome Webstore](https://chrome.google.com/webstore/detail/ibnejdfjmmkpcnlpebklmnkoeoihofec/).

## Instructions :

Install TronLink chrome extension in browser.

```
$ npm install -g tronbox
$ npm install -g tronweb
$ npm install
```

Add your Private key to tronbox.js from shasta or nile test network account of TronLink.

```
$ tronbox compile --compile-all
$ tronbox migrate --reset --network nile
```

Paste (base58) key of SmartContract (The contracts wallet address) in Line 1 of src/utils/index.js

```
$ yarn
$ yarn start
```

checkout the platform at http://localhost:3000/

------------------------