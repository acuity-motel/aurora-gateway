# Aurora Gateway (Built for Base)

Aurora Gateway is a read-only, onchain inspection tool designed for Base, offering network validation, balance checking, and block inspection capabilities with easy integration via Coinbase Wallet SDK.

---

## Repository layout

- app/aurora-gateway.ts  
  Browser-based script to connect a Coinbase Wallet and perform Base RPC queries.
  
- scripts/example-addresses.json  
  Example addresses for repeatable read-only checks.

- contracts/  
  Solidity contracts deployed to Base Sepolia for testnet validation:
  - mapping.sol — enables fast lookup of values using a key
  - inheritance_sequence — shows how inheritance works when multiple contracts inherit from a base contract 
  - errors.sol — defines custom errors for more efficient and readable failure handling  

- package.json  
  Manifest for project dependencies, including references to Base and Coinbase SDKs.

- README.md  
  Primary documentation for setting up and using the repository.

---

## Capabilities

- Coinbase Wallet SDK integration for wallet connection  
- Validation of Base Mainnet (8453) and Base Sepolia (84532) chainIds  
- Snapshot functionality to retrieve block height, timestamp, and gas data  
- Address inspection (balance, nonce, bytecode presence)  
- Independent verification via Basescan links  

---

## Base network context

Base Sepolia  
chainId (decimal): 84532  
Explorer: https://sepolia.basescan.org  

Base Mainnet  
chainId (decimal): 8453  
Explorer: https://basescan.org  

---

## Tooling and dependencies

This repository uses official tools from the Base and Coinbase ecosystems:
- Coinbase Wallet SDK for wallet connectivity  
- OnchainKit for Base-native tools and account abstraction  
- viem for typed, efficient RPC communication  
- Direct dependencies from Base and Coinbase GitHub repositories  

---

## License

MIT License

Copyright (c) 2025 YOUR_NAME

---

## Testnet Deployment (Base Sepolia)

As part of pre-production validation, one or more contracts may be deployed to the Base Sepolia test network to confirm correct behavior and tooling compatibility.

Network: Base Sepolia  
chainId (decimal): 84532  
Explorer: https://sepolia.basescan.org  

Contract mapping.sol address:  
0x01E9B446042b264989BB00aE6060b603682B8292

Deployment and verification:
- https://sepolia.basescan.org/address/0x01E9B446042b264989BB00aE6060b603682B8292
- https://sepolia.basescan.org/0x01E9B446042b264989BB00aE6060b603682B8292/0#code  

Contract inheritance_sequence.sol address:  
0xf7e0AF466ff0455515e5B34445e6Ed11611472c9 

Deployment and verification:
- https://sepolia.basescan.org/address/0xf7e0AF466ff0455515e5B34445e6Ed11611472c9 
- https://sepolia.basescan.org/0xf7e0AF466ff0455515e5B34445e6Ed11611472c9/0#code  

Contract errors.sol address:  
0x1708eC50fd5741320C4011bcBfAc2e744934C6eD

Deployment and verification:
- https://sepolia.basescan.org/address/0x1708eC50fd5741320C4011bcBfAc2e744934C6eD
- https://sepolia.basescan.org/0x1708eC50fd5741320C4011bcBfAc2e744934C6eD/0#code  

These testnet deployments provide a controlled environment for validating Base tooling, account abstraction flows, and read-only onchain interactions prior to Base Mainnet usage.

---

## Author

GitHub: https://github.com/acuity-motel

Email: acuity.motel.0q@icloud.com 

My twitter: https://x.com/lissagavingreen
