# ETH-AVAX-TypesOfFunctions

# MyToken README

This repository contains the source code for the MyToken ERC-20 token written in Solidity. The token is based on the OpenZeppelin library, providing standard ERC-20 functionality. Below is an overview of the key components and functionalities of the MyToken contract.

## Overview

- **Name**: MyToken
- **Symbol**: CRZ
- **Decimals**: 18
- **Initial Supply**: Specified during deployment

## Features

1. **Constructor**: Initializes the token with a given name, symbol, and initial supply. The creator of the contract becomes the owner.

2. **Owner**: The `owner` variable stores the address of the contract owner. Only the owner has the authority to mint new tokens.

3. **Minting**: The `mint` function allows the owner to create new tokens and assign them to a specific address.

4. **Burning**: The `burn` function enables any address to burn a certain amount of their tokens.

5. **Transfer**: The `transfer` function is overridden to include custom logic. It allows token transfers between addresses.

6. **Modifier - onlyOwner**: A custom modifier, `onlyOwner`, ensures that only the owner can execute specific functions.

## Usage

### Prerequisites

- A development environment with a Solidity compiler
- [OpenZeppelin Contracts](https://github.com/OpenZeppelin/openzeppelin-contracts) library

### Deployment

1. Deploy the contract to your Ethereum development environment.
2. Specify the initial supply during deployment.

### Interact with the Contract

- Use a wallet or a tool like Remix to interact with the contract.
- The contract owner can mint new tokens using the `mint` function.
- Any address can burn its tokens using the `burn` function.
- Transfers between addresses can be executed using the standard ERC-20 `transfer` function.

### Important Note

- Ensure that you have the necessary OpenZeppelin Contracts installed (`ERC20.sol`).

## Disclaimer

This contract is provided as-is without any warranty. It is essential to review and test the code thoroughly before deploying it to a live network. The README is meant for informational purposes only and does not constitute financial or legal advice.
