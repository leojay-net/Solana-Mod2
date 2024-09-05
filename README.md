# Solana Wallet Application

This React application demonstrates basic interactions with the Solana blockchain, specifically focusing on creating wallets, connecting to the Phantom wallet, and transferring SOL between wallets.

## Features

1. **Create a New Solana Account**: Generates a new Solana account (sender wallet) and airdrops 2 SOL into it on the Devnet.
2. **Connect to Phantom Wallet**: Allows users to connect their Phantom wallet to the application.
3. **Transfer SOL**: Enables the transfer of SOL from the created sender wallet to the connected Phantom wallet.
4. **Disconnect Wallet**: Provides the ability to disconnect the Phantom wallet from the application.

## How It Works

1. The application uses the `@solana/web3.js` library to interact with the Solana blockchain.
2. It connects to the Solana Devnet cluster for testing purposes.
3. When creating a new Solana account, it generates a new keypair and requests an airdrop of 2 SOL.
4. The Phantom wallet connection is handled through the browser's `window.solana` object.
5. SOL transfers are executed using Solana's `SystemProgram.transfer` instruction.

## Key Components

- `createSender()`: Creates a new Solana account and airdrops 2 SOL into it.
- `connectWallet()`: Prompts the user to connect their Phantom wallet.
- `disconnectWallet()`: Disconnects the Phantom wallet from the application.
- `transferSol()`: Transfers 0.01 SOL from the sender wallet to the connected Phantom wallet.





