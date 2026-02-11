# Ease

Built at **ETHGlobal 2025** with @Oliverpt-1.

Ease is a biometric smart account wallet that uses facial recognition to secure ERC-4337 smart accounts. Built on Kernel v3 and ERC-7579, it enables passwordless on-chain transactions authenticated by your face.

## Features

- **Facial Recognition Validator** - Custom ERC-7579 validator module using CompreFace for biometric authentication
- **Smart Account Wallets** - ERC-4337 account abstraction with Kernel v3
- **Merchant Payments** - On-chain checkout flow with `MerchantAccount` and `CheckoutProcessor` contracts
- **Cross-Chain Support** - LayerZero v2 integration for multi-chain operations

## Stack

- **Frontend**: Next.js, TypeScript, Radix UI
- **Smart Contracts**: Solidity, Foundry
- **Account Abstraction**: ERC-4337 (Kernel v3), ERC-7579
- **Biometrics**: CompreFace
- **Cross-Chain**: LayerZero v2

## Getting Started

```bash
# Install dependencies
npm install

# Run the development server
npm run dev
```

### Smart Contracts

```bash
# Build contracts
forge build

# Run tests
forge test

# Deploy to Sepolia
./deploy-sepolia.sh
```

### Environment Setup

Copy `.env.example` and fill in your values:

```bash
cp .env.example .env.local
```

See [README-DEPLOYMENT.md](./README-DEPLOYMENT.md) for Railway deployment instructions.

## Contracts

| Contract | Description |
|----------|-------------|
| `FaceRecognitionValidator` | ERC-7579 validator module for biometric auth |
| `MerchantAccount` | On-chain merchant payment accounts |
| `CheckoutProcessor` | Payment processing and checkout flow |
