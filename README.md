# MyToken Smart Contract

![MIT License](https://img.shields.io/badge/License-MIT-blue)

**MyToken** is an Ethereum smart contract that allows you to create and manage a custom token. This contract is implemented in Solidity version 0.8.18 and follows specific requirements for managing token details, minting new tokens, and burning existing tokens.

## Table of Contents

- [Overview](#overview)
- [Token Details](#token-details)
- [Token Balances](#token-balances)
- [Mint Function](#mint-function)
- [Burn Function](#burn-function)
- [Conditions for Burning](#conditions-for-burning)
- [Getting Started](#getting-started)
- [License](#license)

## Overview

This smart contract serves as a basic example of how to create and manage a custom token on the Ethereum blockchain. It provides the essential functions for minting new tokens and burning existing tokens.

## Token Details

- **Token Name**: ENRI
- **Token Symbol**: Dog
- **Total Supply**: 1000

## Token Balances

The contract maintains a mapping of Ethereum addresses to token balances using the `BALANCES` mapping. Users can query the balance of any address on the blockchain.

## Mint Function

The `mint` function allows you to create new tokens. It takes two parameters: an address and a value. When tokens are minted, the function increases the total supply by the specified amount and increases the balance of the provided address by the same amount.

## Burn Function

The `burn` function works in the opposite way of the `mint` function. It allows for the destruction of tokens. It also takes an address and a value as parameters. The function deducts the specified value from both the total supply and the balance of the provided address.

## Conditions for Burning

The `burn` function includes conditional checks to ensure that the balance of the sender is greater than or equal to the amount that is supposed to be burned. Tokens cannot be burned in excess of the sender's balance.

## Getting Started

To use this smart contract, you can deploy it on an Ethereum testnet or a local Ethereum blockchain using a development environment like Remix or Truffle. Make sure to follow best practices for deploying and interacting with smart contracts.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
