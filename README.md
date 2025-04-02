# Utilize - Crypto Utility Payments for Africa

[![Arbitrum](https://img.shields.io/badge/Powered%20by-Arbitrum-blue)](https://arbitrum.io)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

## Overview
Africa's first non-custodial platform for paying utility bills (electricity, water, internet) directly with cryptocurrencies. Built for 600M+ unbanked Africans and $100B+ annual diaspora remittances.

**Key Stats**:
- 61% of African crypto users need utility payments (Stellar 2024)
- 40% avg. remittance fee savings vs traditional methods
- 200ms avg. transaction finality on Arbitrum

## Architecture
```mermaid
graph TB
    A[User] --> B{{Next.js/Flutter}}
    B --> C[Payment Router]
    C -->|Stablecoins| D[Arbitrum]
    C -->|Crypto| E[Chainlink]
    D/E --> F[Utility APIs]
    F --> G[DAO Treasury]
