# Pre-Deployment

## First:
  - make new workspace
  - delete default contracts
  - paste in Grill2.sol, Burger.sol, Metabull.sol, PhysicalBull.sol
  - open .deps/npm/erc721a/contracts/
  -   - replace code for erc721a.sol and ierc721.sol from this repo

## Next:
  - set compiler to 0.8.9
  - enable gas optimization (200)

## Finally, 
  - change environment to 'injected web3'
  - verify account/balance/chainId

# Deployment
Deploy each contract in order using the following parameters


## Grill Deployment:
  - grill1 address: 0xE11AF478aF241FAb926f4c111d50139Ae003F7fd
  - gas cost at 40 gwei: 0.07543624

## Burger Deployment:
  - tokenURI: baselink.com/{}.json
  - grill2 address: < grill2 addr >
  - gas cost at 40 gwei: 0.0799362

## Metabull Deployment:
  - tokenURI: baselink.com/ (post reveal will be: baselink.io/<>.json)
  - burger address: < burger addr >
  - grill2 address: < grill2 addr >
  - * Need to replace erc721a.sol and ierc721a.sol in .deps
  - gas cost at 40 gwei: 0.08037496
  
  
## Phybull Deployment:
  - vault address: < receiver of erc20 >
  - erc20 address: 0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48 (USDC)
  - burger address: < burger addr >
  - grill2 address: < grill2 addr >
  - gas cost at 40 gwei: 0.04133816

# Gas Usage
Assuming 40 gwei:
  - grill2: 0.07543624
  - burger: 0.0799362
  - metabull: 0.08037496
  - phybull: 0.04133816
  - total: 0.27708556

# Setting Proxy
- Step 1: setProxyRegistry(), function 15 @ https://etherscan.io/address/0x71B11Ac923C967CD5998F23F6dae0d779A6ac8Af#writeContract
  - address: 0x90DD49e039B6C1343cDd59c7032c51a9f769823F
- Step 2: setProxyForAccount(), function 10 @ https://etherscan.io/address/0x90dd49e039b6c1343cdd59c7032c51a9f769823f#writeContract
  - account: 0xE11AF478aF241FAb926f4c111d50139Ae003F7fd
  - operator: 0x90DD49e039B6C1343cDd59c7032c51a9f769823F
  
# Live deploys:
  - Grill2: https://goerli.etherscan.io/address/
  - Burger: https://goerli.etherscan.io/address/
  - Metabull: https://goerli.etherscan.io/address/
  - Phybull: https://goerli.etherscan.io/address/


