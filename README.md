# BitVault Finance

A Bitcoin-backed stablecoin protocol implemented on the Stacks blockchain.

## Overview

BitVault Finance is a decentralized finance (DeFi) protocol that enables users to mint stablecoins using Bitcoin as collateral. The protocol maintains stability through automated liquidation mechanisms, dynamic pricing oracles, and carefully calibrated risk parameters.

## Features

- Bitcoin-collateralized vault creation
- Stablecoin minting and redemption
- Multi-oracle price feeds
- Automated liquidation system
- Governance controls
- SIP-010 token standard compliance

## Core Components

### Vault System

- Minimum collateralization ratio: 150%
- Liquidation threshold: 125%
- Dynamic vault creation and management
- Unique identifier per vault

### Stablecoin

- Name: Bitcoin-Backed Stablecoin
- Symbol: BTCS
- Minting fee: 0.5%
- Redemption fee: 0.5%
- Maximum mint limit: 1,000,000 BTCS

### Price Oracle

- Decentralized price feed system
- Real-time BTC price updates
- Price validation mechanisms
- Timestamp verification

## Installation

1. Clone the repository

```bash
git clone https://github.com/benedict-drio/bitvault-finance.git
```

2. Install dependencies

```bash
clarinet install
```

## Usage

### Creating a Vault

```clarity
(contract-call? .bitvault-finance create-vault u1000000)
```

### Minting Stablecoins

```clarity
(contract-call? .bitvault-finance mint-stablecoin tx-sender u1 u5000)
```

### Redeeming Stablecoins

```clarity
(contract-call? .bitvault-finance redeem-stablecoin tx-sender u1 u2500)
```

## Testing

Run the test suite:

```bash
clarinet test
```

## Documentation

For detailed documentation, see:

- [Technical Documentation](./docs/TECHNICAL.md)
- [Security Policy](./SECURITY.md)
- [Contributing Guidelines](./CONTRIBUTING.md)

## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.

## Support

For support, please open an issue on GitHub or contact the team at nicholasbenedict04@gmail.com
