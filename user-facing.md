**Table of Contents**
* [Problem Statement](https://github.com/alokm/defi-wallet#problem-statement)
* [User Facing Improvements](https://github.com/alokm/defi-wallet/blob/main/user-facing.md#user-facing-product-improvements)
* [Backend Improvements](https://github.com/alokm/defi-wallet/blob/main/Backend.md#backend-product-operations)

# User-facing Product Improvements

Below are several suggestions for product roadmap candidates designed to drive significant growth or deepen user engagement for defi-wallet.

## defi-wallet Roadmap Candidates - Summary

 1. *[Your gateway to deFi](https://github.com/alokm/defi-wallet/blob/main/user-facing.md#1-your-gateway-to-defi)* - product messaging strategy to reach new users 
 2. *[Save your seed](https://github.com/alokm/defi-wallet/blob/main/user-facing.md#2-save-your-seed)* - product feature to build trust and drive virality
 3. *[What is deFi?](https://github.com/alokm/defi-wallet/blob/main/user-facing.md#3-what-is-defi)* - product education strategy to support new user growth
 4. *[Name your wallet](https://github.com/alokm/defi-wallet/blob/main/user-facing.md#4-name-your-wallet)* - product renaming powered by the community
 
## defi-wallet Roadmap Candidates - Details

### 1. Your gateway to deFi
A small pivot on product messaging strategy away from individual features and towards a vision relevant to our next 1 million users

**Vision: Enabling economic freedom and empowerment through access to open and interoperable decentralized monetary networks.**

**Current Product message**: defi-wallet offers a non-custodial multi-chain cryptocurrency wallet with built-in cross-chain atomic swaps.

**Revised Product message** defi-wallet is a multi-chain wallet that offers users a gateway to the world of decentralized finance.

**With defi-wallet** 
* users can access Bitcoin, Ethereum, Sidechains, Stablecoins, NFTs and a new universe of decentralized apps (dapps)
* users can easily and securely swap between any two assets in a trusted and completely decentralized way using atomic swaps
* users have the easiest gateway to the decentralized universe bridging main-chains and side chains, stablecoins and NFTs or other dapps.
* **more benefit statements** - see [User Persona](https://github.com/alokm/defi-wallet/blob/main/Backend.md#user-persona-model)
 - new users can ..
 - experienced users can ..
 - casual users can ..
 - power users can ..

### 2. Save your seed

Multi-user seed phrase backup and recovery strategy

**Problem: How do I backup my seed phrase and password?**
- For users of a non-custodial wallet such as defi-wallet, the problem of securely and safely backing up one's seed phrase is a serious consideration. 
- Many users would agree that most wallets have not done enough to protect them from loss of funds due to user errors that are easily recoverable when dealing with traditional centralized systems. 
- Non-custodial wallets such as defi-wallet
-  do not offer a universal mechanism for seed phrase recovery or password recovery in the case of catastrophic loss of a device or other valid recovery mode. 
- The default experience for new users is therefore likely to result in the catastrophic loss of funds in the case of a device failure or if the user loses their password. This is unacceptable for a cryptowallet and yet it is the default experience for users of any hardware wallet or other non-custodial wallet today.

**Current Solution: Write it down somewhere safe and don't lose it**

- A user is expected to be extremely diligent and proactive in the setup and ongoing maintenance of a system to store their seed phrase offline in a safe, secure, weather-proof, theft-resistant, disaster-resistant, physically redundant location. 
- **Traditional Advice:** Write it down somewhere safe and don’t lose it is harder than it looks for users to follow. It is not safe to assume that most or even many users follow best practice in securing their seed phrase offline. Given that the seed phrase is more important than the wallet, this is a scary situation.
- **Key Takeaway**  Most non-custodial wallets are borderline negligent in that they do virtually nothing to prevent their users from losing access to funds without recourse. At best they check that a user has recorded their seed phrase on wallet install, but none take responsibility for helping users on Day 2 to infinity of seed phrase backup. This is an opportunity to build trust.
	- Most non-custodial wallets only test that the user can reproduce the seed phrase at the time of wallet creation. 
	- After that some wallets never allow a user to recover their seed phrase under any circumstances. 
	- Other wallets will allow users to recover their seed phrase provided they have authenticated another way (usually a password)
	- All available wallets rely on the hope that the device is not damaged beyond usability say in the example of a catastrophic hardware loss. If the device is damaged beyond use then it is no longer possible to recover a user’s seed phrase so we better hope they wrote it down safely.
	- A better solution would be one that could offer redundant secure off-site backups of a seed phrase that is done so that no one other than the user ever has access to the user’s seed phrase.

**Better Conclusion** - seed of a new feature request. subject to feedback.

defi-wallet should offer a better solution. One that stores seed phrases securely in a physically redundant setup that relies on ones close friends and/or the community to help you recover a lost seed phrase without you ever losing exclusive access to the seed phrase.
 * Solution can allow a user to recover a seed phrase if they validate identity with a friend or friends (similar to [Argent](https://www.argent.xyz/) app)
 * Solution could leverage the community to recover a seed phrase if user validates identity securely through the community (using zk-Snarks)
* The point is not to propose this as a solution to the problem. Instead it is to propose this problem as a worthy one of going deep on together.

**Viral and Network Effects** - driving viral adoption while dramatically increasing long-term retention

* By leveraging a user's real-world closest crypto-friendly friends as their *Seed Recovery* backup system, defi-wallet makes social networks a part of your seed phrase backup strategy, driving virality and long-term retention.
* The solution also drives virality and network effects to drive adoption and increase retention by encouraging users to build a personal trusted network of one or more close friends to serve as your backup as social network.


### 3. What is deFi?
Build a web gateway to deFi for normals that provides an encyclopedia-like experience on crypto offerings and acts as a funnel to channel users from no-coiners to deFi maximalists. Optionally license content and data from a 3rd party like Messari.io or alternative

**Problem**
Most of defi-wallet’s future users are not yet mature enough on their *DeFi lifecycle of knowledge* to be able to be high-quality long-term users. We therefore need to help grow our users by helping them navigate the complex and fast evolving distributed finance landscape. Helping users go from noobs to experts on the DeFi universe so they understand which products solve what use cases and users develop the skill of evaluating a new crypto technology. This is how we will win the hearts and minds of new DeFi-curious users and how defi-wallet will grow its user base by 100x.

**Solution**
A content-rich website that takes a complete noob through the process of understanding *What is deFi?*. Beginning understanding the benefits and risks of each currency defi-wallet supports, how they work, and what traditional options they replace. This will help serve as an ongoing inbound content marketing funnel to attract and retain an educated user who will understand how to take full advantage of their defi-wallet.

### 4. Name your wallet
Community engagement in renaming defi-wallet
I think the defi-wallet name could be replaced with something stronger. I believe the community could help us rename the wallet. I propose we build a feature that allows the community to collaborate on the renaming. It would include a leaderboard for voting and comments as well as the ability for users to choose a name from the leaderboard that would re-brand the app and allow users to vote for their preference while signaling for their preference.

**Why it is a good idea**
This strategy drives community engagement and ownership around the product through naming rights. We want the community to feel the ownership and this is a great way to do it. We could run the campaign for up to a year or so to get lots of marketing mileage from the democratic process and then rename it once it is clear that we have consensus around a new name.

## Next Steps

* Explore [Backend Product Improvements](https://github.com/alokm/defi-wallet/blob/main/Backend.md#backend-product-operations)
