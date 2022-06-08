# -BSC-Universal-dividend-token

Full functioning

All tokens except bnb that support Binance Chain, such as ETH/DOGE/USDT, etc.

One-click to set the amount of coins that can receive dividends, and the dividend interval

Add whitelist and block addresses in batches

Set the proportion of dividends, return, marketing and destruction of buying and selling with one click

Compilation/Open Source Notes

COMPILER: v0.8.7+commit.e28d00a7.js

Enable optimization: enable and use the default value of 200

Other Settings: default evmVersion, MIT license

Deployment parameters

The contract selects the Blocktechnology contract for deployment, and the Value value is 200000000000000000 (17 0s, 0.2BNB)

name_: token name
symbol_: token symbol
totalSupply_: supply volume
rewardAddr_: The contract of the dividend token, note that it must be on the Binance Chain
marketingWalletAddr_: Marketing Wallet, own
serviceAddr_: 0x7Ea95D639c59E5E0Dd4b7f4d62b5558933a84Fd9 (mainnet dependent contract)
buyFeeSetting_: [X,X,X,X] (X is a number, that is, a percentage, corresponding to dividends, liquidity, marketing, combustion, refer to [1,1,1,2])
sellFeeSetting_: [X,X,X,X] Same as above
tokenBalanceForReward_: How many tokens are held to participate in the dividend, the unit is wei, so add 18 0s after the number

Testnet related parameters
Pancake test network routing, source code line 676: 0xB6BA90af76D139AB3170c7df0139636dB6120F7e
Testnet usdt: 0xEdA5dA0050e21e9E34fadb1075986Af1370c7BDb
Testnet SHIB: 0x11e815a78Cc41D733Db00f06B3A96074855362CE
Testnet dependent contract: 0x72519BE1b6fcd1493378e38628ba60Dc34DeB41f
When adding liquidity (adding a pool), pay attention to adding it with bnb, because the transaction pair of the source code is bnb and the deployed token
