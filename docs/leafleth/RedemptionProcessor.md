# RedemptionProcessor
> 
```

```






### 🎟 Events


#### AccessControlManagerSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| accessControlAddress | `true` | `address` |


#### CurrencyOracleAddressSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| currencyOracle | `true` | `address` |


#### RedeemRequestCancelled
| Name | Indexed | Type |
|:-:|:-:|:-:|
| requestor | `false` | `address` |
| tokenSymbol | `false` | `bytes32` |
| index | `false` | `uint256` |


#### RedeemRequestCreated
| Name | Indexed | Type |
|:-:|:-:|:-:|
| requestor | `false` | `address` |
| tokenSymbol | `false` | `bytes32` |
| requestTokens | `false` | `uint256` |


#### RedeemRequestFulfilled
| Name | Indexed | Type |
|:-:|:-:|:-:|
| requestor | `false` | `address` |
| tokenSymbol | `false` | `bytes32` |
| requestTokens | `false` | `uint256` |


#### RedeemRequestModified
| Name | Indexed | Type |
|:-:|:-:|:-:|
| requestor | `false` | `address` |
| tokenSymbol | `false` | `bytes32` |
| newRequestTokens | `false` | `uint256` |


#### RefundCoinSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| coin | `true` | `bytes32` |


#### TokenRequestCreated
| Name | Indexed | Type |
|:-:|:-:|:-:|
| tokenIndex | `false` | `uint16` |
| tokenSymbol | `false` | `bytes32` |



## `MO_DECIMALS`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint8` |



## `accessControlManager`

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



## `currencyOracle`

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



## `stableCoin`

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



## `tokenSymbolToId`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint16` |



## `setAccessControlManager`

>👀 `nonpayable`

### 📋 Notice

Setter for setAccessControlManager



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _accessControlManager | `address` | Set accessControlManagerAddress to this address |



## `setTokenManagerFactoryAddress`

>👀 `nonpayable`

### 📋 Notice

Setter for setTokenManagerFactoryAddress



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokenManagerFactoryAddress | `address` | Set tokenManagerFactoryAddress to this address |



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
| _currencyOracle | `address` | address of the currency oracle |



## `createRequestToTokenMapping`

>👀 `nonpayable`

### 📋 Notice

creates request details for a token and stores it in allTokenRequestsDetails array &amp; stores the token symbol and its index in tokenSymbolToId mapping



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokenSymbol | `bytes32` | Symbol of the token for which request details are to be created |



## `createRedeemRequest`

>👀 `nonpayable`

### 📋 Notice

Creates a request for a token for a user for a given amount of tokens &amp; stores the request details in allTokenRequestsDetails array



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokenSymbol | `bytes32` | Symbol of the token for which request details are to be created |



## `modifyRedeemRequest`

>👀 `nonpayable`

### 📋 Notice

Modifies a request for a token for a user for a given amount of tokens &amp; updates the request details in allTokenRequestsDetails array



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| index | `bytes32` | Index of the request to be modified |



## `fulfill`

>👀 `nonpayable`

### 📋 Notice

fulfill a request for a token symbol for a user for a given amount of stable coin &amp; updates the request details in allTokenRequestsDetails array



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokenSymbol | `bytes32` | Symbol of the token for which request details are to be fulfilled |



## `getTotalRequest`

>👀 `view`

### 📋 Notice

Gets the total request count for a token symbol



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokenSymbol | `bytes32` | Symbol of the token for which request count is to be retrieved |

### → Returns



| Name | Type |
|:-:|:-:|
|  totalRequest  | `uint256` |



## `getRequestDetailsById`

>👀 `view`

### 📋 Notice

Gets the request details for a token symbol by index



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokenSymbol | `bytes32` | Symbol of the token for which request details are to be retrieved |

### → Returns



| Name | Type |
|:-:|:-:|
|  requestTokens  | `uint256` |
|  requestTokensPending  | `uint256` |
|  requestor  | `address` |



## `getRequestDetailsByIdAndRequestor`

>👀 `view`

### 📋 Notice

Gets the request details for a token symbol by index and requestor



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| requestor | `bytes32` | Address of the requestor |

### → Returns



| Name | Type |
|:-:|:-:|
|  id  | `uint256` |
|  requestTokens  | `uint256` |
|  requestTokensPending  | `uint256` |



## `getRedemptionRequestDetailsByAddress`

>👀 `view`

### 📋 Notice

Gets the request details for a token symbol by user address



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokenSymbol | `bytes32` | Symbol of the token for which request details are to be retrieved |

### → Returns



| Name | Type |
|:-:|:-:|
|  length  | `uint256` |



