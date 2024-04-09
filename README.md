# Crypto Wallet Tracker Bot

## Introduction

The Crypto Wallet Tracker Bot is a Telegram bot that allows users to monitor their Ethereum (ETH) and Binance Smart Chain (BNB) wallet transactions in real-time. Users can add their wallet addresses to the bot, and it will send them notifications whenever incoming or outgoing transactions occur on their wallets.

## Features

- **Real-time Transaction Monitoring**: The bot continuously monitors user-specified wallet addresses and sends notifications for incoming and outgoing transactions.
- **Supports Ethereum and Binance Smart Chain**: Users can monitor wallets on both Ethereum and Binance Smart Chain blockchains.
- **Telegram Integration**: Notifications are sent directly to users via Telegram, making it convenient to stay updated on wallet activities.

## Installation

To use the Crypto Wallet Tracker Bot, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/crypto-wallet-tracker-bot.git
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Create a `.env` file and add your Telegram bot token:

   ```bash
   TELEGRAM_BOT_TOKEN=<your_telegram_bot_token>
   TELEGRAM_CHAT_ID=<your_telegram_chat_id>
   ```

4. Obtain API keys from Etherscan and BscScan for Ethereum and Binance Smart Chain respectively, and replace `<your_etherscan_api_key>` and `<your_bscscan_api_key>` in the code with your actual API keys.

5. Run the bot:

   ```bash
   python bot.py
   ```

## Changes and Fixes

- **Improved Code Readability**: Refactored the code to improve readability and maintainability.
- **Added Environment Variables**: Utilized environment variables for sensitive information such as API keys and Telegram bot token.
- **Enhanced Error Handling**: Implemented better error handling mechanisms to gracefully handle exceptions and errors.
- **Updated Dependency Management**: Included `python-dotenv` for managing environment variables more effectively.
- **Fixed API Key Handling**: Revised the code to properly handle API keys for different blockchains.

## Usage

1. Start the bot by sending the `/start` command to initiate the bot and get instructions on how to use it.

2. Add a wallet to monitor using the `/add <blockchain> <wallet_address>` command. For example:

   ```
   /add ETH 0x123456789abcdef
   ```

   Replace `ETH` with the blockchain (either `ETH` for Ethereum or `BNB` for Binance Smart Chain), and `0x123456789abcdef` with the wallet address you want to monitor.

3. Remove a wallet from monitoring using the `/remove <blockchain> <wallet_address>` command. For example:

   ```
   /remove ETH 0x123456789abcdef
   ```

   Replace `ETH` with the blockchain and `0x123456789abcdef` with the wallet address you want to stop monitoring.

4. List all wallets being monitored for a specific blockchain using the `/list <blockchain>` command. For example:

   ```
   /list ETH
   ```

   Replace `ETH` with the blockchain you want to list wallets for.

## Contributing

Contributions are welcome! If you find any bugs or have suggestions for improvements, feel free to open an issue or submit a pull request. Email : Ashik@Spudblocks.com
