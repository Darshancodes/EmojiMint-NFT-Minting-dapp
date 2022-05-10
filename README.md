# EmojiMint - NFT Minting dapp

This is EmojiMint - A fullstack NFT minting dApp. Emojiint is built with the purpose of providing an entry point for future NFT Minting dapps.

# Installation
You can either use the default EmojiMint smart contract and play with it or you can also put your own smart contract and make changes as needed. *Remember to change ```.env``` file with your own variables*.

**Use the default Smart Contracts**:
```
git clone https://github.com/Darshancodes/Emojimint.git
cd Emojimint
npm install
npm run dev
```

**To use your own Smart Contracts**:

- Change ```.env``` with your own environment variables.
- Remove ```/artifactsfolder``` if it exists.
- Put your own smart contract inside ```/contracts/```.
- Compile your smart contract with ```npx hardhat compile```.
- Update ```/scripts/deploy.js``` according to your needs.
- Deploy your smart contract with ```npx hardhat run``` ```scripts/deploy.js --network rinkeby```.
- Copy the deployed contract address and put it inside ```/utils/interact.js``` ```contractAddress``` section.
