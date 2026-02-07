<p align="center">
  <img src="resources/img/logo.png" width="130" alt="TON Galaxy Logo">
</p>

<div align="center">

# Awesome TON

</div>

<p align="center">
  <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="Awesome"></a>
  <br><br>
  <i>A curated list of awesome TON (The Open Network) contracts and apps</i>
</p>

---

## Contents

- [📜 Contracts](#contracts)
  - [🪙 Jetton](#jetton)
  - [🖼 NFT](#nft)
  - [👛 Wallets](#wallets)
  - [🔄 DEX](#dex)
  - [🏦 Lending & Borrowing](#lending--borrowing)
  - [🥩 Staking](#staking)
- [📱 Apps](#apps)
  - [👛 Wallets](#wallets-1)
  - [💱 Exchanges](#exchanges)
  - [🔍 Blockchain Explorers](#blockchain-explorers)
  - [🖼 NFT](#nft-1)
  - [🚰 Faucets](#faucets)
- [🤝 Contributing](#contributing)

## <a id="contracts"></a> 📜 Contracts

### <a id="jetton"></a> 🪙 Jetton

- **Jetton** - implementation of [TEP-74](https://github.com/ton-blockchain/TEPs/blob/0d7989fba6f2d9cb08811bf47263a9b314dc5296/text/0074-jettons-standard.md), a fungible token standard, serving as TON equivalent to Ethereum's ERC-20 tokens. Used for custom currencies, stablecoins (e.g., [USDT](https://tonviewer.com/EQCxE6mUtQJKFnGfaROTKOt1lZbDiiX1kCixRv7Nw2Id_sDs)) and memecoins (e.g., [UTYA](https://tonviewer.com/EQBaCgUwOoc6gHCNln_oJzb0mVs79YG7wYoavh-o1ItaneLA))
    - [**Tact reference implementation**](https://github.com/tact-lang/jetton)
    - [**FunC reference implementation**](https://github.com/ton-blockchain/jetton-contract)

- [**Mintless Jetton**](https://github.com/ton-blockchain/mintless-jetton-contract) - implementation of [TEP-177](https://github.com/ton-blockchain/TEPs/pull/177/changes) - mintless version of Jetton; enables Merkle-proof airdrops & minting of Jettons directly on the Jetton-Wallet contract in a decentralized manner

- [**zkJetton**](https://github.com/zk-examples/zkJetton) - a minimal version of a jetton contract for the TON blockchain that uses zk-SNARKs to provide hidden balances and private transfer amounts functionality. In other words, it's a Zcash (ZEC)-like anonymous currency token for the TON blockchain

- [**Jetton with governance**](https://github.com/ton-blockchain/stablecoin-contract) - a version of the Jetton contract, developed for centralized stablecoins (e.g., [USDT](https://tonviewer.com/EQCxE6mUtQJKFnGfaROTKOt1lZbDiiX1kCixRv7Nw2Id_sDs?section=code)). Non-compliant with the original Jetton TEP due to requirements for centralized stablecoins that conflict with the original standard (e.g., no user-initiated token burning, a governance mechanism that allows performing any action on other Jetton wallets, etc.)

### <a id="nft"></a> 🖼 NFT

- **NFT** - implementation of [TEP-62](https://github.com/ton-blockchain/TEPs/blob/63fc78718dd9930f3e106954ebec743c3ad07993/text/0062-nft-standard.md), a non-fungible token standard, serving as the TON equivalent of Ethereum's ERC-721 tokens. Used for custom NFTs (e.g., meme collections like [Plush Pepes](https://tonviewer.com/EQBG-g6ahkAUGWpefWbx-D_9sQ8oWbvy6puuq78U2c4NUDFS?section=overview), digital assets like [Telegram Usernames](https://tonviewer.com/EQCA14o1-VWhS2efqoh_9M1b_A9DtKTuoqfmkn83AbJzwnPi?section=overview), real-world assets (RWAs), etc.)
    - [**FunC reference implementation**](https://github.com/ton-blockchain/nft-contract)

- [**NFT Bundle**](https://github.com/1IxI1/NFT-Bundle) - a contract that enables you to own and transfer several NFT items as a single package

- [**TON DNS for .ton domains**](https://github.com/ton-blockchain/dns-contract) - implementation of [TEP-81](https://github.com/ton-blockchain/TEPs/blob/63fc78718dd9930f3e106954ebec743c3ad07993/text/0081-dns-standard.md). Used for resolving .ton domain names, which are represented on-chain as NFTs (e.g., [TON DNS Names](https://tonviewer.com/EQC3dNlesgVD8YbAazcauIrXBPfiVhMMr5YYk2in0Mtsz0Bz?section=code))

### <a id="wallets"></a> 👛 Wallets

- [**Wallet v5**](https://github.com/ton-blockchain/wallet-contract-v5) - v5 of one of the most common user wallet contracts. Among the improvements: support for sending up to 255 messages at once, reduced network fees, and unlimited extensions

- [**Wallet v4**](https://github.com/ton-blockchain/wallet-contract) - v4 of one of the most common user wallet contracts. Main improvement over the v3 and older versions - support for plugins that enable easy extension of the wallet functionality

### <a id="dex"></a> 🔄 DEX

- **STON.fi** - core contracts for the STON.fi DEX protocol, including pool, router, and liquidity provider-related contracts
    - [**STON.fi DEX core v1**](https://github.com/ston-fi/dex-core)
    - [**STON.fi DEX core v2**](https://github.com/ston-fi/dex-core-v2)

### <a id="lending--borrowing"></a> 🏦 Lending & Borrowing

- [**EVAA Protocol**](https://github.com/evaafi/contracts) - a decentralized lending platform that enables users to lend and borrow digital assets without the need for a central intermediary

### <a id="staking"></a> 🥩 Staking

- [**Native staking**](https://github.com/ton-blockchain/nominator-pool) - the official TON Foundation standard for pooling funds to run a Validator. Since running a validator requires a massive amount of TON, this contract allows a "Pool Owner" (who has the hardware) to accept TON from "Nominators" (regular users) to meet the requirement

- [**Tokamak Network v2**](https://github.com/tokamak-network/ton-staking-v2/tree/ton-staking-v2) - a liquid staking implementation. In native staking, your TON is "locked" and inaccessible. This protocol takes your TON, stakes it in a validator, and gives you a "receipt token" in return, which enables liquidity of the staked share

## <a id="apps"></a> 📱 Apps

### <a id="wallets-1"></a> 👛 Wallets

- [**MyTonWallet**](https://mytonwallet.io/) - an open-source, audited, self-custody mobile wallet for TON and TRON with support for tokens and NFTs. Security-focused with a commitment to zero user tracking and no data selling. On-ramping (debit/credit cards)

- [**Tonkeeper**](https://tonkeeper.com/) - a self-custody mobile wallet. Supports TON, Jetton-based tokens and NFTs. On-ramping (debit/credit cards)

- [**Wallet**](https://t.me/wallet) - custodial and self-custody TON wallet, integrated into Telegram. The custodial version supports management of SOL, ETH, BTC and other cryptocurrencies. On/Off ramping (e.g., debit/credit cards). P2P market.

### <a id="exchanges"></a> 💱 Exchanges

- [**STON.fi**](https://ston.fi/) - cross-chain native asset DEX with own security protocol built on TON Blockchain. DEX on TON is live, cross-chain is coming soon

- [**DeDust.io**](https://dedust.io/) - AMM DEX based on TON with a wide variety of listed tokens

- [**Storm Trade**](https://storm.tg/) - decentralized leveraged trading DEX that supports trading of various asset types (Cryptocurrencies, Stock, Forex and Commodities)

### <a id="blockchain-explorers"></a> 🔍 Blockchain Explorers

- [**Tonviewer**](https://tonviewer.com/) - a feature-rich blockchain explorer specifically designed for TON

- [**DYOR.io**](https://dyor.io/) - trust scores, charts and analytics for TON-based assets

### <a id="nft-1"></a> 🖼 NFT

- [**getgems.io**](https://getgems.io/) - NFT marketplace with a wide selection of NFT collections

- [**Fragment**](https://fragment.com/) - NFT marketplace, mainly focusing on Telegram-based assets (e.g., usernames, anonymous Telegram phone numbers, gifts, stars, etc.)

### <a id="faucets"></a> 🚰 Faucets

- [**Testgiver TON Bot**](https://t.me/testgiver_ton_bot) - faucet on the TON Test network. As of February 2026, provides 2 TON per request with a waiting window of 1-2 hours

## <a id="contributing"></a> 🤝 Contributing

Know a project that deserves to be on this list? We'd love your input! Open an [issue](../../issues/new) with the name, link, and a short description of the service you'd like to suggest, and we'll review it for inclusion.
