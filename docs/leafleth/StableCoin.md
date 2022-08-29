# StableCoin
> 
```
Stable coin manager
```


### 📋 Notice

This handles all stable coin operations related to the token




### 🎟 Events


#### AccessControlManagerSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| accessControlAddress | `true` | `address` |


#### CurrencyOracleAddressSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| currencyOracleAddress | `true` | `address` |


#### StableCoinAdded
| Name | Indexed | Type |
|:-:|:-:|:-:|
| symbol | `true` | `bytes32` |
| contractAddress | `true` | `address` |
| pipeAddress | `true` | `address` |


#### StableCoinDeleted
| Name | Indexed | Type |
|:-:|:-:|:-:|
| symbol | `true` | `bytes32` |



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



## `accruedPlatformFee`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint256` |



## `contractAddressOf`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `currencyOracleAddress`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `pipeAddressOf`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `platformFeeCurrency`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bytes32` |



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



## `addStableCoin`

>👀 `nonpayable`

### 📋 Notice

Adds a new stablecoin


### 🔎 Details

There can be no duplicate entries for same stablecoin symbol

### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _symbol | `bytes32` | Stablecoin symbol |



## `deleteStableCoin`

>👀 `nonpayable`

### 📋 Notice

Deletes an existing stablecoin



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _symbol | `bytes32` | Stablecoin symbol |



## `getStableCoinsAssociated`

>👀 `view`

### 📋 Notice

Getter for Stable coins associated



### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bytes32[]` |



## `balanceOf`

>👀 `view`

### 📋 Notice

Get balance of the stablecoins in the wallet address



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _symbol | `bytes32` | Stablecoin symbol |

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint256` |



## `decimals`

>👀 `view`

### 📋 Notice

Gets the decimals of the token



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokenSymbol | `bytes32` | Token symbol |

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint8` |



## `totalBalanceInFiat`

>👀 `view`

### 📋 Notice

Gets the total stablecoin balance associated with the MoToken



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _token | `address` | Token address |

### → Returns



| Name | Type |
|:-:|:-:|
|  balance  | `uint256` |



## `initiateTransferFrom`

>👀 `nonpayable`

### 📋 Notice

Transfers tokens from an external address to the MoToken Address



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _token | `address` | Token address |

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



## `transferFundsToPipe`

>👀 `nonpayable`

### 📋 Notice

Transfers tokens from the MoToken address to the stablecoin pipe address



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _token | `address` | Token address |

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



## `checkForSufficientBalance`

>👀 `view`

### 📋 Notice

Check for sufficient balance



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _symbol | `address` | Symbol of the token |



