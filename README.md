# Project Create a Token
 Creating a simple token contract in Solidity, Where we see balance, mint and burn tokens.

 Metacrafters ETH PROOF: Beginner EVM Course Final Assessment.
 This Solidity contract provides a basic implementation of a token contract with two functions i.e. mint and burn. This allows the users to create and destroy tokens while maintaining the total supply and balances of the individuals.

# Details:
This Solidity smart contract is designed to complete these requirements ->
1. Token Details: This contract uses some variables with public access specifiers to store the information about the token. These variables are- tokenName, tokenAbbrv and totalSupply.
2. Balances addressing: In this contract, we are using a mapping named 'balances' to map the address to their token balance.
3. Mint Function: This function has two parameters- an address and a value. This function increases the total token supply by the value given in the parameter and then updates the balance of the sender's address accordingly.
4. Burn Function: This function also uses two parameters same as the mint function but it works opposite to the mint function. This function is used to burn or destroy the total supply by the given value and update the balance of the individual accordingly.
5. Condition check: With this condition we are allowing the 'burn' function to burn the token if the sender's balance is greater than or equal to the number of tokens to be burned.
6. In code the initial supply is given 0 tokens, So make sure first use the mint function before calling burn at the first instance.

# What I have done in this code:
1. Deployed the MyToken contract on Ethereum Virtual Machine (EVM) having the solidity compatible version(0.8.9).
  
2. use the two functions for interacting with the contract:
   
       -mint(address _address, uint _value)
   here the '_address' parameter is denoting the recipient's address and the '_value' parameter represents the token amount to be minted. This function increases or mints new tokens with a given value by increasing the total supply and the balance at the particular address.

       -burn(address _address, uint _value)
    here the '_address' parameter is denoting the sender's address and the '_value' parameter represents the token amount to be burned.
    The function burn the tokens from the total supply and also deducts the balance of the sender's address. Also, it uses a condition to do so, if the sender's balance is   below the need, nothing will happen.
 
        mapping(address => uint) balances
   Using balances[_address] we can access the balance of that address.

3. access the public variables:

>   tokenName: Gives the name of the token.

>   tokenAbbrv: Gives the abbreviation of the token.

>   totalSupply: Gives the total supply of the token.


   <a href="https://www.loom.com/share/7e8205feb6334d78a9aea185478036e6">
    <p>A Walkthrough of Creating a Simple Token 🚀 - Watch Video</p>
    <img style="max-width:300px;" src="https://cdn.loom.com/sessions/thumbnails/7e8205feb6334d78a9aea185478036e6-with-play.gif">
    </a>
    

  

# License
This project is licensed under the MIT License. 
You can find this in the code as "SPDX-License-Identifier: MIT" with a comment(//) ahead in the first line of code.

