# Uniswap V2 Area

Code from [Uniswap V2](https://github.com/Uniswap/uniswap-v2-core/tree/27f6354bae6685612c182c3bc7577e61bc8717e3/contracts) with the following modifications.

1. Change contract version to 0.6.12 and do the necessary patching.
2. Change swap equation to allow only one swap per block per direction.
3. Change swap equation to require (`balance0` in excess of `reserve0`) * `balance1` >= (`reserve1` in excess of `balance1`) * `balance0` and (`balance1` in excess of `reserve1`) * `balance0` >= (`reserve0` in excess of `balance0`) * `balance1`.