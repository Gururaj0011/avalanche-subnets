**ERC20 and Vault Contracts README**

This repository contains Solidity smart contracts for ERC20 tokens and a vault contract to manage and secure those tokens. Below, you'll find an overview of each contract, instructions for deployment, and basic usage guidelines.

### ERC20 Contract
The ERC20 contract implements the standard interface for fungible tokens on the Ethereum blockchain. It allows for the creation and management of tokens following the ERC20 standard specifications.

#### Features:
- Minting new tokens.
- Transferring tokens between addresses.
- Approving and transferring tokens on behalf of another address.
- Checking balances of addresses.

#### Deployment:
1. Compile the ERC20.sol file using a Solidity compiler like Remix or Truffle.
2. Deploy the compiled contract to an Ethereum network of your choice (e.g., Mainnet, Ropsten, Rinkeby).

### Vault Contract
The Vault contract serves as a secure storage facility for ERC20 tokens. It implements additional features to enhance security and control over the stored tokens.

#### Features:
- Depositing ERC20 tokens into the vault.
- Withdrawing ERC20 tokens from the vault.
- Transfer of tokens from the vault to specified addresses.
- Admin functionalities for pausing/unpausing deposits and withdrawals.
- Emergency withdrawal functionality in case of critical situations.

#### Deployment:
1. Compile the Vault.sol file along with ERC20.sol using a Solidity compiler.
2. Deploy both the ERC20 and Vault contracts to an Ethereum network.

### Usage:
1. **Deploy Contracts:** Deploy ERC20 and Vault contracts to the desired Ethereum network.
2. **Interact with ERC20 Contract:** Use the ERC20 contract to mint tokens, transfer tokens between addresses, approve token transfers, etc.
3. **Deposit Tokens into Vault:** Use the deposit function of the Vault contract to deposit ERC20 tokens into the vault.
4. **Withdraw Tokens from Vault:** Authorized addresses can withdraw tokens from the vault using the withdraw function.
5. **Transfer Tokens from Vault:** Authorized addresses can transfer tokens from the vault to specified addresses using the transferFromVault function.
6. **Admin Controls:** The admin of the Vault contract can pause/unpause deposits and withdrawals as needed. In case of emergencies, the emergencyWithdraw function allows for immediate withdrawal of all tokens from the vault.

### Security Considerations:
- Ensure that only trusted parties have administrative access to the Vault contract.
- Regularly audit the contracts for any potential vulnerabilities.
- Exercise caution when interacting with smart contracts, especially when dealing with large sums of tokens.

### Disclaimer:
These contracts are provided as-is, without any guarantees of functionality or security. Use them at your own risk.

### License:
This code is licensed under the [MIT License](LICENSE).

## Author

Gururaj Mahansheetar

Thank you for using our ERC20 and Vault contracts! We appreciate your interest and feedback.
