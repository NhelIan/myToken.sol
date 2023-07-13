# # TOKEN Creation

This project is a simple token contract implementing the following:

Minting new tokens
Burning tokens
Transferring tokens between accounts

## Description

The project is a simple token contract that can be used to create, burn, and transfer tokens. The contract is implemented in Solidity and can be compiled and deployed using a web3 development environment. The token contract can be used for a variety of purposes, such as creating a new cryptocurrency, implementing a loyalty program, or creating a crowdfunding platform. Some of the key features of the token contract are:

The contract allows the owner to mint new tokens.
The contract allows the owner to burn tokens.
The contract allows users to transfer tokens to each other. The token contract is a valuable tool for anyone who wants to create or use decentralized applications. It is easy to use and provides a variety of features that can be used to implement a variety of applications.

## Getting Started
Installing
To run this program, you can use Remix, a web-based Solidity IDE. To get started, head to the Remix website at https://remix.ethereum.org/. Once you're on the Remix website, create a new file by clicking the "+" icon in the left-hand sidebar. Save the file with a .sol extension, such as MyToken.sol.
### Executing program

The contract has three public variables: tName, tAbrv, and totSupply.
The contract also has a mapping variable called balances.
The contract has two functions: mint() and burn().
The mint() function mints new tokens and the burn() function burns tokens.

    */

      contract MyToken {
    // public variables here
    string public tokenName = "CABAYAO";
    string public tokenAbbry = "CBO";
    uint public totalSupply = 0;

    // mapping variable here
    mapping(address =>uint) public balances;

    // mint function
    function mint (address _address, uint _value) public{
        totalSupply += _value;
        balances[_address]+= _value;
    
    }
     // burn function
     function burn (address _address, uint _value) public{
    if (balances[_address] >= _value) {
        totalSupply -= _value;
        balances[_address]-= _value;
    }
     }
    }

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.4" (or another compatible version), and then click on the "Compile myToken.sol" button.

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "myToken" contract from the dropdown menu, and then click on the "Deploy" button.

Once the contract is deployed, first put a value then copy the account address. Next is going to the mint function by pasting the account adress that you copy.Put a value in mint function then transact. Next step is checking the balance.After that we can now test the program that you created.


## Authors

Cabayao, Nhel Ian (National Teachers College)


## License

This project is licensed under the MIT License - see the LICENSE.md file for details

This Solidity program is a simple "Hello World" program that demonstrates the basic syntax and functionality of the Solidity programming language. The purpose of this program is to serve as a starting point for those who are new to Solidity and want to get a feel for how it works.

