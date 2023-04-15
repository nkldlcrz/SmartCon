# Creating-and-Deploying-a-Contract-
// SPDX-License-Identifier: MIT 
pragma solidity 0.8.18; 

contract FEU {
    
    string public tokenName =
    "FEU Token";
    string public tokenSymbol=
    "FEU";
    uint totalSupply = 0;

    mapping(address => uint)
    public balances;

    function mint(address _address,uint _amount) public
     {
        totalSupply +=_amount;
        balances[_address] +=
        _amount;
        
    }
    function burn(address _address,uint _amount)public
     {
        totalSupply -= _amount;
        balances[_address] -= 
        _amount;
    }
}
