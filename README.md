# SimpleCryptoKitties

This project is a simplified version of the popular CryptoKitties game, implemented using Solidity and the ERC-721 standard. It is a guided project of the ***Complete Ethereum learning track*** by HackQuest.

## Overview

**SimpleCryptoKitties** allows users to create and breed digital cats (Kitties) with unique genetic codes. Each Kitty is an ERC-721 non-fungible token (NFT), meaning it is unique and can be owned and traded on the Ethereum blockchain.

### Features

- **Generation 0 Kitties**: Two Kitties are automatically created upon contract deployment.
- **Breeding**: Users can breed their Kitties to create new ones with unique genetic codes.
- **ERC-721 Compliance**: Each Kitty is a unique token that follows the ERC-721 standard, ensuring compatibility with other platforms and marketplaces.

## Contract Details

### Solidity Version

The contract is written in Solidity `0.8.17` and uses OpenZeppelin's ERC-721 implementation for NFT functionality.

### Main Components

- **Kitty Struct**: Represents a Kitty with properties such as `genes`, `birthTime`, `momId`, `dadId`, and `generation`.
- **Mapping of Kitties**: All Kitties are stored in a mapping where the key is the token ID and the value is the Kitty struct.
- **_createKitty**: A private function to create new Kitties.
- **createKittyGen0**: A private function that creates Generation 0 Kitties.
- **breed**: A public function that allows users to breed two Kitties they own, producing a new Kitty.

### Dependencies

This project uses OpenZeppelin's ERC-721 implementation:

