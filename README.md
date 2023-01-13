# ERC20-Access-Control


[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

This code is written in the Solidity for the Ethereum blockchain. It defines a smart contract called "DEVToken" which inherits functionality from several other contracts, including "ERC20" and "ERC20Burnable" for implementing token functionality, "Ownable" for controlling access to the contract, and "AccessControl" for managing roles and permissions.

The contract has a constructor function that takes in an address for a "minter" and assigns the "MINTER_ROLE" to that address using the _grantRole function. The contract also has a "mint" function, which allows the minter to mint new tokens and assign them to a specified address. The function first checks that the calling account has the minter role before proceeding with the minting of tokens, using the require(hasRole(MINTER_ROLE, msg.sender), "Caller is not a minter") and _mint(to, amount) function.

I've implemented this code assigning the "Minter" rol to other smart contract.

## License

MIT

