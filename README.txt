### Cross-Chain NFT Minting with Chainlink Integration

This project consists of a series of Solidity smart contracts enabling NFT minting on a specific blockchain using the Chainlink Cross-Chain Interoperability Protocol (CCIP). These contracts are designed to mint NFTs on the Sepolia blockchain from other blockchains such as Fuji and Mumbai.

#### Contracts

1. **CrossDestinationMinter.sol**: This contract enables NFT minting on the Sepolia blockchain from a different blockchain using the CCIP. Each generated NFT represents the price of an asset on the source blockchain. The appearance of the NFT varies based on the background color and the facial expression of the emoji depending on the movement of the asset price.

2. **CrossSourceMinter.sol**: This contract is similar to the previous one but specifically designed for the Fuji blockchain. It allows minting NFTs on the Sepolia blockchain from the Fuji blockchain.

3. **CrossSourceMinterMumbai.sol**: Similar to the previous contract, but designed for the Mumbai blockchain. It facilitates minting NFTs on the Sepolia blockchain from the Mumbai blockchain.

4. **CrossSourceMinterSepolia.sol**: This contract allows minting NFTs on the Sepolia blockchain from the Sepolia blockchain itself. The functionality is similar to the previous contracts but is designed for cases where NFTs need to be minted directly from the source blockchain.

#### Functionality

- **NFT Minting on Sepolia from other blockchains**: Each smart contract enables users to mint NFTs on the Sepolia blockchain from other blockchains using the Chainlink CCIP.

- **Visual Representation of Asset Price**: The appearance of the generated NFT varies based on the movement of the asset price. If the price goes up, the emoji's face will be happy, and the NFT's background will be green. If the price goes down, the emoji's face will be sad, and the NFT's background will be red. If the price remains unchanged, the emoji's face will be normal, and the NFT's background will be blue.

#### Usage

1. Deploy the corresponding contract on the specific blockchain according to the contract you are using (Fuji, Mumbai, or Sepolia).
2. Configure the contract with the address of the minting contract on the Sepolia blockchain.
3. Use the functions provided by the contract to mint NFTs on Sepolia from the source blockchain.
4. Observe the visual representation of the asset price on the minted NFTs.
