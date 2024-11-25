# ETHAVAX2

This is a user-friendly Web3 application developed with HTML, CSS, and Solidity. It utilizes the Ethereum network to offer a decentralized banking experience. Through this dApp, users can effortlessly deploy contracts, transfer Ether, and customize their account names. The app is powered by Solidity smart contracts, the robust Ethers.js library, and integrates with the convenient MetaMask wallet extension.

## Installation

2. Install the dependencies by running `npm install`.
3. Start the local blockchain using Hardhat by running `npx hardhat node`.
4. Open new terminal and deploy the Bank contract `npx hardhat run --network localhost scripts/deploy.js`.
5. Start the development server by running `npm run dev`.

### Configure MetaMask to use the Hardhat node

1. Open the MetaMask extension in your browser.
2. Click on the account icon in the top right corner and select "Settings".
3. In the "Networks" tab, click on "Add Network".
4. Fill in the following details:
   - Network Name: hardhat-test-network
   - RPC URL: http://127.0.0.1:8545/
   - Chain ID: 31337
   - Currency Symbol: GO or ETH
5. Click on "Save" to add the Hardhat network to MetaMask.
   
> If you need detailed instructions or visual guidance, you can refer to this step-by-step guide on [how to use MetaMask with a Hardhat node](https://support.chainstack.com/hc/en-us/articles/4408642503449-Using-MetaMask-with-a-Hardhat-node).

### Add accounts using private keys by Hardhat for testing 🔑

1. In the MetaMask extension, click on the account icon in the top right corner.
2. Select "Import Account" or "Import Account using Private Key" (depending on your version of MetaMask).
3. In the "Private Key" field, enter one of the private keys provided by Hardhat.
   - To access the list of private keys, open the terminal where you started the Hardhat local network.
   - The private keys are displayed as part of the accounts generated by Hardhat.
4. Click on "Import" to import the account into MetaMask.
5. Repeat the above steps to add more accounts for testing purposes.

## Usage

**To use the Ethers Bank application, follow these instructions:**

1. After installing MetaMask and connecting it to the Ethereum network, connect your wallet to the application.
2. The application will automatically display your Ethereum account and balance.
3. To transfer funds, fill in the recipient's Ethereum address and the amount of ETH you want to transfer.
4. Click the "Transfer" button to initiate the transaction.
5. Confirm the transaction in MetaMask.
6. The transaction will be processed, and the account balance will be updated accordingly.

**You can also update your account's name:**

1. The owner's name is displayed once connected, which can be fetched from the contract.
2. You can view the contract owner’s address alongside your own account information.
3. If the name is missing, the contract is still loading the data.

**You can also update your account's name:**

1. Ensure that both the recipient's address and transfer amount fields are filled correctly.
2. The transaction will be initiated on the blockchain after the "Transfer" button is clicked.
3. Monitor the transaction in MetaMask for confirmation and successful transfer.

## Authors

Metacrafter John Alvin R. Cruz

## License

This project is licensed under the MIT License - see the LICENSE.md file for details
