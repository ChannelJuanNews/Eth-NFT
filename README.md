# How to NFT 

There are many different steps we need ot take to take to mint and NFT, but roughtly we can outline 5 major steps with several micro steps we need to take to create a custom eth wallet & NFT minter. 

1. First, we must have a mechanism to create, read & update ethereum accounts/wallets. This is where the [`web3`] \(https://web3py.readthedocs.io/en/stable/) via `wallet.create`. This API will come in handy since it natively allows us to create wallets & manage their private keys via our web application interface (chrome extension).
We will integrate via the IPFS protocol to host metadata associated with the NFT image https://ipfs.io/
2. Once we create a wallet for a user, we want to be able to deliver the NFT image to that particular wallet using Solidity smart contracts.  
3. Once we are able to manage a wallet directly, along with the private key, we will want to work with the `brownie` library to write Solidity smart contracts that allow us to create ERC-721 compliant smart contracts on the fly for sponors & investors 
4. Execute the smart contract to generage an NFT via the eth network 
5. Retrieve the NFT via the `web3` python/javascript package. 

Additional abillities 
1. Can view on opensea 
2. Can view on etherscan 

Started code https://github.com/eth-brownie/brownie
