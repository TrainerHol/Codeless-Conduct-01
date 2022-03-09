# Open Track: Tokenomics

A design for a novel token distribution mechanism for gamified NFT's. 

## Introduction

A lot of gamified systems that use ERC-20 token emissions as rewards tend to have a high decline in token value as time goes by, even if there are use cases that reduce the supply. This design aims to explore and prototype a system that increases liquidity permanently and tries to model emissions by time since minting. This system doesn't go into specifics in terms of utility/gamification as it is meant to be a broad system that could be applied to any project and tweaked to each team's needs.

## Permanent Liquidity Minting

A common cause for big price changes is lack of liquidity. The less liquidity a token has, the easier it is for the price to change. 

To start, we will categorize the NFT's in two different categories:
**Starter NFT's**: The NFT's minted initially in the collection/game.
**Secondary NFT's**: The subsequent NFT's that can only be minted using the emitted ERC-20.

### Point System for Minting
The token minting will require an auction-style bidding system that will mint token for the *n* highest bidders, with *n* being the total initial supply for the minting.

The bids will have thresholds that determine the number of points. For example, having a 0.1 ETH threshold for the project would mean that if someone bid 1 ETH, they would get 10 points.

|Amount| Points |
|--|--|
| 1 ETH |10 points  |

### Permanent Liquidity Locking
After the bids have been paid, the model would emmit an arbitrary number of tokens proportional to the number of total points across all the bids. This number of tokens would then be permanently locked into LP tokens.

It is important to note that in order to have less fluctuation in the price, it's necesssary to have this locked supply be much larger than the projected emission amount in a period of time that is long enough for all the game/utility functions to be fully implemented.

## Emission Model
The emission model must be projected in a way that the users can profit from the emissions based on the initial investment during the starter minting. The ERC-20 emissions would work in a way that the user is rewarded tokens proportionally to the point system of each token that was given during the minting phase. 
There would be a daily emission pool and it would be divided among all the point holders.

For example, for a 100 daily token pool:

| NFT ID | Points  |Daily Emission|
|--|--|--|
|#1  |4  |40	|
|#4 | 6 | 60|


 For this, the secondary NFT minting functionality can be useful, as it gives a basic use case for the ERC-20 besides selling. 

The secondary NFT's would also emit the token, but at a much lower rate than the base ones.
The secondary emission could be calculated by having a flat 5-10% of the daily pool divided by all the secondary token holders. This would make holding a secondary NFT still profitable. 

## Secondary Minting & Other Utility Costs
The secondary minting (and other gamified utilities made by the team) should have a growth-based cost system. This means that the more NFT's are minted, the higher the minting price becomes. This would make the token price more resistant to inflation as it would cost more the more tokens there are.

Each time a token is minted or utility action is performed, the tokens use would be burned permanently to reduce the supply.

The increase could be a 5% increase (this % can be tweaked to change the projected # of NFT's) after each mint/utility action. Meaning that if it costs 10 tokens to mint the first NFT, it would cost 10.5 tokens to mint the second one, and so on.

To avoid extremely high prices eventually making the game unplayable, utility action costs should also deflate over time. This can be achieved by having an "inflation counter" and comparing timestamps to reduce the counter every once in a while. 
