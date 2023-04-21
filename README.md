# Smart Contract

The Artify token was designed to represent the concepts gained through this course. This will be an initial token example in which we will use the 
Cryptography basic concepts, blockchain, and solidity.

## Description

Artify token is an example of a smartcontract written in Solidity. This smartcontract will carry out the essential operations of this token, such as mapping, minting, and burning. Artify token will be my first initiative, serving as the initial stage in accomplishing my Web3 objective.

## Getting Started

### Installing

* Like the other smart contracts on the blockchain. The Artify coin will be run at Remix or Remix IDE https://remix.ethereum.org/ 
which is a no-setup tool with an intuitive user interface for writing smart contracts.
*  To execute this code, the user must first provide the licensing identification, followed by the IDE's version: 

### Executing program

# Creating-and-Deploying-a-Contract-
// SPDX-License-Identifier: MIT 
pragma solidity 0.8.18; 

contract Artify {
    
    string public tokenName =
    "Artify Token";
    string public tokenSymbol=
    "Artify";
    uint totalSupply = 0; public

    mapping(address => uint)
    public balances;

    function mint(address _address,uint _amount) public
     {
        totalSupply +=_amount;
        balances[_address] += _amount;
         
    }
    function burn(address _address,uint _amount)public
       if (balances[_address] >= _amount) {
        totalSupply -= _amount;
        balances[_address] -= 
        _amount;
       }
    }
}




Once the token has been run, test it by hitting the "Deploy & run transactions" button on the left side panel. Continue by selecting "Artify Token" from the "Contract" section and pressing "deploy" after that. Finally, run all of the functions. 


```

## Authors

Bautista, Nicole D. 

@8210179@ntc.edu.ph


## License

This project is licensed under the [MIT] License - see the LICENSE.md file for details
