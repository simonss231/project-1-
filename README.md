# 🏰 DeFi Empire: ERC20 & Vault Contracts

Welcome to the **DeFi Empire** project, where we harness the power of **Avalanche** subnets to create a decentralized finance (DeFi) platform inspired by **DeFi Kingdoms**. This repository contains the building blocks of your DeFi Empire: an ERC20 token and a Vault contract, designed to operate on a custom Avalanche EVM subnet.

---

## 🌟 Overview

This project is a step towards building a gamified DeFi experience where users can:

- **Mint and Burn Tokens** 🪙 using the ERC20 contract.
- **Deposit and Withdraw Assets** into a secure Vault.
- Explore Avalanche's **EVM Subnets** to reduce fees and enhance scalability.

Dive in to understand the mechanics of decentralized finance through **Solidity smart contracts** deployed on Avalanche.

---

## 📜 Contracts

### **1. ERC20 Token Contract**
The ERC20 contract is the foundation of your in-game economy. Here's what it does:

- **Mint Tokens**: Add to the total supply.
- **Burn Tokens**: Remove tokens from circulation.
- **Transfer Tokens**: Peer-to-peer token transfers.
- **Approve & Allowance**: Delegate spending authority.

#### Key Features
- `mint(uint amount)`: Mints new tokens to the caller's balance.
- `burn(uint amount)`: Burns tokens from the caller's balance.
- Standard functions: `transfer`, `approve`, and `transferFrom`.

📂 **File**: [`ERC20.sol`](./contracts/ERC20.sol)

---

### **2. Vault Contract**
The Vault contract acts as a decentralized bank, enabling users to deposit tokens and earn shares proportionate to their contributions.

#### Core Functionalities
- **Deposit Tokens**: Converts deposits into Vault shares.
- **Withdraw Tokens**: Converts shares back into tokens.

#### Key Features
- **Proportional Rewards**: Shares represent a user's stake in the Vault.
- **Efficiency**: Uses precise math to ensure fair share calculations.

📂 **File**: [`Vault.sol`](./contracts/Vault.sol)

---

## 🛠️ Setup & Deployment

### **Prerequisites**
- **Unix-based OS**: MacOS/Linux.
- **Development Tools**: Solidity, Remix, Metamask, and Avalanche CLI.
- **Wallet**: Metamask configured for Avalanche Fuji Testnet.

### **Deployment Steps**
1. **Create an EVM Subnet**: Follow the [Avalanche Subnet Guide](https://docs.avax.network/).
2. **Add Subnet to Metamask**: Use your Subnet's RPC endpoint.
3. **Deploy Contracts**:
   - Use Remix with the Injected Web3 provider (Metamask).
   - Deploy the `ERC20` contract first.
   - Deploy the `Vault` contract, linking it to your `ERC20` token.
4. **Test**:
   - Mint tokens and approve the Vault for deposits.
   - Deposit and withdraw tokens using the Vault.

---

## 🚀 How to Use

### **Interact via Remix**
1. Deploy the contracts.
2. Use the ERC20 contract to mint tokens.
3. Approve the Vault contract to handle your tokens.
4. Deposit tokens into the Vault and observe the shares allocation.

### **Transaction Example**
- **Mint Tokens**: Call `mint` with an amount (e.g., 1000 tokens).
- **Deposit Tokens**: Call `deposit` on the Vault with the approved amount.
- **Withdraw Shares**: Call `withdraw` to retrieve your proportionate tokens.

---

## 📚 Resources

- **Avalanche Documentation**: [Official Docs](https://docs.avax.network/)
- **Solidity Documentation**: [Solidity Lang](https://soliditylang.org/)
- **Metamask Setup**: [Metamask Guide](https://metamask.io/)

---
## 💡 Inspiration

This project is inspired by **DeFi Kingdoms** and aims to simplify the creation of gamified DeFi ecosystems on Avalanche. While this is just the beginning, it lays the groundwork for creating tokenized economies, staking, and reward systems.

---

## 🛡️ License
This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more details.

---
