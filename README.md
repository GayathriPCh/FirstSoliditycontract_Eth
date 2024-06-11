## FirstSoliditycontract_Eth
Writing my first Solididty smart contract on Ethereum, from Metaschool

# Setup
- Install and set up Metamask account.
- Set up the Sepolia testnet environment.
- Fetch some testnet eth.
- Set up Hardhat project.
- Set up environment variables.

# Creating the contract
- Wrote some solidity code after creating a HelloWorld.sol .
- Added sepolia to the hardhat project via Alchemy

# Deployment
- Wrote a deployment script
- Ran the script using
  	```
      npx hardhat compile
   	```
  	```
      npx hardhat run scripts/deploy.js --network sepolia
   	```
# Interacting with the contract
- Created interact.js
- Ran it with
   	```
    npx hardhat run scripts/interact.js --network sepolia
  	```

    Output:
  	```
   the message is Hello World! Bingo
   the new message is Good Bye, World!
   	```
# Conclusion: 
The purpose of interacting with the deployed contract is to demonstrate two key functionalities of smart contracts:
- Reading Data: The script retrieves the current message stored on the blockchain using the message() function of the contract. This showcases how users can interact with a deployed contract to access information stored on it.
- Updating Data: The script goes beyond just reading data and also modifies the message stored on the blockchain. It calls the update() function with a new message "Good Bye, World!" and waits for the update to be confirmed on the network. This demonstrates how smart contracts can be used to manage and update data in a secure and transparent way.
