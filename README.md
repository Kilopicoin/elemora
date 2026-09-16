# Elemora

A fully on-chain strategy game on **BNB Smart Chain (BSC)** built around daily progression, elemental tower strategy, long-term consistency, and a live BNB reward pool.

🌐 Live dApp: https://kilopi.net/elemora/

## Technology Stack

- **Blockchain**: BNB Smart Chain
- **Smart Contract**: Solidity ^0.8.24
- **Frontend**: Browser-based Web3 dApp
- **Architecture**: Fully on-chain game logic and persistent player progression
- **Native Asset**: BNB
- **Token Requirement**: None
- **Contract Verification**: Source code verified on BscScan

## Supported Networks

- **BNB Smart Chain Mainnet** — Chain ID: `56`

Elemora is currently deployed only on BNB Smart Chain Mainnet.

## Contract Addresses

| Network | Core Game Contract | Token Contract |
|---|---|---|
| BNB Smart Chain Mainnet | `0x4f0539B658f6EA529E61E1e24AE007Dda092C58b` | N/A |

### Verified Contract

https://bscscan.com/address/0x4f0539B658f6EA529E61E1e24AE007Dda092C58b#code

Elemora does not have its own token and does not require a project-specific token to play. The game uses native BNB for its Daily Wave fee and reward pool.

## Features

- **Fully On-Chain Gameplay**  
  Core game logic, player progression, tower levels, gold, kills, streaks, rewards, and voting are managed by the smart contract.

- **One Daily Core Action**  
  Each wallet can play one paid Daily Wave per game day.

- **Four Elemental Towers**  
  Players develop Fire, Water, Air, and Earth towers, each with different strengths and weaknesses.

- **Deterministic On-Chain Battles**  
  Wave results are calculated directly by the smart contract using tower levels, damage, monster HP, shots, and elemental multipliers.

- **Progressive Difficulty**  
  The number of monsters in Daily Waves increases as the player's progression advances.

- **Tower Progression**  
  Players earn in-game gold by defeating monsters and use it to upgrade their elemental towers.

- **Assault Seals**  
  Playing for seven consecutive days earns an Assault Seal. Seals can be spent on additional waves where the player chooses the enemy element.

- **Weekly Community Voting**  
  Players vote for an element during seven-day epochs. Voting power is based on the combined levels of the player's towers.

- **Weekly Waves**  
  The winning community-voted element determines the enemy element of the following Weekly Wave.

- **Live BNB Reward Pool**  
  80% of every Daily Wave fee is added to the live player reward pool, while 20% is sent to the project treasury.

- **Progression-Based Reward Cooldown**  
  Reward claim cooldowns are calculated on-chain using the player's tower strength relative to the total tower levels across the game.

- **No Game Token**  
  Elemora does not issue or require a separate cryptocurrency or game token. The only blockchain-native asset used by the game is BNB.

- **Immutable Core Rules**  
  Core gameplay parameters and reward rules are fixed at deployment. There is no owner/admin function that can modify individual player progression or rebalance the core game rules.

## Gameplay Overview

Every player begins with four elemental towers:

- Fire
- Water
- Air
- Earth

Players return each game day to play a Daily Wave, defeat monsters, earn in-game gold, and strengthen their towers.

Elemental matchups affect damage:

- Strong matchup: `150%`
- Neutral matchup: `100%`
- Weak matchup: `50%`

As players continue progressing, their Daily Waves become increasingly difficult.

Long-term consistency unlocks additional gameplay through Assault Seals, while tower progression also increases weekly voting power and influences reward eligibility.

## Reward Pool

Each paid Daily Wave automatically distributes its BNB fee according to the immutable smart contract rules:

- **80% → Live Player Reward Pool**
- **20% → Project Treasury**

When an eligible player successfully claims the reward pool, the entire currently available pool is transferred to the selected recipient.

The player's next reward cooldown is then calculated using their relative tower progression.

## Smart Contract Architecture

Elemora is designed so that core gameplay does not depend on a traditional centralized game server.

The smart contract handles:

- Player initialization
- Tower levels
- In-game gold
- Kill statistics
- Daily progression
- Consecutive-day streaks
- Assault Seals
- Daily Wave resolution
- Assault Wave resolution
- Weekly voting
- Weekly Wave resolution
- Reward pool accounting
- Reward eligibility and cooldowns

This allows the core game state and rules to remain publicly verifiable on BNB Smart Chain.

## Links

- **Play Elemora:** https://kilopi.net/elemora/
- **Kilopi:** https://kilopi.net/
- **Verified Contract:** https://bscscan.com/address/0x4f0539B658f6EA529E61E1e24AE007Dda092C58b#code

## License

The Elemora smart contract source code is released under the MIT License.
