# SportsContract README

## Overview

The `SportsContract` is a simple smart contract deployed on the Ethereum blockchain using Solidity. This contract manages a token called "Football" with the abbreviation "FS". It allows minting and burning of tokens, updating the total supply and individual balances accordingly.

## Contract Details

- **Token Name:** Football
- **Token Abbreviation:** FS
- **Initial Total Supply:** 110 FS

## Functionalities

### Public Variables

- `tokenName`: A `string` that stores the name of the token.
- `tokenAbbr`: A `string` that stores the abbreviation of the token.
- `totalSupply`: An `uint` that stores the total supply of the token.

### Mappings

- `balances`: A mapping from addresses to their respective token balances (`address => uint`).

### Functions

#### mint

The `mint` function allows the creation of new tokens.

- **Parameters:**
  - `addr`: The address to which the minted tokens will be assigned.
  - `amount`: The number of tokens to mint.

- **Functionality:**
  - Increases the total supply by the specified `amount`.
  - Increases the balance of the specified `addr` by the specified `amount`.

#### burn

The `burn` function allows the destruction of existing tokens.

- **Parameters:**
  - `addr`: The address from which the tokens will be burned.
  - `amount`: The number of tokens to burn.

- **Functionality:**
  - Decreases the balance of the specified `addr` by the specified `amount`, provided the balance is greater than or equal to the `amount`.
  - Decreases the total supply by the specified `amount`.

## Example Usage

### Minting Tokens

To mint tokens, call the `mint` function with the recipient's address and the amount to be minted.

