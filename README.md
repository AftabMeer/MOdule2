# PurchaseTickets Smart Contract

This is a simple Solidity smart contract named `PurchaseTickets` that allows users to purchase tickets and check whether they have purchased a ticket or not. Below is a brief explanation of the contract's functionality and usage.

## Table of Contents
- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
  - [Contract Deployment](#contract-deployment)
- [Usage](#usage)
  - [Purchase a Ticket](#purchase-a-ticket)
  - [Check Ticket Purchase](#check-ticket-purchase)
- [License](#license)

## Introduction

This Solidity smart contract, with the SPDX-License-Identifier set to MIT, is designed to manage ticket purchases. It features a basic implementation of purchasing tickets and checking whether a ticket has been purchased by a specific Ethereum address. The contract has an owner who can control its functions, and users can purchase tickets through this contract.

## Prerequisites

Before using this smart contract, you should have:

- A development environment set up for Ethereum smart contract development.
- Knowledge of deploying and interacting with smart contracts.
- An Ethereum wallet or client to execute transactions.

## Getting Started

### Contract Deployment

1. Compile and deploy the `PurchaseTickets.sol` smart contract using your preferred Ethereum development environment, such as Remix or Truffle.

2. Ensure that you have sufficient Ether in your Ethereum wallet to deploy the contract.

3. Deploy the contract, and the owner will be set to the Ethereum address that deploys the contract.

## Usage

### Purchase a Ticket

To purchase a ticket, follow these steps:

1. Call the `purchaseTicket` function.

   This function will set the `ticketPurchased` mapping to `true` for the sender's address, indicating that they have purchased a ticket.

### Check Ticket Purchase

To check whether a specific address has purchased a ticket, follow these steps:

1. Call the `checkPurchase` function.

   This function will return `true` if the sender's address has purchased a ticket and `false` otherwise.

Please note that only the owner of the contract can access the `Onlyowner` function, which restricts certain operations to the owner's address.

## License

This smart contract is released under the MIT License. You can find the full text of the license in the SPDX-License-Identifier specified at the beginning of the contract. Feel free to use, modify, and distribute this code in accordance with the MIT License terms.
