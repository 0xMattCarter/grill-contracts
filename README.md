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
  - gas cost at 40 gwei: 

## Burger Deployment:
  - tokenURI: baselink.com/{}.json
  - grill2 address: < grill2 addr >
  - gas cost at 40 gwei:

## Metabull Deployment:
  - tokenURI: baselink.com/ (post reveal will be: baselink.io/<>.json)
  - burger address: < burger addr >
  - grill2 address: < grill2 addr >
  - * Need to replace erc721a.sol and ierc721a.sol in .deps
  - gas cost at 40 gwei: 
  
  
## Phybull Deployment:
  - vault address: < receiver of erc20 >
  - erc20 address: 0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48 (USDC)
  - burger address: < burger addr >
  - grill2 address: < grill2 addr >
  - gas cost at 40 gwei: 
 
  
# Test deploys:
  - Grill2: https://goerli.etherscan.io/address/0x5d84968d70f3bc98840ca37178c261fc0368e7fd
  - Burger: https://goerli.etherscan.io/address/0x23726589ce342c2f3064a7611df2771c16e63fe5
  - Metabull: https://goerli.etherscan.io/address/0x89c21ce749f5b9dfcf74d79276ee6ce8e507d4b7
  - Phybull: https://goerli.etherscan.io/address/0x6a6ee18e688d2df3f7b843185290445a582269b0
