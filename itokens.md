## How are iTokens generated?

When a vault user deposit USDC/USDT/DAI/yCRV/ETH or other assets into the YFII Vault, iTokens of the corresponding currency will be generated and issued to this user. For instance, if you recharge the vault with USDC, you get iUSDC.


## What does iToken stand for?

iToken can be understood as the equity Token of the YFII Vault, representing your equity share in the Vault. Taking USDC as an example, you can get slightly less than 1000 iUSDC by depositing 1000 USDC. If the current price is 1 iUSDC = 1.01 USDC, then you can mint 1000/1.01 = 990 iUSDC. If there are 99,000 iUSDCs distributed for the entire USDC Vault, it means you own 1% of the total USDC in this vault.


## Why does the value of iTokens increase automatically?

Because YFII Vault uses a lossless strategy for the principal, the revenue of the target farming pool will automatically be converted to the vault's Token and returned to the vault, while the number of iTokens remains unchanged. In this way, the iToken for the vault can be exchanged for more Tokens, resulting in an increase in the price of iToken.


## Are there any other ways to get iToken?

In addition to participating in the YFII Vault, i.e., depositing Token to generate iToken, you can also purchase iTokens directly through DEX like Uniswap. According to YFII YIP-5, 5% of the Vault's profit will be sent to the recursive farming pool. This part of YFII rewards should incentivize iUSDT/USDT, iUSDC/USDC, iDAI/DAI and iETH/ETH, iBTC/wBTC and other trading pairs. Users farm this recursive pool by collateralizing the UNI_LP of these trading pairs to yield additional YFII. There will be trading pairs with sufficient liquidity to support users to use YFII's business by just purchasing iTokens.


## What is the role of iToken?

The most important role of iTokens is to prevent the outflow of funds that have entered the YFII Vault. When the user needs funds, they don't need to withdraw their principal from the Vault (currently a 0.2% withdrawal fee is applied). They may choose to directly trade their iTokens for Tokens on Uniswap. The value of iToken will always be higher than the original Token, but the growth rate of the price may slow down later, because the more funds in the vault, the more diluted APY there will be. The 0.2% withdrawal fee is designed to prevent the whale from diluting the APY on the one hand, and the other function is to lock in more AUM (Assets Under Management).


## What does iToken/Token market making bring?

1. Because the exchange rate of iToken/Token changes very slowly, the impermanent loss of the market maker is expected to be controlled within a very low range. If Balancer supports iTokens, we can even get BAL as additional rewards.

2. It creates a convenient way for users to participate in YFII's business. Purchasing iTokens will just do the work, which saves gas fees that would otherwise be higher when depositing funds in Vault.

3. There will always be a price gap between the minting of iTokens through vaults and the purchase of iTokens. When someone buys iToken in large quantities through DEXes, the price of iToken rises, and arbitrageurs will mint iTokens and inject trading pair's liquidity pool to smooth out the arbitrage space. These processes will generate more iTokens, which is conducive to expanding the AUM of the YFII Vault.


## What businesses can be derived from iToken?

1. Because the iToken/Token exchange rate will always be higher than 1, consider adding leverage for lending. Mortgage iToken in the lending platform that supports iToken, and then borrow Token at a 1:1 ratio.

> A specific example: With 1000 USDC diposited into YFII Vault, you can get 990 iUSDC, and then take 990 iUSDC to the lending platform for mortgage to borrow out 990 USDC; once again deposit 990 USDC in the Vault, exchange for 980 iUSDC, and then perform the mortgage lending...
>
> According to this cycle, users can get leveraged assets that are multiple times to the principal for financial management, though it requires sufficient USDC on the lending platform. This process is equivalent to users moving USDC from the DeFi market to the YFII platform, thereby increasing YFII's AUM.

2. The yCRV system of Curve creates two parts of income: yToken's automatic optimization of lending income, and curve's exchange fee. Similarly in YFII, the three assets of iUSDC/iUSDT/iDAI can be synthesized into iCRV, which not only enjoys the income of iToken's automatic yield farming strategy, but also collects the stable currency swap fee from Curve or other stablecoin AMM platforms. iTokens and iCRV will also have multiple possibilities of combination with other DeFi projects in the future.


## What are the benefits of iToken to YFII token price?

The YFII Vault is characterized by recursive yield farming (with compound interests). 10% of the profit generated by all Vault managed funds will be used to repurchase YFII and sent to development funds, insurance funds, etc.

The former strategy of the Vault was using 100% of revenue to repurchase YFII, which is only effective when the AUM is small; the new strategy of YFII Vault increases the value of YFII by bringing up the total AUM, so even 10% for repurchase of YFII is a very large sum of money.

iTokens represent the scale of YFII managed funds. The larger the issuance of iTokens, the more profit the Vault will obtain, which will drive 10% of YFII repurchase to increase the token price. Therefore, all these iTokens of YFII serve to increase the price of YFII.