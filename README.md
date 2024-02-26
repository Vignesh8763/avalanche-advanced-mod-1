# Vault Contract README

## Introduction to the Vault Contract

The Vault contract is an Ethereum smart contract designed to facilitate the secure and efficient deposit and withdrawal of ERC-20 tokens. Serving as a secure storage facility, it allows users to deposit tokens to receive vault shares and withdraw tokens by redeeming these shares.

### Functionality Overview

1. **`deposit(uint _amount)`**
   - Enables users to deposit ERC-20 tokens into the vault, acquiring shares proportional to their deposit.
   - Utilizes a mathematical algorithm to determine the number of shares to mint based on the current total supply and token balance of the vault.

2. **`withdraw(uint _shares)`**
   - Allows users to exchange a specified number of shares for an equivalent amount of ERC-20 tokens.
   - Utilizes a mathematical algorithm to calculate the quantity of tokens to withdraw based on the current total supply and token balance of the vault.

### Contract Variables

- `token`: Represents an instance of the ERC-20 token interface managing the token within the vault.
- `totalSupply`: Denotes the total shares minted by the vault.
- `balanceOf`: Maps user addresses to their respective share balances within the vault.

## ERC20 Contract README

# Introduction to the ERC-20 Token Contract

The ERC20 contract provides a fundamental implementation of the ERC-20 token standard on the Ethereum blockchain. It facilitates the creation of fungible tokens with functionalities including transfers, allowances, approvals, minting, and burning.

### Key Features

- **`transfer`**: Enables users to transfer tokens to another address.
- **`approve`**: Allows users to authorize another address to spend tokens on their behalf.
- **`transferFrom`**: Facilitates delegated token transfers between addresses based on prior approval.
- **`mint`**: Enables the creation of new tokens by increasing the total supply.
- **`burn`**: Permits the destruction of tokens by decreasing the total supply.

### Contract Variables

- `totalSupply`: Represents the overall supply of the ERC-20 token.
- `balanceOf`: Maps user addresses to their respective token balances.
- `allowance`: Maps owner addresses to spender addresses along with the permitted token amounts.

### Event Emission

- **`Transfer`**: Triggered upon the transfer of tokens from one address to another.
- **`Approval`**: Triggered when an owner authorizes another address to spend tokens on their behalf.

### Token Details

- `name`: Specifies the name of the ERC-20 token ("Solidity").
- `symbol`: Represents the symbol for the ERC-20 token ("SOL").
- `decimals`: Indicates the number of decimals for token representation (18).
## Author

Vignesh V 
