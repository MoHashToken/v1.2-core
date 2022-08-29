# MoTokenTrader
> 
```
Token Trade Listing Contract
```


### 📋 Notice

This contract handles P2P trade listing and purchase of tokens




### 🎟 Events


#### AccessControlManagerSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| accessControlAddress | `true` | `address` |


#### CancelledListing
| Name | Indexed | Type |
|:-:|:-:|:-:|
| sellerAddress | `true` | `address` |
| listingId | `true` | `uint256` |


#### CreatedListing
| Name | Indexed | Type |
|:-:|:-:|:-:|
| sellerAddress | `true` | `address` |
| tokenSymbol | `true` | `bytes32` |
| tokens | `true` | `uint256` |


#### CurrencyOracleAddressSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| currencyOracleAddress | `true` | `address` |


#### EditedListing
| Name | Indexed | Type |
|:-:|:-:|:-:|
| listingId | `true` | `uint256` |
| tokens | `true` | `uint256` |
| price | `true` | `int256` |


#### PurchasedFromListing
| Name | Indexed | Type |
|:-:|:-:|:-:|
| listingId | `true` | `uint256` |
| tokens | `true` | `uint256` |
| buyerAddress | `true` | `address` |



## `MO_DECIMALS`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint8` |



## `accessControlManagerAddress`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `allListings`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  seller  | `address` |
|  tokenSymbol  | `bytes32` |
|  listedTokens  | `uint256` |
|  listedTokensPending  | `uint256` |
|  listedPrice  | `int256` |



## `currencyOracleAddress`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `listingHead`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint256` |



## `listingTail`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint256` |



## `stableCoinAddress`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `tokenManagerFactoryAddress`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `totalTokensListedOf`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint256` |



## `setAccessControlManagerAddress`

>👀 `nonpayable`

### 📋 Notice

Setter for accessControlManagerAddress



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _accessControlManagerAddress | `address` | Set accessControlManagerAddress to this address |



## `setCurrencyOracleAddress`

>👀 `nonpayable`

### 📋 Notice

Allows setting currencyOracleAddress



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _currencyOracleAddress | `address` | address of the currency oracle |



## `createNewListing`

>👀 `nonpayable`

### 📋 Notice

Create a new listing



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokens | `bytes32` | The amount of tokens to redeem |



## `cancelListing`

>👀 `nonpayable`

### 📋 Notice

Cancel an existing listing



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _id | `uint256` | listing id |



## `editListing`

>👀 `nonpayable`

### 📋 Notice

Edit an existing listing



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokens | `uint256` | Update tokens in this listing |



## `purchaseFromListing`

>👀 `nonpayable`

### 📋 Notice

Purchase tokens from a given Listing



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _stableCoin | `uint256` | Token symbol of the stable coin used |



