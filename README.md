## TRON Message Board

This is a simple DApp demo built for TRON. It allows you to post messages,
tip messages and receive tips on your messages. It's powered by [TronWeb](https://github.com/tronprotocol/tron-web)
and integrated using [TronLink](https://github.com/TronWatch/TronLink).

Whilst you do not need TronLink installed to view the site, we recommend installing
it if you want to interact with any messages. You can [install TronLink from the Chrome Webstore](https://chrome.google.com/webstore/detail/ibnejdfjmmkpcnlpebklmnkoeoihofec/).

## Instructions :

1. [install TronLink](https://chrome.google.com/webstore/detail/ibnejdfjmmkpcnlpebklmnkoeoihofec/) chrome extension in browser and add some free coins to your wallet from any of the testnet faucets.
[Nile Testnet Faucet] (https://nileex.io/join/getJoinPage)
[Shasta Testnet Faucet 1] (https://www.trongrid.io/faucet)
[Shasta Testnet Faucet 2] (https://testnet.help/en/tronfaucet/testnet)

2. Clone this repo
```
$ git clone https://github.com/PorkyForky/TronLink-Demo-Messages
$ cd TronLink-Demo-Messages
```

3. Install TronBox and TronWeb
```
$ npm install -g tronbox
$ npm install -g tronweb
```

4. Install all required dependencies
```
$ npm install
```

5. Add your Private key to tronbox.js from shasta or nile test network account of TronLink.

6. Compile the smart contract
```
$ tronbox compile --compile-all
$ tronbox migrate --reset --network nile
```

7. Paste (base58) key of the SmartContract (The contracts wallet address) in Line 1 of src/utils/index.js

8. Start with yarn
```
$ yarn
$ yarn start
```

checkout the platform at http://localhost:3000/

------------------------