# Utility for ordering pair of assets in (amount_asset, price_asset)

[![Build Status](https://dev.azure.com/BlackTurtleBVBA/TurtleNetwork_OpenSource/_apis/build/status/TurtleNetwork.assets-pairs-order?branchName=master)](https://dev.azure.com/BlackTurtleBVBA/TurtleNetwork_OpenSource/_build/latest?definitionId=14&branchName=master)

## Example:

```
yarn add @waves/assets-pairs-order
```

```javascript
import { createOrderPair, MAINNET_DATA } from '@waves/assets-pairs-order'

const orderPair = createOrderPair(MAINNET_DATA);
orderPair(
  'DNhP2zAH5HM1kdUSmxcBqs8RP4vvUgRFc1YgAKkfPmPD',
  'FxSm86qcEw8wGfpX3T7X5fsnuK5XxYA6ZfVYJja29vMA'
)

/* [
    'FxSm86qcEw8wGfpX3T7X5fsnuK5XxYA6ZfVYJja29vMA',
    'DNhP2zAH5HM1kdUSmxcBqs8RP4vvUgRFc1YgAKkfPmPD',
  ]
*/

## Browser

For using in browser include dist/browser.js
```
