# NFT Marketplace

This is a decentralized NFT (Non-Fungible Token) marketplace built on the Sepolia testnet, allowing users to mint, buy, and sell unique digital assets securely. The marketplace leverages Solidity for smart contracts, IPFS for decentralized storage, and the Alchemy API for enhanced blockchain interactions.

## Project Overview

The NFT Marketplace provides a decentralized platform for creating, listing, and trading NFTs directly from MetaMask, ensuring a secure and user-friendly experience. Built with Next.js for a responsive frontend, the project is designed to offer fast, decentralized transactions on the Ethereum Sepolia testnet.

### Features

- **Minting**: Users can create NFTs by uploading digital assets.
- **Buying & Selling**: Users can list their NFTs for sale or purchase NFTs from others.
- **Wallet Integration**: Connect with MetaMask to manage assets.
- **Decentralized Storage**: Utilizes IPFS and Pinata for secure, immutable media hosting.

## Technologies Used

### Blockchain

- **Sepolia Testnet**: Test environment for Ethereum blockchain development.
- **Hardhat**: Tool for testing, compiling, and deploying contracts.
- **Solidity**: Programming language for Ethereum smart contracts.

### Web3 & Wallet Integration

- **Web3.js**: Library for blockchain interaction.
- **MetaMask**: Wallet connection for asset management.

### APIs

- **Alchemy API**: Access to Ethereum blockchain on Sepolia.
- **Pinata & IPFS**: Decentralized storage for NFT assets.

### Frontend

- **Next.js**: Framework for server-side rendered, fast-loading web applications.

## Getting Started

### Prerequisites

- **Node.js** (v14+)
- **MetaMask** (browser extension)
- **Alchemy Account** (API Key for Sepolia)

### Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/jaygohil-x/NFT-Marketplace.git
   cd NFT-Marketplace
   ```

2. **Install Dependencies**

   ```bash
   npm install
   ```

3. **Configure Environment Variables**

   Create a `.env` file and add your API keys:

   ```plaintext
   ALCHEMY_API_KEY=your_alchemy_api_key
   NEXT_PUBLIC_PINATA_API_KEY=your_pinata_api_key
   NEXT_PUBLIC_PINATA_SECRET_API_KEY=your_pinata_secret_api_key
   ```

4. **Compile and Deploy Contracts on Sepolia**

   ```bash
   npx hardhat compile
   npx hardhat run scripts/deploy.js --network sepolia
   ```

5. **Start the Application**

   ```bash
   npm run dev
   ```

   The app runs on `http://localhost:3000`.

## Usage

1. **Connect Wallet**: Open the marketplace and connect your MetaMask wallet.
2. **Mint NFT**: Use "Mint" to upload your asset and mint an NFT.
3. **List for Sale**: Set a price and list minted NFTs for sale.
4. **Buy NFTs**: Browse and purchase available NFTs using MetaMask.

## Folder Structure

- **contracts/**: Solidity smart contracts.
- **pages/**: Next.js pages for the application.
- **scripts/**: Deployment scripts.
- **utils/**: Web3 and blockchain helpers.

