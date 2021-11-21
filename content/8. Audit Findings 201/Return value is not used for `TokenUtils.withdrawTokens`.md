
# 106 - [Return value is not used for `TokenUtils.withdrawTokens`](./Return%20value%20is%20not%20used%20for%20`TokenUtils.withdrawTokens`.md)

Return value is not used for `TokenUtils.withdrawTokens` The return value of `TokenUtils.withdrawTokens` which represents the actual amount of tokens that were transferred is never used throughout the repository. This might cause discrepancy in the case where the original value of `_amount` was `type(uint256).max`.


1. Recommendation: The return value can be used to validate the withdrawal or used in the event emitted
2. [ConsenSys's Audit of DeFi Saver](https://consensys.net/diligence/audits/2021/03/defi-saver/#return-value-is-not-used-for-tokenutils-withdrawtokens)


___
## Slide Screenshot
![106.png](../../images/8.%20Audit%20Findings%20201/106.png)
___
## Slide Text
- 
___
## References
- Youtube Reference
___
## Tags