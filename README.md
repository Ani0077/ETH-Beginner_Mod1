SportsContract
Overview
The SportsContract is a simple Solidity smart contract designed to manage a token with minting and burning functionalities. This contract includes public variables to store the token details such as the token name, abbreviation, and total supply. Additionally, it maintains a mapping to keep track of the balances of different addresses.

Features
Token Details:
Public variables to store the token name, abbreviation, and total supply.
Balance Mapping:
A mapping of addresses to their respective balances.
Mint Function:
A function to increase the total supply of tokens and the balance of a specified address.
Burn Function:
A function to decrease the total supply of tokens and the balance of a specified address.
Includes conditional checks to ensure the balance of the address is sufficient before burning the tokens.
Contract Details
State Variables
string public tokenName = "Football ";
The name of the token.
string public tokenAbbr = "FS";
The abbreviation of the token.
uint public totalSupply = 110;
The total supply of the token.
Mapping
mapping(address => uint) public balances;
A mapping to store the balance of each address.
