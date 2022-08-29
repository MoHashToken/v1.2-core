# MoTokenManagerFactory
> 
```

```


### 📋 Notice

This contract creates MoTokenManager for a given MoToken.  This also gives us a way to get MoTokenManager give a token symbol.




### 🎟 Events


#### JrTokenLinkedToSrToken
| Name | Indexed | Type |
|:-:|:-:|:-:|
| jrToken | `true` | `bytes32` |
| srToken | `true` | `bytes32` |


#### MoTokenManagerAdded
| Name | Indexed | Type |
|:-:|:-:|:-:|
| from | `true` | `address` |
| tokenSymbol | `true` | `bytes32` |
| tokenManager | `true` | `address` |


#### OwnershipTransferred
| Name | Indexed | Type |
|:-:|:-:|:-:|
| previousOwner | `true` | `address` |
| newOwner | `true` | `address` |



## `linkedSrTokenOf`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bytes32` |



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



## `symbolToTokenManager`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `symbols`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bytes32` |



## `tokenId`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint16` |



## `transferOwnership`

>👀 `nonpayable`



### 🔎 Details

Transfers ownership of the contract to a new account (`newOwner`). Can only be called by the current owner.



## `addTokenManager`

>👀 `nonpayable`

### 📋 Notice

Adds MoTokenManager for a given MoToken



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokenManager | `address` | Address of MoTokenManager contract |



## `linkJrTokenToSrToken`

>👀 `nonpayable`

### 📋 Notice

Links a Junior token to Senior token.



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _srToken | `bytes32` | Symbol of Senior MoToken |



