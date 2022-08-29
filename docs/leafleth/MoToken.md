# MoToken
> 
```

```




### 🔎 Details

This contract is an extension of ERC20PresetMinterPauser which has implementations of ERC20, Burnable, Pausable,  Access Control and Context.  In addition to serve as the ERC20 implementation this also serves as a vault which will hold  1. stablecoins transferred from the users during token purchase and  2. tokens themselves which are transferred from the users while requesting for redemption  3. restrict transfers to only whitelisted addresses


### 🎟 Events


#### AccessControlManagerSet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| accessControlAddress | `true` | `address` |


#### Approval
| Name | Indexed | Type |
|:-:|:-:|:-:|
| owner | `true` | `address` |
| spender | `true` | `address` |
| value | `false` | `uint256` |


#### JuniorTokenLinked
| Name | Indexed | Type |
|:-:|:-:|:-:|
| token | `true` | `address` |


#### Paused
| Name | Indexed | Type |
|:-:|:-:|:-:|
| account | `false` | `address` |


#### RoleAdminChanged
| Name | Indexed | Type |
|:-:|:-:|:-:|
| role | `true` | `bytes32` |
| previousAdminRole | `true` | `bytes32` |
| newAdminRole | `true` | `bytes32` |


#### RoleGranted
| Name | Indexed | Type |
|:-:|:-:|:-:|
| role | `true` | `bytes32` |
| account | `true` | `address` |
| sender | `true` | `address` |


#### RoleRevoked
| Name | Indexed | Type |
|:-:|:-:|:-:|
| role | `true` | `bytes32` |
| account | `true` | `address` |
| sender | `true` | `address` |


#### SeniorTokenLinked
| Name | Indexed | Type |
|:-:|:-:|:-:|
| token | `true` | `address` |


#### TradabilitySet
| Name | Indexed | Type |
|:-:|:-:|:-:|
| tradable | `true` | `bool` |


#### Transfer
| Name | Indexed | Type |
|:-:|:-:|:-:|
| from | `true` | `address` |
| to | `true` | `address` |
| value | `false` | `uint256` |


#### Unpaused
| Name | Indexed | Type |
|:-:|:-:|:-:|
| account | `false` | `address` |



## `DEFAULT_ADMIN_ROLE`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bytes32` |



## `MINTER_ROLE`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bytes32` |



## `PAUSER_ROLE`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bytes32` |



## `UNDERWRITER_ROLE`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bytes32` |



## `accessControlManagerAddress`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



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



## `getRoleAdmin`

>👀 `view`



### 🔎 Details

Returns the admin role that controls `role`. See {grantRole} and {revokeRole}. To change a role&#39;s admin, use {_setRoleAdmin}.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bytes32` |



## `getRoleMember`

>👀 `view`



### 🔎 Details

Returns one of the accounts that have `role`. `index` must be a value between 0 and {getRoleMemberCount}, non-inclusive. Role bearers are not sorted in any particular way, and their ordering may change at any point. WARNING: When using {getRoleMember} and {getRoleMemberCount}, make sure you perform all queries on the same block. See the following https://forum.openzeppelin.com/t/iterating-over-elements-on-enumerableset-in-openzeppelin-contracts/2296[forum post] for more information.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `getRoleMemberCount`

>👀 `view`



### 🔎 Details

Returns the number of accounts that have `role`. Can be used together with {getRoleMember} to enumerate all bearers of a role.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint256` |



## `grantRole`

>👀 `nonpayable`



### 🔎 Details

Grants `role` to `account`. If `account` had not been already granted `role`, emits a {RoleGranted} event. Requirements: - the caller must have ``role``&#39;s admin role.



## `hasRole`

>👀 `view`



### 🔎 Details

Returns `true` if `account` has been granted `role`.

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



## `isTradable`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



## `juniorTokenAddress`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `mint`

>👀 `nonpayable`



### 🔎 Details

Creates `amount` new tokens for `to`. See {ERC20-_mint}. Requirements: - the caller must have the `MINTER_ROLE`.



## `name`

>👀 `view`



### 🔎 Details

Returns the name of the token.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `string` |



## `pause`

>👀 `nonpayable`



### 🔎 Details

Pauses all token transfers. See {ERC20Pausable} and {Pausable-_pause}. Requirements: - the caller must have the `PAUSER_ROLE`.



## `paused`

>👀 `view`



### 🔎 Details

Returns true if the contract is paused, and false otherwise.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



## `renounceRole`

>👀 `nonpayable`



### 🔎 Details

Revokes `role` from the calling account. Roles are often managed via {grantRole} and {revokeRole}: this function&#39;s purpose is to provide a mechanism for accounts to lose their privileges if they are compromised (such as when a trusted device is misplaced). If the calling account had been revoked `role`, emits a {RoleRevoked} event. Requirements: - the caller must be `account`.



## `revokeRole`

>👀 `nonpayable`



### 🔎 Details

Revokes `role` from `account`. If `account` had been granted `role`, emits a {RoleRevoked} event. Requirements: - the caller must have ``role``&#39;s admin role.



## `seniorTokenAddress`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `address` |



## `supportsInterface`

>👀 `view`



### 🔎 Details

See {IERC165-supportsInterface}.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



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



## `unpause`

>👀 `nonpayable`



### 🔎 Details

Unpauses all token transfers. See {ERC20Pausable} and {Pausable-_unpause}. Requirements: - the caller must have the `PAUSER_ROLE`.



## `isUnderwriter`

>👀 `view`

### 📋 Notice

Returns if the address is an underwriter



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _account | `address` | The address being checked |

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



## `decimals`

>👀 `pure`

### 📋 Notice

Overrides decimals() function to restrict decimals to 4



### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `uint8` |



## `burn`

>👀 `nonpayable`

### 📋 Notice

Burns tokens from the given address



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokens | `uint256` | The amount of tokens to burn |



## `transferTokens`

>👀 `nonpayable`

### 📋 Notice

Transfers MoTokens from self to an external address



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokens | `address` | The amount of tokens to transfer |

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



## `transferStableCoins`

>👀 `nonpayable`

### 📋 Notice

Transfers stablecoins from self to an external address



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _contractAddress | `address` | Stablecoin contract address on chain |

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



## `receiveTokens`

>👀 `nonpayable`

### 📋 Notice

Transfers MoTokens from an external address to self



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _tokens | `address` | The amount of tokens to transfer |

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



## `receiveStableCoins`

>👀 `nonpayable`

### 📋 Notice

Transfers stablecoins from an external address to self



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _contractAddress | `address` | Stablecoin contract address on chain |

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



## `setTradability`

>👀 `nonpayable`

### 📋 Notice

Setter for isTradable



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| tradable | `bool` | tradability set to true/false |



## `linkToSeniorToken`

>👀 `nonpayable`

### 📋 Notice

Link to a Senior token



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| seniorToken | `address` | Token address |



## `linkToJuniorToken`

>👀 `nonpayable`

### 📋 Notice

Link to a Junior token



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| juniorToken | `address` | Token address |



## `setAccessControlManagerAddress`

>👀 `nonpayable`

### 📋 Notice

Setter for accessControlManagerAddress



### ⚙️ Parameters

| Name | Type | Description |
|:-:|:-:| - |
| _address | `address` | Set accessControlManagerAddress to this address |



