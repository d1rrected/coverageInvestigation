# Giveth Contracts test coverage analysis
---
## Overall
| Contract | Coverage | Comment |
| --- | --- | --- |
| PermittableToken | 0% | **Not covered by tests** |
| MerkleDistro | 13% | **Only constructor covered** |
| UnipoolTokenDistro | 68.66% | Most critical functions are covered |
| GardenUnipoolTokenDistributor| 74.19% | **withdraw** and _onTransfer (copypaste from 1Hive) not covered |
| GIVBacksRelayer | 100% | Covered |
| TokenDistro | 90.91% | Covered |
| GIV | 54.35% | **burn**, **transferFrom** and **transferWithAuthorization** not covered |

---
## Details
### PermittableToken - **0%**
#### Not covered
---
### MerkleDistro - **13%**
#### Only constructor covered.
---
### UnipoolTokenDistro - **68,66%**
| Function | Covered |
| --- | --- |
| onlyRewardDistribution | true |
| updateReward | true |
| initialize | true |
| lastTimeRewardApplicable | true |
| rewardPerToken | true |
| notifyRewardAmount | ~50% |
| setRewardDistribution | true |
| stakeWithPermit | false |
| getSelector | false |
| _permit | false |
| _getBlockTimestamp | false |
---
### GardenUnipoolTokenDistributor - **74.19%**
| Function | Covered |
| --- | --- |
| onlyRewardDistribution | true |
| updateReward | true |
| lastTimeRewardApplicable | true |
| rewardPerToken | true |
| getTimestamp | true |
| earned| true |
| claimableStream| true |
| stake| true |
| withdraw| **false** |
| getReward| true |
| _getReward| true |
| notifyRewardAmount| true |
| setRewardDistribution| true|
| _onTransfer| **30%** |
---
### GIVBacksRelayer - **100%**
| Function | Covered |
| --- | --- |
| initialize | true |
| addBatch | true |
|addBatches | true |
|executeBatch | true |
|hashBatch | true |
|isPending | true |
---
### TokenDistro - **90.91%**
| Function | Covered |
| --- | --- |
| initialize | true |
| setStartTime | false |
| assign| true |
| claimTo| false |
| claim | true |
| _allocate | true |
| _allocateMany | true |
| allocateMany | true |
| sendGIVbacks | true |
| changeAddress| true |
| getTimestamp | true |
| globallyClaimableAt | true |
| claimableAt | true |
| claimableNow | true |
| cancelAllocation | true |
| _claim| true |
---
### GIV - **54.35%**
| Function | Covered |
| --- | --- |
| _validateSignedData | true |
| _changeMinter | true |
| _burn| false |
| _approve | true |
| _transfer | true |
| getChainId| true |
| getDomainSeparator | true |
| mint| true |
| changeMinter | false |
| burn| **false** |
| approve | false |
| transfer | true |
| transferFrom | **false** |
| transferWithAuthorization | **false** |


