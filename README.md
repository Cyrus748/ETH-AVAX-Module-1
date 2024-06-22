# ETH-AVAX-Module-# Transaction Contract

#### Overview

This repository contains a Solidity smart contract for a basic ERC20 token called `MyToken`. The contract provides functionalities for minting new tokens, burning existing tokens, and transferring tokens between addresses.

#### Contract Details

- **Contract Name**: `MyToken`
- **Version**: Solidity 0.8.26

#### Key Features

1. **Token Details**
   - **Name**: "AdityaToken"
   - **Symbol**: "ADT"
   - **Total Supply**: Initialized to 0 and increases with minting.

2. **Owner**
   - The contract is owned by the deployer (`msg.sender` at deployment).

3. **Events**
   - `Mint`: Triggered when tokens are minted.
   - `Burn`: Triggered when tokens are burned.
   - `Transfer`: Triggered when tokens are transferred between addresses.

4. **Modifiers**
   - `onlyOwner`: Restricts access to functions only to the owner of the contract.

5. **Functions**
   - `constructor()`: Initializes the contract and sets the deployer as the owner.
   - `mint(address _address, uint _value)`: Allows the owner to mint new tokens and allocate them to a specific address.
   - `burn(address _address, uint _value)`: Allows the owner to burn (destroy) tokens from a specific address.
   - `transfer(address _receiver, uint _value)`: Allows any address to transfer tokens to another address, provided they have sufficient balance.

6. **Errors**
   - `InsufficientBalance`: Custom error thrown when attempting to burn tokens from an address with insufficient balance.

#### Deployment

To deploy the `MyToken` contract:
- Use Solidity version 0.8.26 or compatible.
- Ensure to set the SPDX license identifier appropriately for your use case.

#### Usage

1. **Minting Tokens**
   - Only the owner can mint new tokens using the `mint` function.

2. **Burning Tokens**
   - Only the owner can burn tokens from any address using the `burn` function.

3. **Transferring Tokens**
   - Any address can transfer tokens using the `transfer` function, provided they have enough tokens.

#### Testing

- Test the contract thoroughly for different scenarios such as minting, burning, transferring tokens, and handling errors like insufficient balances.

#### License

This contract is provided under an unlicensed SPDX-License-Identifier. Modify the license identifier as per your requirements.

#### Author

- Replace this section with your details if you are the author of the contract.

#### Disclaimer

- Include any necessary disclaimers or notices pertinent to the usage or deployment of the contract.

#### Support

- Provide information on how users can get support or report issues related to this contract.

---

Feel free to customize this README file according to your specific deployment details, authorship, and any additional information relevant to your use case.


## Author

Aditya Negi

[Linkedin](https://www.linkedin.com/in/adityanegi748)
