# Introduction 

[credits](https://github.com/liquity/dev/tree/main#liquity-overview). 

## Salient points  : 


- The protocol  algorithmically controls the generation of LUSD based on underlying ether 

- uses decentralized data feed for price management  and liquidates the  pool having Collectorization ration less than defined parameter.

- Machanisms to consider :
    - liquidation mechanisms . 
    - management of the stablity pool. 
    - LiqUSD token redemption. 
    - core smart contracts explained [here](https://github.com/liquity/dev/tree/main#liquity-overview).




- recently being audited by [ToB](https://github.com/trailofbits/publications/blob/master/reviews/Liquity.pdf). 

## contracts under consideration . 


- the contracts are written  in solidity 0.6.11  version .
    - no inhereted bugs in the given version . 


description  on the diffrent contracts which will be tested :  
- LPRewards : 
    -  Unipol.sol : an modified  version  from [synthetix contract](https://sips.synthetix.io/sips/sip-31) , which makes the process of LP completely onchain . 

- LQTYStaking.sol : fora staking / unstaking of the holders of token  by getting the fees from ETH / debt issuance. 

- CommunityIssuance.sol : for issuance of LQTY tokens to stablity providers based on defined timeline .

