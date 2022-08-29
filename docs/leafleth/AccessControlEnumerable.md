# AccessControlEnumerable
> 
```

```




### 🔎 Details

Extension of {AccessControl} that allows enumerating the members of each role.


### 🎟 Events


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



## `DEFAULT_ADMIN_ROLE`

>👀 `view`




### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bytes32` |



## `getRoleAdmin`

>👀 `view`



### 🔎 Details

Returns the admin role that controls `role`. See {grantRole} and {revokeRole}. To change a role&#39;s admin, use {_setRoleAdmin}.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bytes32` |



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



## `renounceRole`

>👀 `nonpayable`



### 🔎 Details

Revokes `role` from the calling account. Roles are often managed via {grantRole} and {revokeRole}: this function&#39;s purpose is to provide a mechanism for accounts to lose their privileges if they are compromised (such as when a trusted device is misplaced). If the calling account had been revoked `role`, emits a {RoleRevoked} event. Requirements: - the caller must be `account`.



## `revokeRole`

>👀 `nonpayable`



### 🔎 Details

Revokes `role` from `account`. If `account` had been granted `role`, emits a {RoleRevoked} event. Requirements: - the caller must have ``role``&#39;s admin role.



## `supportsInterface`

>👀 `view`



### 🔎 Details

See {IERC165-supportsInterface}.

### → Returns



| Name | Type |
|:-:|:-:|
|  Not specified  | `bool` |



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



