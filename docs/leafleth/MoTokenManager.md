# MoTokenManager
> 
```
Token manager for open/senior token
```


### 📋 Notice

This is a token manager which handles all operations related to the token




### 🎟 Events


#### AccessControlManagerSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| accessControlAddress | `true` | `address` |


#### CurrencyOracleAddressSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| currencyOracleAddress | `true` | `address` |


#### FeeTransferred
| Name | Indexed | Type |
|:-:|:-:|:-:|
| fee | `true` | `uint256` |


#### FiatCredited
| Name | Indexed | Type |
|:-:|:-:|:-:|
| amount | `true` | `uint64` |
| date | `true` | `uint32` |


#### FiatCurrencySet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| currency | `true` | `bytes32` |


#### FiatDebited
| Name | Indexed | Type |
|:-:|:-:|:-:|
| amount | `true` | `uint64` |
| date | `true` | `uint32` |


#### NAVApprovalRequest
| Name | Indexed | Type |
|:-:|:-:|:-:|
| navUnapproved | `true` | `uint64` |
| stashUpdateDate | `true` | `uint32` |


#### NAVUpdated
| Name | Indexed | Type |
|:-:|:-:|:-:|
| nav | `true` | `uint64` |
| date | `true` | `uint32` |


#### PlatformFeeCurrencySet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| currency | `true` | `bytes32` |


#### PlatformFeeSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| platformFee | `true` | `uint32` |


#### Purchase
| Name | Indexed | Type |
|:-:|:-:|:-:|
| user | `true` | `address` |
| tokens | `true` | `uint256` |


#### RWADetailsSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| rwaAddress | `true` | `address` |


#### StableCoinAddressSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| stableCoinAddress | `true` | `address` |


#### TokenSupplyLimitSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| tokenSupplyLimit | `true` | `uint256` |



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



## `currencyOracleAddress`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `fiatCurrency`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bytes32` |



## `linkedSrRwaUnitId`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint256` |



## `platformFeeCurrency`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bytes32` |



## `rWADetails`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `stableCoinAddress`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `token`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `tokenData`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  id  | `uint16` |
|  navDeviationAllowance  | `uint16` |
|  daysInAYear  | `uint16` |
|  platformFee  | `uint32` |
|  navUpdateTimestamp  | `uint32` |
|  navApprovalRequestTimestamp  | `uint32` |
|  nav  | `uint64` |
|  navUnapproved  | `uint64` |
|  pipeFiatStash  | `uint64` |
|  fiatInTransit  | `uint64` |



## `tokenDecimals`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint256` |



## `tokenSupplyLimit`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint256` |



## `owner`

>👀 `view`

### 📋 Notice

returns the owner address



### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `initialize`

>👀 `nonpayable`

### 📋 Notice

Initializes basic properties associated with the token



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _token | `uint16` | token address |



## `setAccessControlManagerAddress`

>👀 `nonpayable`

### 📋 Notice

Setter for accessControlManagerAddress



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _accessControlManagerAddress | `address` | Set accessControlManagerAddress to this address |



## `setStableCoinAddress`

>👀 `nonpayable`

### 📋 Notice

Setter for stableCoin



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _stableCoinAddress | `address` | Set stableCoin to this address |



## `setRWADetailsAddress`

>👀 `nonpayable`

### 📋 Notice

Setter for RWADetails contract associated with the MoToken



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _rWADetails | `address` | Address of contract storing RWADetails |



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

Allows setting fiatCurrecy associated with tokens



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _fiatCurrency | `bytes32` | fiatCurrency |



## `setPlatformFeeCurrency`

>👀 `nonpayable`

### 📋 Notice

Setter for platform fee currency



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _feeCurrency | `bytes32` | platform fee currency |



## `setFee`

>👀 `nonpayable`

### 📋 Notice

Setter for platform fee



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _fee | `uint32` | platform fee |



## `setTokenSupplyLimit`

>👀 `nonpayable`

### 📋 Notice

Allows setting tokenSupplyLimit associated with tokens



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokenSupplyLimit | `uint256` | limit to be set for the token supply |



## `setNavDeviationAllowance`

>👀 `nonpayable`

### 📋 Notice

Allows setting NAV deviation allowance by Owner



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _value | `uint16` | Allowed deviation limit (Eg: 10 for 10% deviation) |



## `sweepFeeToGov`

>👀 `nonpayable`

### 📋 Notice

Raise request for platform fee transfer to governor



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| amount | `uint256` | fee transfer amount in fiat currency |



## `getId`

>👀 `view`

### 📋 Notice

Returns the token id for the associated token.



### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint16` |



## `setDaysInAYear`

>👀 `nonpayable`

### 📋 Notice

Sets days in a year to be used in fee calculation.





## `purchase`

>👀 `nonpayable`

### 📋 Notice

This function is called by the purchaser of MoH tokens. The protocol transfers _depositCurrency from the purchaser and mints and transfers MoH token to the purchaser


### 🔎 Details

tokenData.nav has the NAV (in USD) of the MoH token. The number of MoH tokens to mint = _depositAmount (in USD) / NAV

### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _depositCurrency | `uint256` | is the token that purchaser wants to pay with (eg: USDC, USDT etc) |



## `stableCoinToTokens`

>👀 `view`

### 📋 Notice

Converts stable coin amount to token amount



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _stableCoin | `uint256` | Stable coin symbol |

### → Returns



| Name | Type |
|:-:|:-:|
|  tokens  | `uint256` |



## `creditPipeFiat`

>👀 `nonpayable`

### 📋 Notice

The function allows RWA manger to provide the increase in pipe fiat balances against the MoH token



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _date | `uint64` | RWA manager is crediting pipe fiat for this date |



## `debitPipeFiat`

>👀 `nonpayable`

### 📋 Notice

The function allows RWA manger to decrease pipe fiat balances against the MoH token



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _date | `uint64` | RWA manager is debiting pipe fiat for this date |



## `getNAV`

>👀 `view`

### 📋 Notice

Provides the NAV of the MoH token



### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint64` |



## `updateNav`

>👀 `nonpayable`

### 📋 Notice

The function allows the RWA manager to update the NAV. NAV = (Asset value of AFI _ pipe fiat stash in Fiat + stablecoin balance) / Total supply of the MoH token.


### 🔎 Details

getTotalAssetValue gets value of all RWA units held by this MoH token plus stablecoin balances held by this MoH token. tokenData.pipeFiatStash gets the Fiat balances against this MoH token

### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _timestamp | `uint32` | Timestamp for which NAV is calculated |



## `approveNav`

>👀 `nonpayable`

### 📋 Notice

If the change in NAV is more than navDeviationAllowance, it has to be approved by Admin





## `setLinkedSrRwaUnitId`

>👀 `nonpayable`

### 📋 Notice

Sets the RWA unit ID corresponding to the junior RWA Unit ID



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _unitId | `uint256` | Senior RWA Unit ID |



## `updateFiatInTransit`

>👀 `nonpayable`

### 📋 Notice

Sets fiat in transit amount



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _fiatAmount | `uint64` | fiat amount (4 decimal shifted) |



