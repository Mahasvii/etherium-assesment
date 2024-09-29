# BETA Token Contract

This is a simple ERC-20-like token contract written in Solidity that defines a basic token called "BETA" with the symbol "BTA". The contract allows minting and burning of tokens.

## Features

- **Token Name**: BETA
- **Token Symbol**: BTA
- **Total Supply**: The contract keeps track of the total supply of tokens.
- **Mint Function**: Allows minting of new tokens by increasing the total supply.
- **Burn Function**: Allows burning tokens by decreasing the total supply if the user has enough balance.

## Functions

- **Mint**: 
  - Adds tokens to a specified address.
  - Increases the total supply.
  - Updates the balance of the specified address.

- **Burn**: 
  - Removes tokens from a specified address, provided it has a sufficient balance.
  - Decreases the total supply.
  - Updates the balance of the specified address.

## How to Deploy the Contract on Remix

1. **Open Remix**:
   - Visit [Remix IDE](https://remix.ethereum.org/) in your web browser.

2. **Create a New File**:
   - In the left-hand panel, click on the **"Contracts"** folder.
   - Click the **"+"** button to create a new file.
   - Name the file, for example, `BETA.sol`.

3. **Paste the Solidity Code**:
   - Open the newly created file and paste your Solidity code for the BETA token contract.

4. **Compile the Contract**:
   - Click on the **"Solidity Compiler"** tab (the tab with a “compiler” icon on the left-hand panel).
   - Select the appropriate Solidity compiler version (choose `0.6.12` or later but below `0.9.0` as specified in your contract).
   - Press the **"Compile BETA.sol"** button. If there are no errors, the contract will successfully compile.

5. **Deploy the Contract**:
   - After compiling, click on the **"Deploy & Run Transactions"** tab (the tab with a “Ethereum” icon).
   - Under **Environment**, choose the network you want to deploy to:
     - **JavaScript VM**: This is a local blockchain instance running in your browser. It's good for testing.
     - **Injected Web3**: Use this if you want to deploy to a live network like Ropsten or Ethereum mainnet using MetaMask.
     - **Web3 Provider**: For connecting to a custom network (e.g., an external Ethereum node).
   - In the **Account** dropdown, select the account (wallet) you want to use for deployment.
   - Press the **Deploy** button below the contract.

6. **Confirm Deployment**:
   - If you are using **Injected Web3** (like MetaMask), you will need to confirm the transaction in your wallet.
   - After confirming, wait for the contract to be deployed. Once deployed, the contract will appear under **Deployed Contracts** at the bottom of the same tab.

7. **Interacting with the Contract**:
   - After deploying, you can interact with your contract directly from the **Deployed Contracts** section:
     - **Mint Tokens**: Call the `mint` function by entering an address and the amount of tokens.
     - **Burn Tokens**: Call the `burn` function by entering the address and the amount to burn.
     - **Check Balances**: You can input an address in the `balances` field to check how many tokens the address holds.
     - **Check Total Supply**: Call the `total_supply` variable to see the current total supply of tokens.

## Requirements

- Solidity version: `>=0.6.12 <0.9.0`
- Remix IDE or another Solidity development environment.
- A wallet like MetaMask if deploying to a testnet or mainnet.

### Author

This contract was developed by **Mahasvi**.


