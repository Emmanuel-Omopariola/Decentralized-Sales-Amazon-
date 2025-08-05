# Decentralized Sales Using Amazon As A Concept

A decentralized e-commerce platform that reimagines online marketplace functionality using blockchain technology, eliminating intermediaries while maintaining the familiar Amazon-like user experience.

## Overview

This project creates a decentralized marketplace that combines the familiar user experience of Amazon with the transparency, security, and decentralization benefits of blockchain technology. By eliminating traditional intermediaries, the platform enables direct peer-to-peer transactions between buyers and sellers while maintaining trust through smart contracts and community governance.

## Key Features

- **Decentralized Marketplace**: Direct buyer-seller transactions without intermediaries
- **Smart Contract Escrow**: Automated payment release upon delivery confirmation
- **Reputation System**: Blockchain-based reviews and seller ratings
- **Lower Fees**: Reduced transaction costs by eliminating middlemen
- **Global Access**: Borderless commerce with cryptocurrency payments
- **Transparent Governance**: Community-driven platform decisions

## Technology Stack & Tools

- **Solidity** (Writing Smart Contracts & Tests)
- **Javascript** (React & Testing)
- **[Hardhat](https://hardhat.org/)** (Development Framework)
- **[Ethers.js](https://docs.ethers.io/v5/)** (Blockchain Interaction)
- **[React.js](https://reactjs.org/)** (Frontend Framework)

## Requirements For Initial Setup

Before you begin, ensure you have the following installed:

- **[Node.js](https://nodejs.org/en/)** (v16 or higher)
- [Git](https://git-scm.com/)
- [MetaMask](https://metamask.io/) or another Web3 wallet

## Setting Up

### 1. Clone/Download the Repository

```bash
git clone https://github.com/yourusername/decentralized-sales.git
cd decentralized-sales
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Run tests

```bash
npx hardhat test
```

### 4. Start Hardhat node

```bash
npx hardhat node
```

### 5. Run deployment script

In a separate terminal execute:

```bash
npx hardhat run ./scripts/deploy.js --network localhost
```

### 6. Start frontend

```bash
npm run start
```

Visit `http://localhost:3000` to interact with the decentralized marketplace.

## Usage

### Contract Interaction Example

```javascript
import { ethers } from 'ethers';

const provider = new ethers.providers.Web3Provider(window.ethereum);
const signer = provider.getSigner();

const contractAddress = "0x...";
const contract = new ethers.Contract(contractAddress, ABI, signer);

// Example function call
const result = await contract.listItem(itemName, price, description);
```

## Testing

### Run All Tests

```bash
npx hardhat test
```

### Run Coverage Report

```bash
npx hardhat coverage
```

## Deployment

### Deploy to Testnet

```bash
npx hardhat run scripts/deploy.js --network goerli
```

### Verify Contracts

```bash
npx hardhat verify --network goerli DEPLOYED_CONTRACT_ADDRESS
```

## Contributing

We welcome contributions from the community!

### Development Process

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

- **emmaculate_eth**
