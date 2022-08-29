# USDC
> 
```

```






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



## `balanceOf`

>👀 `view`



### 🔎 Details

See {IERC20-balanceOf}.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint256` |



## `burn`

>👀 `nonpayable`



### 🔎 Details

Destroys `amount` tokens from the caller. See {ERC20-_burn}.



## `burnFrom`

>👀 `nonpayable`



### 🔎 Details

Destroys `amount` tokens from `account`, deducting from the caller&#39;s allowance. See {ERC20-_burn} and {ERC20-allowance}. Requirements: - the caller must have allowance for ``accounts``&#39;s tokens of at least `amount`.



## `decreaseAllowance`

>👀 `nonpayable`



### 🔎 Details

Atomically decreases the allowance granted to `spender` by the caller. This is an alternative to {approve} that can be used as a mitigation for problems described in {IERC20-approve}. Emits an {Approval} event indicating the updated allowance. Requirements: - `spender` cannot be the zero address. - `spender` must have allowance for the caller of at least `subtractedValue`.

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



## `totalSupply`

>👀 `view`



### 🔎 Details

See {IERC20-totalSupply}.

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



## `transferFrom`

>👀 `nonpayable`



### 🔎 Details

See {IERC20-transferFrom}. Emits an {Approval} event indicating the updated allowance. This is not required by the EIP. See the note at the beginning of {ERC20}. NOTE: Does not update the allowance if the current allowance is the maximum `uint256`. Requirements: - `from` and `to` cannot be the zero address. - `from` must have a balance of at least `amount`. - the caller must have allowance for ``from``&#39;s tokens of at least `amount`.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



## `decimals`

>👀 `pure`



### 🔎 Details

Returns the number of decimals used to get its user representation. For example, if `decimals` equals `2`, a balance of `505` tokens should be displayed to a user as `5.05` (`505 / 10 ** 2`). Tokens usually opt for a value of 18, imitating the relationship between Ether and Wei. This is the value {ERC20} uses, unless this function is overridden; NOTE: This information is only used for _display_ purposes: it in no way affects any of the arithmetic of the contract, including {IERC20-balanceOf} and {IERC20-transfer}.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint8` |



