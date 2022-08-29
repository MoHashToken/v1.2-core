# CurrencyOracle
> 
```
CurrencyOracle
```


### 📋 Notice

This handles all the operations related currency exchange




### 🎟 Events


#### OwnershipTransferred
| Name | Indexed | Type |
|:-:|:-:|:-:|
| previousOwner | `true` | `address` |
| newOwner | `true` | `address` |


#### feedAddressSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| feedAddress | `true` | `address` |
| fromCurrency | `true` | `bytes32` |
| toCurrency | `true` | `bytes32` |



## `dataFeedAddressMapper`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `owner`

>👀 `view`



### 🔎 Details

Returns the address of the current owner.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `renounceOwnership`

>👀 `nonpayable`



### 🔎 Details

Leaves the contract without owner. It will not be possible to call `onlyOwner` functions anymore. Can only be called by the current owner. NOTE: Renouncing ownership will leave the contract without an owner, thereby removing any functionality that is only available to the owner.



## `transferOwnership`

>👀 `nonpayable`



### 🔎 Details

Transfers ownership of the contract to a new account (`newOwner`). Can only be called by the current owner.



## `setOracleFeedAddress`

>👀 `nonpayable`

### 📋 Notice

Allows adding mapping b/w encoded bytes32 of currecies and chainLink Date Feed proxy Address



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _toCurrency | `bytes32` | _toCurrency |



## `getFeedLatestPriceAndDecimals`

>👀 `view`

### 📋 Notice

to get latest price and decimals



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _toCurrency | `bytes32` | _toCurrency |

### → Returns



| Name | Type |
|:-:|:-:|
|  lastestPrice  | `uint64` |
|  decimals  | `uint8` |



