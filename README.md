# Proplex

A modern admin dashboard for the Proplex platform, built with React, TypeScript, Vite, Redux Toolkit, and Tailwind CSS. Proplex is a pioneering blockchain platform democratizing access to high-value real-world assets (RWAs) such as commercial real estate, private equity, and infrastructure projects. By enabling fractional ownership through tokenized assets, Proplex removes traditional barriers and empowers global retail investors to participate in opportunities previously limited to institutions.

Built natively on Story Protocol, Proplex leverages its decentralized IP graph, scalable infrastructure, and trustless verification layers to deliver secure, compliant, and high-performance RWA tokenization.

At its core, Proplex introduces a dual-token system:

- Asset Tokens representing direct ownership in RWAs
- Proplex Utility Token (PXT) used for governance, network fees, and ecosystem participation

All transactions, settlements, and compliance validations occur through Story Protocol's composable network modules, ensuring transparent, verifiable, and cost-efficient operations.

By merging structured compliance, decentralized governance, and real-world asset backing, Proplex bridges the gap between traditional finance (TradFi) and Web3, enabling a global, borderless investment economy.

## Demo

Proplex Demo Link: https://drive.google.com/drive/folders/1l6PdWTQI5-5WgsBa-yXufjypg_KBIQGx

Live Demo: https://proplex.vercel.app/

## Introduction

Traditional financial markets restrict access to high-value assets due to high entry minimums, jurisdictional barriers, and heavy intermediaries. Historically, only accredited and institutional investors have enjoyed access to high-yield assets such as real estate and private equity.

Proplex transforms this landscape by enabling regulated fractional ownership of real-world assets on Story Protocol, powered by 24/7 liquidity, transparent auditing, and automated yield distribution.

Unlike speculative DeFi systems, Proplex incorporates regulatory frameworks using Special Purpose Vehicles (SPVs) and on-chain identity systems (such as OnChainID) ensuring full KYC/AML compliance at the protocol layer.

Story Protocol's infrastructure—designed for composable, scalable, permissionless applications—enables Proplex to deliver institutional-grade RWA tokenization with speed, security, and verifiability.

## Challenges in RWA Tokenization

Proplex directly addresses the industry's most critical obstacles:

### Regulatory Fragmentation

Global compliance rules vary dramatically across regions.

✅ Proplex uses jurisdiction-specific SPVs, Story Protocol-verified compliance modules, and standard-aligned frameworks (MiCA, MAS Sandboxes, etc.).

### Ownership Verification

Tokens must reflect legally enforceable ownership.

✅ Proplex uses legal wrappers, oracle-verified metadata, and Story Protocol's immutable IP graph for traceable ownership.

### Liquidity Constraints

RWA tokens often fail to scale due to illiquidity.

✅ Proplex integrates story-native DEX markets, PXT staking rewards, and secondary trading within the ecosystem.

### Security Risks

Smart contract vulnerabilities threaten user trust.

✅ Proplex applies audited smart contracts, Chainlink oracles, and multi-sig custody using Story Protocol-compatible security modules.

### User Adoption

New Web3 participants need simplified UX.

✅ Proplex provides clean dashboards, Story Protocol-based identity flows, and a frictionless investment process.

## Proplex Platform Overview

Proplex enables the full lifecycle of RWA tokenization, investment, trading, and governance—all secured by Story Protocol.

### Key Asset Classes

- Commercial / Residential Real Estate (yield-generating)
- Private Equity Funds
- ESG Infrastructure / Renewable Projects

### Core Features

- Fractional Tokenization using ERC-3643 (T-REX) compliance
- Story Protocol Settlement Layer for fast, low-cost transactions
- Automated Yield Distribution through on-chain contracts
- Proplex Marketplace / DEX for secondary trading
- DAO Governance using PXT
- onChainID-based KYC for regulated access

### Workflow

#### 1. Asset Onboarding

- Issuers submit assets for verification
- SPVs (e.g., StoryChain Asset SPV) structure legal ownership
- Oracles validate data and valuation

#### 2. Tokenization & Sale

- Assets fractionalized into ERC-3643 Asset Tokens
- Story Protocol identity modules enforce compliance
- Primary sale executed through escrow smart contracts

#### 3. Investment & Yield

- Investors purchase Asset Tokens with seamless onboarding
- Yields auto-distributed via smart contracts

#### 4. Secondary Liquidity

- Tokens tradable in the Proplex DEX
- LPs earn fees + PXT staking rewards

#### 5. Governance & Redemption

- PXT holders vote on platform upgrades and listings
- Tokens redeemable for underlying value via oracle-based NAV

## Technology & Architecture

### Blockchain Layer

- Story Protocol as the foundational blockchain
- High scalability for metadata, licensing, compliance
- Trustless verification + modular composability

### Smart Contracts

- ERC-3643 regulated RWA contracts
- Escrow, yield distribution, trading, compliance automation
- Fully audited and Story-native optimized

### Data & Compliance Layer

- Chainlink oracles for valuation
- OnChainID for identity management
- SPV legal oracles for enforceability

### Security Infrastructure

- Multi-sig governance treasury
- Smart contract insurance partners
- Decentralized frontend hosted via IPFS

## Roadmap

| Phase | Timeline | Milestones |
|-------|----------|------------|
| Launch Phase | Q4 2025 | Story Protocol deployment, SPV pilots, wallet integration |
| Growth Phase | Q1–Q2 2026 | First real estate tokenization, DAO activation |
| Expansion Phase | Q3–Q4 2026 | Global partners, DEX v2, $100M TVL |
| Maturity Phase | 2027+ | Institutional onboarding, AI-driven curation, $1B AUM |

## Features
- Modular, scalable codebase for RWA tokenization, DAO governance, and compliance management
- TypeScript for type safety in handling on-chain assets, yields, and KYC/AML data
- Redux Toolkit for state management of Story Protocol portfolios, USDC transactions, and PXT governance
- React Hook Form & Zod for robust form validation in asset onboarding, SPV setup, and investor verification
- Tailwind CSS for rapid UI development of intuitive, responsive dashboards
- Code splitting and lazy loading for performance in real-time oracle feeds and liquidity pool monitoring
- REST API integration with Chainlink oracles and Story Protocol RPC endpoints
- Responsive design enabling seamless admin oversight on desktop and mobile for global operations

## Getting Started

### Prerequisites
- Node.js (v18 or higher recommended)
- npm or yarn

### Installation
```bash
git clone <repo-url>
cd proplex-admin
npm install # or yarn install
```

### Running the App
```bash
npm run dev # or yarn dev
```
The app will be available at [http://localhost:5173](http://localhost:5173).

### Building for Production
```bash
npm run build # or yarn build
```

### Linting & Formatting
```bash
npm run lint
npm run format
```

## Project Structure
- `src/components/` — Reusable UI components for RWA workflows and governance interfaces
- `src/pages/` — Application pages for asset management, investor dashboards, and DAO voting
- `src/store/` — Redux slices and store setup for Story Protocol state, yields, and compliance tracking.
- `src/hooks/` — Custom React hooks for blockchain interactions and automated distributions
- `src/types/` — TypeScript type definitions for tokens (ERC-3643), RWAs, and regulatory entities
- `src/config/` — App configuration files for chains, oracles, and USDC settlements
- `src/helpers/` — Utility/helper functions for validations, date formatting, and interoperability

## Detailed Project Structure

### Components
- `Curd/` — CRUD-related components for managing Asset Tokens and SPVs.
- `LoadingSpinner.tsx` — A spinner component for loading states during Chainlink oracle queries.
- `LocationCard.tsx` — Displays location-related information for real estate and infrastructure RWAs.
- `OrderStatusCard.tsx` — Represents investment and yield status visually (e.g., tokenized, distributed).
- `SearchFilter.tsx` — A search filter component for asset classes and liquidity pools.
- `TableComponent/` — Components for table rendering of portfolios, trades, and governance proposals.
- `UseForm/` — Form-related components for KYC (Civic), issuance, and redemption workflows.
- `cards/` — Card UI components for asset overviews, yield analytics, and PXT staking.
- `common/` — Common reusable components for Story Protocol displays and USDC transaction flows.
- `form/` — Form-specific components for primary sales, secondary trading, and fee calculations.
- `role/` — Role-based UI components for admins, issuers, liquidity providers, and DAO voters.
- `spv/` — SPV-related components for jurisdiction-specific legal wrappers and compliance.
- `stepper.tsx` — A stepper component for multi-step processes like asset onboarding and tokenization.
- `ui/` — General UI components for dashboards, charts, and real-time reporting.

### Hooks
- `useAddAdvisor.tsx` — Hook for adding advisors to private equity and infrastructure projects.
- `useAddBank.tsx` — Hook for adding bank details in fiat on-ramps and USDC conversions.
- `useAddBoardMember.tsx` — Hook for adding board members to SPVs and RWA entities.
- `useApi.tsx` — General API interaction hook for LayerZero, Chainlink CCIP, and Circle integrations.
- `useCancel.tsx` — Hook for handling investment cancellations and proposal retractions.
- `useCreateCompany.tsx` — Hook for creating SPVs and fractionalizing RWAs into Asset Tokens.
- `useCrud.tsx` — CRUD operation hooks for tokens, listings, and liquidity incentives.
- `useDebounce.tsx` — Debounce utility hook for searches in asset discovery and investor queries.
- `useDeleteAdvisor.tsx` — Hook for deleting advisors from RWA portfolios and governance.
- `useDeleteCompanyMember.tsx` — Hook for deleting members from equity funds and teams.
- `useDistribution.tsx` — Hook for handling automated yield distributions in USDC.
- `useEOI.tsx` — Hook for managing expressions of interest in new RWA listings.
- `useEmployee.tsx` — Hook for employee-related operations in DAO and platform teams.
- `useFeePercentage.tsx` — Hook for fee percentage calculations in DEX trades and staking.
- `useFetchCompany.tsx` — Hook for fetching RWA data via valuation oracles.
- `useInvestors.tsx` — Hook for managing verified investors and Civic KYC/AML checks.
- `useLocations.tsx` — Hook for location-related operations in real estate tokenization.
- `useRoyalties.tsx` — Hook for handling royalties from rental yields and dividends.
- `useStatements.tsx` — Hook for managing financial statements, audit trails, and tax reports.

### Other Notable Folders
- `src/config/` — Configuration files for charts (yield projections), dialogs (compliance alerts), and tables (asset listings).
- `src/constants/` — Default values and utility constants for chains, ERC-3643 standards, and USDC addresses.
- `src/helpers/` — Helper functions for global operations, date formatting, validations, and Story Protocol bridging.
- `src/layout/` — Layout components for the application, including navigation for Story Protocol and phases.
- `src/pages/` — Contains application pages like `customers` (investors), `investors` (portfolios), and `governance` (DAO).
- `src/store/` — Redux store setup and slices for PXT voting, USDC balances, and RWA metadata.
- `src/types/` — TypeScript type definitions for RWAs, tokens, oracles, and MiCA compliance.
- `src/utils/` — General utility functions for oracle parsing, Snapshot integration, and IPFS hosting.

This structure ensures modularity and scalability, aligning with Proplex's Story Protocol-based RWA ecosystem and hackathon-ready deployment.

## Environment Variables
Create a `.env` file in the root directory and add the required variables:
```
VITE_API_URL=<your-api-url>
VITE_STORY_PROTOCOL_RPC=<story-protocol-rpc-url>
VITE_CHAINLINK_ORACLE=<chainlink-oracle-url>
VITE_ONCHAINID_CONTRACT=<onchainid-contract-address>
VITE_PXT_TOKEN_ADDRESS=<pxt-token-contract-address>
VITE_ASSET_TOKEN_FACTORY=<asset-token-factory-address>
```

## Security Notice
**Never commit sensitive information (API keys, private keys, passwords) to the repository.** Smart contracts are audited for reentrancy and overflows; compliance enforced via Civic and Gnosis Safe multisigs. Nexus Mutual coverage recommended for production.

## Contributing
Pull requests are welcome! For major changes, especially regulatory or chain expansions, please open an issue first to discuss. Ideal for hackathon collaborators on RWA pilots.

## License
[MIT](LICENSE)