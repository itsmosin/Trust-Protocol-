# Trust Protocol (An onchain trust primitive)

## Welcome to Trust Protocol

In the real world, trust has foundation in primitives like survival, social bonds, bloodlines etc. These trust primitives transform depending on time and place, the cavemen had a primitive of survival in order to form their trust. We might not be cavemen anymore, but humans crave connection and security, even in the digital ecosystems of today. Hence what if there is a new way to establish on-chain trust and reduce fraud in decentralized environments. Trust Protocol introduces on-chain trust bonds that allow users to put their money where their mouth is, proving trustworthiness while earning yield on their bond funds.

## Problem Statement

Trust redefines different human interactions, be that individuals interacting on markets or party members running a state. However, in decentralized environments, ensuring trust and credibility is challenging due to anonymity, the lack of robust verification mechanisms and lack quantifiable credibility. Hence the positive externalities trust brings in human interactions is low or even absent on chain. That is something we wanna change.

## Our Solution

### On-Chain Trust Bonds

- Users create bonds by depositing funds into an escrow which gives to only 2 users, the person creating the bond and the other pair signaling trust in another user.
- The funds in the bonds generate yield through yield bearing protocols (like Aave), allowing users to not ideally lock funds while still participating in the protocol.
- A bond score is measuring on the following parameters of, value locked in bond, number of bonds, context of other users bond score, time of bond and range of a user's bond value

### Challenges:

- **Sybil in Web3**: The ability to create multiple anonymous identities enables bad actors to exploit decentralized platforms through scams, rug pulls, and phishing attacks. Sybil resistance is a huge challenge for Trust protocol currently.
- **Track of Credibility**: Honest users have other reliable way to demonstrate trustworthiness which may not be captured fully by the protocol, reducing collaboration and opportunities.

## New Features

- **Social Trust Graph**: Reputation is calculated based on trust relationships and weighted metrics.
- **Types of Bonds**: Support for one-way and regular bonds with different weights in reputation scoring.
- **Transitive Trust**: A trusts B, B trusts C, so A indirectly trusts C, contributing to the social trust graph.
- **Community Reward Pool**: Yield from collected withdrawal fees, grants, and funds is distributed to honest and loyal bondholders.

## Reputation Score

Reputation lies at the core of Trust Protocol, encouraging users to behave honestly by rewarding good actions and penalizing bad ones.

### Parameters for Reputation Calculation:

- **Time**: Duration for which someone maintains trust bonds without dissolving them.
- **Amount**: Total bond money currently held by a user.
- **Reputation**: The reputation score of users creating bonds with you (higher reputation connections carry more weight).
- **Number**: Total number of active bonds.
- **Type of Bond**:
  - **One-Way Bonds**: User A trusts User B and deposits money without requiring B to reciprocate.
  - **Regular Bonds**: Both users deposit money, demonstrating mutual trust. Regular bonds carry a higher weight in score calculations.
- **Transitive Trust**: Trust connections through intermediaries enhance reputation, fostering a web of trust.

## Community Reward Pool

The Community Reward Pool incentivize loyalty and honesty within the ecosystem.

### Sources of the Reward Pool:

- **Withdrawal Fees**: Charged when users break bonds or dissolve them prematurely.
- **Dissolving Fees**: Small fees charged when users take back their money by dissolving bonds.
- **Grants and Funds**: Contributions from organizations supporting the protocol.

### Distribution:

Yield from the pool is distributed to bondholders who:
- Maintain bonds for longer durations.
- Actively create trust and build the community.

## Architecture

### How It Works

1. **Create/Join a Bond**:
   - Deposit funds into a bond (one-way or mutual).

2. **Earn Reputation**:
   - Active bonds increase your reputation over time.

3. **Breaking Bonds**:
   - Incurs a 5% penalty to the treasury, reputation loss, and an SBT (Soulbound Token) in your wallet marking you as a bond breaker.

4. **Build Credibility**:
   - On-chain reputation unlocks perks and trustworthiness across Web3 platforms.

### Sequence Diagram

*[Sequence diagram placeholder - to be added]*

### Technical Architecture Overview

*[Technical architecture image placeholder - to be added]*

### Smart Contracts Architecture

*[Smart contracts architecture placeholder - to be added]*

### Contracts Class Diagram

*[Contracts class diagram placeholder - to be added]*

## Use Cases

- **Proof of Trustworthiness**: Show verifiable trust for perks in dApps.
- **Earn Yield**: Deposits generate passive income.
- **Interoperable Reputation**: Carry your credibility across multiple platforms.
- **Fraud Prevention**: Discourage bad actors with transparent penalties and rewards.

## Getting Started

This is a [Next.js](https://nextjs.org) project built for the Sui blockchain.

### Prerequisites

- Node.js 18+ 
- pnpm (recommended)
- Sui wallet extension

### Installation

```bash
# Clone the repository
git clone https://github.com/itsmosin/Trust-Protocol-.git
cd Trust-Protocol-

# Install dependencies
pnpm install

# Run the development server
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the application.

### Environment Setup

Create a `.env.local` file with the necessary environment variables for Sui network configuration.

## Tech Stack

- **Frontend**: Next.js 14, React, TypeScript
- **Styling**: Tailwind CSS, shadcn/ui
- **Blockchain**: Sui Network
- **Wallet Integration**: Sui Wallet Adapter
- **State Management**: React Hooks

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

- Project Link: [https://github.com/itsmosin/Trust-Protocol-](https://github.com/itsmosin/Trust-Protocol-)
- Documentation: *[Coming soon]*

---

**Trust Protocol** - Building the future of on-chain trust and reputation.