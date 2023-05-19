# MyToken Smart Contract  
  The MyToken smart contract is a basic implementation of a token contract on the Ethereum blockchain. It allows for minting and burning tokens, as well as tracking token balances and total   supply.
## Contract Details  
  The smart contract consists of the following functionalities:  
  •	Token Details: The contract includes public variables tokenName and tokenAbbrv to store the name and abbreviation of the token, respectively. The totalSupply variable keeps track of the     total number of tokens in circulation.  
  •	Token Balances: The contract uses a mapping balances to associate addresses with their respective token balances. The balance of each address can be accessed using the address as the         key.  
  •	Mint Function: The mint function allows the contract owner to mint new tokens and assign them to a specified address. It takes two parameters: _address, which represents the address to       receive the tokens, and _value, which specifies the amount of tokens to be minted. The function increases the total supply by the minted amount and updates the balance of the recipient       address accordingly.  
  •	Burn Function: The burn function enables the contract owner to burn tokens. It accepts two parameters: _address, representing the address from which the tokens will be burned, and           _value, indicating the amount of tokens to be burned. Before deducting the tokens, the function checks if the balance of the sender address is greater than or equal to the specified         amount. If the condition is met, the function deducts the tokens from the total supply and updates the balance of the sender address.  
## Usage  
  To use the MyToken smart contract:  
  1.	Compile the contract using a Solidity compiler (e.g., solc).  
  2.	Deploy the contract to the Ethereum network using your preferred deployment method (e.g., Remix, Truffle, or web3.js).  
  3.	Once deployed, you can interact with the contract functions:  
  •	To mint new tokens, call the mint function, providing the recipient's address and the amount of tokens to be minted.  
  •	To burn tokens, call the burn function, specifying the sender's address and the amount of tokens to be burned. Ensure that the sender's balance is sufficient to perform the burn               operation.  
  Remember to handle proper access control and security considerations when using and deploying smart contracts in production environments.  
## Author  
  Atharv Kumar Gupta  
## License  
  The MyToken smart contract is licensed under the MIT License. You can find the license text in the SPDX-License-Identifier comment at the beginning of the contract code.  

