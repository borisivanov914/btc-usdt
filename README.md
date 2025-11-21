# BTC/USDT Token (Ethereum)

**Contract Address:** `0xd5a90C85555Ee13863EE2b7a07D4B8807218Ef6b`  
**Network:** Ethereum Mainnet  
**Token Name:** BTC/USDT  
**Symbol:** BTCUSDT  
**Decimals:** 8  

---

## Overview

BTC/USDT is an experimental ERC-20 token deployed on the Ethereum Mainnet.  
It is designed for research purposes, particularly for studying wrapped-asset behavior, liquidity formation, price discovery mechanics, and chart visibility in modern cryptocurrency wallets (MetaMask, Coinbase Wallet) and DeFi platforms.

This token features an intentionally **ultra-limited supply (5 tokens total)**, enabling experiments with:

- DEX liquidity pools (especially Uniswap v2/v3),
- price chart rendering in wallets,
- price-tracking behavior of portfolio apps,
- wrapped-asset modeling similar to WBTC or synthetic BTC assets,
- DeFi risk modelling and AMM behavior under extreme scarcity conditions.

>  **Note:** BTC/USDT is not a financial product. It is an experimental asset created solely for technical and research activities.

---

## Technical Specification

- **Standard:** ERC-20 (OpenZeppelin)
- **Contract:** [`0xd5a90C85555Ee13863EE2b7a07D4B8807218Ef6b`](https://etherscan.io/token/0xd5a90C85555Ee13863EE2b7a07D4B8807218Ef6b)
- **Decimals:** 8
- **Total Supply:** `5.00000000 BTCUSDT`
- **Network:** Ethereum Mainnet (chainId `1`)
- **Libraries Used:**
  - OpenZeppelin `ERC20`
  - OpenZeppelin `Ownable`
  - OpenZeppelin `Pausable`

### Contract Features

- `pause()` / `unpause()` — emergency pause mechanism (owner-only).  
- `burnFromAny(address account, uint256 amount)` — burn tokens from any address (owner-only).  
- `rescueERC20(address token, address to, uint256 amount)` — recover any ERC-20 tokens mistakenly sent to the contract (except BTCUSDT).

---

## Use Cases & Research Applications

BTC/USDT can be used for:

### ► DeFi Research
- Creating low-liquidity experimental pools  
- Studying price discovery in AMMs  
- Simulating wrapped-token arbitrage patterns  
- Testing the effect of ultra-low supply on volatility  

### ► Wallet Price Chart Experiments
MetaMask, Coinbase Wallet, and many portfolio trackers use CoinGecko/CMC as their backends.  
The token is suitable for analyzing:

- chart indexing behavior  
- update intervals  
- price aggregation from DEX liquidity  
- volatility propagation from WBTC/WETH pairs  

### ► Wrapped-Asset Modeling
BTC/USDT can simulate:

- pseudo-BTC behavior,  
- synthetic BTC representations,  
- micro-liquidity wrapped tokens,  
- cross-DEX arbitrage flows.

---

## Adding BTC/USDT to MetaMask

1. Open **MetaMask** and select **Ethereum Mainnet**.  
2. Click **Import Tokens** → **Custom Token**.  
3. Paste the contract address:


