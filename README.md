Full Sail DEX
Full Sail is a next-generation Decentralized Exchange (DEX) on the Sui blockchain, engineered from the ground up to maximize Return on Emissions (ROE) and create the most capital-efficient and sustainable AMM ever designed.

Incubated by Aftermath Finance and backed by the Sui Foundation, Full Sail moves beyond the incremental improvements of existing ve(3,3) models to pioneer a new, more efficient paradigm we call ve(4,4).

Table of Contents
The Full Sail Innovation: Solving the Core Problems of Modern DEXs

Core Features

Technical Architecture

Getting Started

License

The Full Sail Innovation: Solving the Core Problems of Modern DEXs
Today's leading DEXs, while innovative, suffer from systemic flaws: misaligned tokenomics, inefficient emissions, reflexive sell pressure, and cumbersome governance. Full Sail addresses each of these issues with targeted solutions:

Problem

Full Sail's Solution

Massive Airdrops & Dilution

Strategic Initial Distribution. No massive airdrop. Early LPs are rewarded with a "best price guarantee" and boosted yield for locking liquidity, turning a spend into a long-term investment.

Inefficient Emissions

Concentrated Liquidity & Dynamic Fees. Built on a CLAMM from day one, ensuring higher fees per dollar of liquidity and maximizing capital efficiency.

Boring, Non-Strategic Voting

Responsive Organized Weighting (ROW). A weekly PvP voting game where users predict a pool's volume. Emissions are adjusted based on collective accuracy, directly tying rewards to revenue generation.

The "Great Unlock" & Inflation

Insurance Fund & oSAIL. A portion of protocol fees builds a yield-generating insurance fund to manage unlock volatility. Emissions are paid in oSAIL (an options token), giving LPs the choice to lock for full value or cash out at a discount that benefits the protocol.

Mercenary Capital & Bribes

Bribes for Liquidity Locking. Bribes are redirected to LPs in exchange for locking their Position NFTs, providing transparent, long-term liquidity security for all participants.

Core Features
Concentrated Liquidity AMM (CLAMM): Allows LPs to concentrate their capital in specific price ranges, dramatically increasing capital efficiency.

Dynamic Fee Tiers: Different pools can be created with different fee tiers (e.g., 0.05%, 0.30%, 1.00%), allowing fees to be optimized for different asset pairs.

ve(4,4) Tokenomics: A novel system built around the SAIL and oSAIL tokens to align long-term incentives between LPs, traders, and the protocol.

On-Chain TWAP Oracle: Every pool provides a reliable, manipulation-resistant Time-Weighted Average Price oracle for other protocols to build upon.

Protocol-Owned Liquidity (POL): A core strategy to build a sustainable liquidity foundation and reduce reliance on mercenary capital.

Technical Architecture
The Full Sail protocol is built on a modular and secure foundation using Sui Move. The core engine is a sophisticated Concentrated Liquidity AMM.

Core Modules
my_dex::pool: The main module that defines the Pool, Position, and AdminCap structs. It handles all core logic for swaps, liquidity provisioning, and fee collection.

my_dex::math_lib: A dedicated library for all fixed-point arithmetic required for price, tick, and liquidity calculations. (Note: This must be implemented with a professionally audited library).

my_dex::tick_manager & my_dex::bitmap: Helper modules that manage tick data and provide gas-efficient lookups for active liquidity, preventing DoS attacks and reducing swap costs.

On-Chain Objects
AdminCap: A unique capability object required to create new pools and collect protocol fees, securing the treasury.

Pool: A shared object representing a single liquidity pool for a specific token pair and fee tier.

Position (NFT): An owned object that represents a user's unique liquidity position, tracking its price range, liquidity amount, and earned fees.

Getting Started
This repository contains the core smart contracts for the Full Sail DEX.

Prerequisites:

Sui CLI

Move Language Extension for your IDE

Build & Test:

# Clone the repository
git clone [your-repo-url]
cd [your-repo-name]

# Build the package
sui move build

# Run tests
sui move test

License
The source code for Full Sail is licensed under the Business Source License 1.1 (BSL 1.1).

Permitted Use: You are free to copy, modify, and use this code for non-production purposes.

Prohibited Use: You may not use this code in a commercial or production setting without an additional license from Full Sail.

License Conversion: This license will automatically convert to a standard permissive open-source license (e.g., MIT) after a period of two years.

This license structure allows us to protect our innovative ve(4,4) mechanics during the crucial early stages of development while ensuring the protocol becomes fully open-source for the community in the long term.
