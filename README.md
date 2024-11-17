# Kite Publisher

A lightweight NPM package for integrating Kite Connect Publisher functionalities.

## Installation

```bash
npm install kite-publisher
```

```bash
const KitePublisher = require('kite-publisher');

const publisher = new KitePublisher("your_api_key");

publisher.initialize().then(() => {
publisher.addStockToBasket({
exchange: "NSE",
tradingsymbol: "INFY",
quantity: 1,
transaction_type: "BUY",
order_type: "MARKET",
});

    publisher.renderButton('#buy-button');

});
```
