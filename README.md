# Box to deploy smart contracts on Harmony One Testnet
## Version
Truffle v5.3.1 (core: 5.3.1)  
Solidity v0.5.16 (solc-js)  
Node v15.14.0  
Web3.js v1.3.5  
## Installation
1. ```git clone https://github.com/noahfigueras/one_hdwallet_boilerplate.git```  
2. export MNEMONIC='Your metamask mnemonic'
3. Set truffle-config.js with correct account funded in HDWalletProvider():    
```provider: () => new HDWalletProvider(
		mnemonic, 
		'https://api.s0.b.hm,
		1                //EX:(this is accounts[1] in metamask)
	),
   network_id: 1666700000,       // Harmony One's Testnet id shard 0		     
```  
4. ```truffle migrate --network testnet``` in order to deploy and you will be able to find the contract deployed in https://explorer.pops.one/#/  

