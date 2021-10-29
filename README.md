# BLOCKCHAIN based Reviews & Rewards System
*DApp to create a platform for Reviews & Rewards System on Ethereum Framework.

# What it does:
* Any users, will be able to submit their reviews on any products/services.- They will be represented as Reviewers.
* Any users, who is reviewing those reviews & can up-vote or down-vote basis their opinions.
* If a reviews get Upvoted, then a minute fraction of ether(0.0001) will be transferred to "Original Reviewer" address. 
* If a reviews get DownVoted, then nothing happens, except downvote count get increases. If Downvote limit reaches more than 50, then "original reviewers" will be deducted the minuet fraction of ether..(Say - 0.00001)
* Reviewers cannot upvote/downvote their own reviews, which helps eliminate fake review counts

# STEPS to Install / Setup
1) Clone the repositories  using following command

2) do run "npm install" command to ensure node packages are up-to-date & in sync
3) Ensure you have "Ganache" & It is running status
4) Ensure you have "MetaMask" extensions added into chrome & enabled custom RPC to sync the accounts with Ganache
5) Using below command to deploy the contract into Ganache
   truffle migrate --network ganache --compile-all --reset
6) Setup IPFS locally and run the daemon to communicat with the public IPFS network
7) Once it is migrated successfully, run below command to launch the server
   npm run dev
8) You can add "reviews" using "add my review", choose file(photos) & upload. this will upload your pic in IPFS & return back the hash key, once it is showing succesuflly upload. Click submit to add your reviews into Blockchain.
9) Now, choose anotherr account in metamask, now you can see two button enabled (upvote/downvote). if reviews are upvoted, then original "reviews provider" will get some ether(0.0001) as rewards
910) if downvotes, same will be reduced from user account.

# Implementation:
* Developed using Solidity and web3.js
  * used node.js, web3 and solc compiler
  * used Remix for contract testing
  * Used truffle framework in order to the ease developement process
  * IPFS for decentralized storage
* Testing of smart contracts was done on 
  * Ganache (Private Local Blockchain)
* Javascript testing method used the Mocha framework
  
# Build With:
* Solidity,IPFS, MetaMask, Web3js, Truffle, Ganache, Shell script, EVM Framework. JQuery
