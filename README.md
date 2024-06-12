# MyToken Contract

## Overview

MyToken is a simple ERC20-like token implemented in Solidity. This smart contract allows minting and burning of tokens, with basic functionalities to track balances and total supply.

## Features

1. **Public Variables**: 
   - `name`: The name of the token (MyToken).
   - `symbol`: The symbol of the token (MTK).
   - `totalSupply`: The total supply of tokens in existence.

2. **Mappings**:
   - `balances`: A mapping to track the balance of each address.

3. **Functions**:
   - `mint(address to, uint256 value)`: Increases the total supply and the balance of the specified address.
   - `burn(address from, uint256 value)`: Decreases the total supply and the balance of the specified address, with a check to ensure the balance is sufficient.

## Usage

### Minting Tokens

To mint new tokens, call the `mint` function with the recipient's address and the amount of tokens to mint:

```solidity
mint(address recipient, uint256 amount)
