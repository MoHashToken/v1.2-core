# RedemptionBatchProcessor
> 
```
Token Redemption Batch Processor
```


### 📋 Notice

This contract handles the token redemption process




### 🎟 Events


#### AccessControlManagerSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| accessControlAddress | `true` | `address` |


#### BatchCreated
| Name | Indexed | Type |
|:-:|:-:|:-:|
| id | `true` | `uint256` |
| creator | `true` | `address` |


#### BatchFulfilled
| Name | Indexed | Type |
|:-:|:-:|:-:|
| id | `true` | `uint256` |
| tokens | `true` | `uint256` |
| closed | `true` | `bool` |


#### CurrencyOracleAddressSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| currencyOracleAddress | `true` | `address` |


#### FiatCurrencySet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| currency | `true` | `bytes32` |


#### RedeemRequestCancelled
| Name | Indexed | Type |
|:-:|:-:|:-:|
| user | `true` | `address` |
| batchId | `true` | `uint256` |


#### RedeemRequestCreated
| Name | Indexed | Type |
|:-:|:-:|:-:|
| user | `true` | `address` |
| tokens | `true` | `uint256` |


#### RefundCoinSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| coin | `true` | `bytes32` |



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



## `assignedRefundCoin`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bytes32` |



## `batchHead`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint256` |



## `batchTail`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint256` |



## `currencyOracleAddress`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `decimalsDiff`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `int8` |



## `fiatCurrency`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bytes32` |



## `stableCoinAddress`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `tokenManagerAddress`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `setAccessControlManagerAddress`

>👀 `nonpayable`

### 📋 Notice

Setter for accessControlManagerAddress



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _accessControlManagerAddress | `address` | Set accessControlManagerAddress to this address |



## `setAssignedRefundCoin`

>👀 `nonpayable`

### 📋 Notice

Setter for assigned refund coin



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _coin | `bytes32` | Refund coin symbol |



## `setCurrencyOracleAddress`

>👀 `nonpayable`

### 📋 Notice

Allows setting currencyOracleAddress



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _currencyOracleAddress | `address` | address of the currency oracle |



## `setFiatCurrency`

>👀 `nonpayable`

### 📋 Notice

Allows setting fiatCurrecy



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _fiatCurrency | `bytes32` | fiatCureency |



## `createBatch`

>👀 `nonpayable`

### 📋 Notice

Creates a new batch





## `createRedeemRequest`

>👀 `nonpayable`

### 📋 Notice

Create a new redeem request in the current batch



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokens | `uint256` | The amount of tokens to redeem |



## `cancelRedeemRequest`

>👀 `nonpayable`

### 📋 Notice

Cancel an existing redeem in the given batch



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _id | `uint256` | Batch id where the redeem request is to be cancelled |



## `fulfillBatch`

>👀 `nonpayable`

### 📋 Notice

Fulfill the redeem requests in the given batch



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _id | `uint256` | Batch Id |



## `getBatchUsers`

>👀 `view`

### 📋 Notice

Getter for all the users who have raised redemption request



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _id | `uint256` | Batch Id |

### → Returns



| Name | Type |
|:-:|:-:|
|  userList  | `address[]` |



## `getBatchRequestDetails`

>👀 `view`

### 📋 Notice

Getter for Request details



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _user | `uint256` | Address of user who has raised the redemption request |

### → Returns



| Name | Type |
|:-:|:-:|
|  request  | `uint256` |
|  pending  | `uint256` |



## `getBatchTokensPending`

>👀 `view`

### 📋 Notice

Getter for tokens pending redemption in the whole batch



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _id | `uint256` | Batch Id |

### → Returns



| Name | Type |
|:-:|:-:|
|  tokens  | `uint256` |



## `getLockedTokens`

>👀 `view`

### 📋 Notice

User can call this function to get total amount of tokens locked for redemption



### → Returns



| Name | Type |
|:-:|:-:|
|  _tokens  | `uint256` |



