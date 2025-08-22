# 🌱 CompostChain: Tokenized Platform for Composting Incentives

Welcome to CompostChain, a blockchain-powered platform that incentivizes individuals, households, and businesses to compost organic waste! By tracking composting activities on the Stacks blockchain, users earn redeemable tokens for their eco-friendly efforts, reducing landfill methane emissions and promoting sustainable waste management. This tackles the real-world problem of organic waste contributing to climate change—globally, food waste alone accounts for 8-10% of greenhouse gases—while creating a tokenized economy around environmental stewardship.

## ✨ Features

♻️ Submit and verify composting proofs with immutable blockchain records  
💰 Earn fungible tokens (COMPOST) for validated composting activities  
🏆 Mint NFTs for composting milestones and achievements  
🛒 Redeem tokens for eco-products, discounts, or carbon credits via partnerships  
📊 Track personal and community composting impact with transparent dashboards  
🗳️ Participate in governance to vote on reward rates and platform updates  
🔒 Secure user registration and anti-fraud measures to prevent duplicate claims  
🌍 Integrate with IoT devices or apps for automated composting logging  

## 🛠 How It Works

CompostChain uses the Stacks blockchain and Clarity smart contracts to ensure transparency, security, and decentralization. Users interact via a web/app interface that calls these contracts. The platform involves 8 smart contracts to handle registration, verification, rewards, and more.

### Core Smart Contracts (Written in Clarity)

1. **UserRegistry.clar**: Handles user registration, storing profiles (e.g., address, type: individual/business) and preventing duplicate accounts.  
2. **CompostLogger.clar**: Logs composting events by accepting hashes of proofs (e.g., photos, weight measurements, or IoT data) with timestamps for immutable tracking.  
3. **VerificationOracle.clar**: Allows trusted verifiers (oracles/partners) to approve or reject submissions, using multi-sig for fraud prevention.  
4. **CompostToken.clar**: SIP-010 compliant fungible token contract for issuing and managing COMPOST tokens as rewards.  
5. **RewardDistributor.clar**: Calculates and distributes tokens based on verified composting volume (e.g., kg of waste), with adjustable rates.  
6. **AchievementNFT.clar**: Mints non-fungible tokens (SIP-009) for milestones like "100kg Composted" to gamify participation.  
7. **RedemptionMarketplace.clar**: Enables token redemption for goods/services from partners, handling escrow and transfers.  
8. **GovernanceDAO.clar**: Manages proposals and voting using staked tokens to decide on platform parameters like reward multipliers.

### For Users (Composters)

- Register your account via the UserRegistry contract.  
- Compost organic waste and generate a proof (e.g., app photo or scale reading). Hash it and submit to CompostLogger.  
- Wait for verification through VerificationOracle—if approved, RewardDistributor automatically sends COMPOST tokens to your wallet.  
- Track progress: Hit milestones to mint NFTs via AchievementNFT.  
- Redeem tokens in the RedemptionMarketplace for real-world perks like discounts on sustainable products.

Boom! You're earning while helping the planet.

### For Verifiers/Partners

- Join as a trusted verifier to review submissions in VerificationOracle.  
- Sponsors can fund rewards through GovernanceDAO proposals.  
- Use get-user-impact or get-event-details functions across contracts to query data and verify claims instantly.

### For Developers/Community

- Stake COMPOST tokens in GovernanceDAO to propose changes, like new reward tiers.  
- Integrate IoT for auto-logging: Devices can call CompostLogger directly.  
- All contracts are open-source; deploy on Stacks testnet for testing.

That's it! Join CompostChain to turn waste into wealth and make composting rewarding for everyone. 🚀