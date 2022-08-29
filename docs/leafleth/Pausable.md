# Pausable
> 
```

```




### 🔎 Details

Contract module which allows children to implement an emergency stop mechanism that can be triggered by an authorized account. This module is used through inheritance. It will make available the modifiers `whenNotPaused` and `whenPaused`, which can be applied to the functions of your contract. Note that they will not be pausable by simply including this module, only once the modifiers are put in place.


### 🎟 Events


#### Paused
| Name | Indexed | Type |
|:-:|:-:|:-:|
| account | `false` | `address` |


#### Unpaused
| Name | Indexed | Type |
|:-:|:-:|:-:|
| account | `false` | `address` |



## `paused`

>👀 `view`



### 🔎 Details

Returns true if the contract is paused, and false otherwise.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



