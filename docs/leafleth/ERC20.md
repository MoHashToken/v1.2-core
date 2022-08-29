# ERC20
> 
```

```




### 🔎 Details

Implementation of the {IERC20} interface. This implementation is agnostic to the way tokens are created. This means that a supply mechanism has to be added in a derived contract using {_mint}. For a generic mechanism see {ERC20PresetMinterPauser}. TIP: For a detailed writeup see our guide https://forum.zeppelin.solutions/t/how-to-implement-erc20-supply-mechanisms/226[How to implement supply mechanisms]. We have followed general OpenZeppelin Contracts guidelines: functions revert instead returning `false` on failure. This behavior is nonetheless conventional and does not conflict with the expectations of ERC20 applications. Additionally, an {Approval} event is emitted on calls to {transferFrom}. This allows applications to reconstruct the allowance for all accounts just by listening to said events. Other implementations of the EIP may not emit these events, as it isn&#39;t required by the specification. Finally, the non-standard {decreaseAllowance} and {increaseAllowance} functions have been added to mitigate the well-known issues around setting allowances. See {IERC20-approve}.


### 🎟 Events


#### Approval
| Name | Indexed | Type |
|:-:|:-:|:-:|
| owner | `true` | `address` |
| spender | `true` | `address` |
| value | `false` | `uint256` |


#### Transfer
| Name | Indexed | Type |
|:-:|:-:|:-:|
| from | `true` | `address` |
| to | `true` | `address` |
| value | `false` | `uint256` |



## `name`

>👀 `view`



### 🔎 Details

Returns the name of the token.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `string` |



## `symbol`

>👀 `view`



### 🔎 Details

Returns the symbol of the token, usually a shorter version of the name.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `string` |



## `decimals`

>👀 `view`



### 🔎 Details

Returns the number of decimals used to get its user representation. For example, if `decimals` equals `2`, a balance of `505` tokens should be displayed to a user as `5.05` (`505 / 10 ** 2`). Tokens usually opt for a value of 18, imitating the relationship between Ether and Wei. This is the value {ERC20} uses, unless this function is overridden; NOTE: This information is only used for _display_ purposes: it in no way affects any of the arithmetic of the contract, including {IERC20-balanceOf} and {IERC20-transfer}.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint8` |



## `totalSupply`

>👀 `view`



### 🔎 Details

See {IERC20-totalSupply}.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint256` |



## `balanceOf`

>👀 `view`



### 🔎 Details

See {IERC20-balanceOf}.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint256` |



## `transfer`

>👀 `nonpayable`



### 🔎 Details

See {IERC20-transfer}. Requirements: - `to` cannot be the zero address. - the caller must have a balance of at least `amount`.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



## `allowance`

>👀 `view`



### 🔎 Details

See {IERC20-allowance}.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint256` |



## `approve`

>👀 `nonpayable`



### 🔎 Details

See {IERC20-approve}. NOTE: If `amount` is the maximum `uint256`, the allowance is not updated on `transferFrom`. This is semantically equivalent to an infinite approval. Requirements: - `spender` cannot be the zero address.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



## `transferFrom`

>👀 `nonpayable`



### 🔎 Details

See {IERC20-transferFrom}. Emits an {Approval} event indicating the updated allowance. This is not required by the EIP. See the note at the beginning of {ERC20}. NOTE: Does not update the allowance if the current allowance is the maximum `uint256`. Requirements: - `from` and `to` cannot be the zero address. - `from` must have a balance of at least `amount`. - the caller must have allowance for ``from``&#39;s tokens of at least `amount`.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



## `increaseAllowance`

>👀 `nonpayable`



### 🔎 Details

Atomically increases the allowance granted to `spender` by the caller. This is an alternative to {approve} that can be used as a mitigation for problems described in {IERC20-approve}. Emits an {Approval} event indicating the updated allowance. Requirements: - `spender` cannot be the zero address.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



## `decreaseAllowance`

>👀 `nonpayable`



### 🔎 Details

Atomically decreases the allowance granted to `spender` by the caller. This is an alternative to {approve} that can be used as a mitigation for problems described in {IERC20-approve}. Emits an {Approval} event indicating the updated allowance. Requirements: - `spender` cannot be the zero address. - `spender` must have allowance for the caller of at least `subtractedValue`.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



