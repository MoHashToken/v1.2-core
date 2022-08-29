# RWADetails
> 
```
Real World Asset Details
```


### 📋 Notice

This contract stores the real world assets for the protocol




### 🎟 Events


#### AccessControlManagerSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| accessControlAddress | `true` | `address` |


#### AutoCalcFlagUpdated
| Name | Indexed | Type |
|:-:|:-:|:-:|
| rWAUnitId | `true` | `uint256` |
| autoCalcFlag | `true` | `bool` |


#### CurrencyOracleAddressSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| currencyOracleAddress | `true` | `address` |


#### RWAUnitAddedUnitsForTokenId
| Name | Indexed | Type |
|:-:|:-:|:-:|
| rWAUnitId | `true` | `uint256` |
| tokenId | `true` | `uint16` |
| units | `false` | `uint64` |


#### RWAUnitCreated
| Name | Indexed | Type |
|:-:|:-:|:-:|
| rWAUnitId | `true` | `uint256` |


#### RWAUnitDetailsUpdated
| Name | Indexed | Type |
|:-:|:-:|:-:|
| rWAUnitId | `true` | `uint256` |
| unitPrice | `true` | `uint128` |
| priceUpdateDate | `true` | `uint32` |
| portfolioDetailsLink | `false` | `string` |


#### RWAUnitPayoutUpdated
| Name | Indexed | Type |
|:-:|:-:|:-:|
| rWAUnitId | `true` | `uint256` |
| payoutAmount | `true` | `uint128` |
| unitPrice | `true` | `uint128` |


#### RWAUnitRedeemedUnitsForTokenId
| Name | Indexed | Type |
|:-:|:-:|:-:|
| rWAUnitId | `true` | `uint256` |
| tokenId | `true` | `uint16` |
| units | `false` | `uint64` |


#### RWAUnitSchemeDocumentLinkUpdated
| Name | Indexed | Type |
|:-:|:-:|:-:|
| rWAUnitId | `true` | `uint256` |
| schemeDocumentLink | `false` | `string` |


#### RWAUnitValueUpdated
| Name | Indexed | Type |
|:-:|:-:|:-:|
| rWAUnitId | `true` | `uint256` |
| priceUpdateDate | `true` | `uint32` |
| unitPrice | `true` | `uint128` |


#### SeniorDefaultUpdated
| Name | Indexed | Type |
|:-:|:-:|:-:|
| rWAUnitId | `true` | `uint256` |
| defaultFlag | `true` | `bool` |



## `MO_DECIMALS`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint128` |



## `RWA_DECIMALS`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint256` |



## `accessControlManagerAddress`

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



## `leapYear`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



## `rWAUnitDetails`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  name  | `string` |
|  schemeDocumentLink  | `string` |
|  portfolioDetailsLink  | `string` |



## `rWAUnitId`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint256` |



## `rWAUnits`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  autoCalcFlag  | `bool` |
|  defaultFlag  | `bool` |
|  tokenId  | `uint16` |
|  startDate  | `uint32` |
|  endDate  | `uint32` |
|  priceUpdateDate  | `uint32` |
|  apy  | `uint64` |
|  apyLeapYear  | `uint64` |
|  units  | `uint64` |
|  notionalValue  | `uint128` |
|  unitPrice  | `uint128` |
|  fiatCurrency  | `bytes32` |



## `tokenIdToRWAUnitId`

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



## `setLeapYear`

>👀 `nonpayable`

### 📋 Notice

Setter for leapYear



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _leapYear | `bool` | whether current period is in a leap year |



## `createRWAUnit`

>👀 `nonpayable`



### 🔎 Details

Explain to a developer any extra details

### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _units | `string` | number of units. |



## `addRWAUnits`

>👀 `nonpayable`




### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _units | `uint256` | contains the number of RWA units added to the MoH token |



## `redeemRWAUnits`

>👀 `nonpayable`




### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _units | `uint256` | contains the number of RWA units redeemed from the MoH token |



## `updateRWAUnitSchemeDocumentLink`

>👀 `nonpayable`



### 🔎 Details

Function emits RWAUnitSchemeDocumentLinkUpdated event which provides id of RWA scheme update and the updated scheme document link

### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _schemeDocumentLink | `uint256` | stores the link to the RWA scheme document |



## `updateRWAUnitDetails`

>👀 `nonpayable`



### 🔎 Details

Function emits RWAUnitDetailsUpdated event which provides id of RWA updated, unit price updated and price update date

### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _unitPrice | `uint256` | stores the price of a single RWA unit |



## `setCurrencyOracleAddress`

>👀 `nonpayable`

### 📋 Notice

Allows setting currencyOracleAddress



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _currencyOracleAddress | `address` | address of the currency oracle |



## `setSeniorDefault`

>👀 `nonpayable`



### 🔎 Details

Function emits SeniorDefaultUpdated event which provides value of defaultFlag for the unit id.

### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _id | `uint256` | Refers to id of the RWA being updated |



## `updateAutoCalc`

>👀 `nonpayable`



### 🔎 Details

Function emits AutoCalcFlagUpdated event which provides id of RWA updated and autoCalcFlag value set.

### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _unitPrice | `uint256` | Refers to unitPrice of the RWA being updated |



## `isRedemptionAllowed`

>👀 `view`




### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _id | `uint256` | Refers to id of the RWA unit |

### → Returns



| Name | Type |
|:-:|:-:|
|  redemptionAllowed  | `bool` |



## `updateRWAUnitValue`

>👀 `nonpayable`




### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _id | `uint16` | Refers to id of the RWA unit |



## `udpatePayout`

>👀 `nonpayable`




### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _payoutAmount | `uint16` | payout amount to be subtracted from the unit price. |



## `getRWAValueByTokenId`

>👀 `view`



### 🔎 Details

Explain to a developer any extra details

### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokenId | `uint16` | is the MoH token Id for which value of RWA units is being calculated |

### → Returns



| Name | Type |
|:-:|:-:|
|  assetValue  | `uint128` |



## `getRWAUnitsForTokenId`

>👀 `view`




### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokenId | `uint256` | Refers to token id |

### → Returns



| Name | Type |
|:-:|:-:|
|  rWAUnitsByTokenId  | `uint256[]` |



