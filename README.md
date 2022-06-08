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

 
  
# Test deploys:
  - Grill2: https://goerli.etherscan.io/address/0x708790Ca15B5D7aa4797225F05d301A1586E7867
  - Burger: https://goerli.etherscan.io/address/0x324DE66f43535e1469d050F67ceBE99b82C99a25
  - Metabull: https://goerli.etherscan.io/address/0x1eBFb398991e5c49f3DE9424672b0f2De64af6Cc
  - Phybull: https://goerli.etherscan.io/address/0x0430a09Eb345A9D925897c210654640866Ba67C7
