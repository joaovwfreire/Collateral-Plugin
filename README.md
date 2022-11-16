# eToken-Fiat Collateral-Plugin

This collateral plugin implements the functionality to enable Euler Finance's lending pool assets (eTokens) to be utilized as collateral at the Reserve-Protocol.

{tok}: eUSDC/ eUSDT / eDAI

{ref}: USDC / USDT / DAI

{target}: USD

{UoA}: USD

It implements views of refPerTok, targetPerRef and strictPrice exchange rates in accord to [Writing Collateral Plugins](https://github.com/reserve-protocol/protocol/blob/master/docs/collateral.md).

## Lending Pool concerns

In addition to the stable-coin pegging status check implemented at [Curve's cTokens fiat collateral plugin](https://github.com/reserve-protocol/protocol/blob/master/contracts/plugins/assets/CTokenFiatCollateral.sol), Euler Lending requires a second approach in order to maintain funds safety.

To reach maximum capital efficiency and better overall returns, lending pools prioritize borrowing most of it's position.

In the banking industry, there has been cases in which this lead to vaults running out of liquidity, specially in a run-to-the-bank context. This is one of the many reasons that have brought legal regulators to implement minimum reserve ratios for a lending operation to be allowed.
For this specific motive, I've opted to account for reserve ratios as a pool's health metric.

### ReserveRatio 

Omitted 

## Contract Structure

Omitted

## Checklist
- [x] refPerToken()
- [x] strictPrice()
- [ ] ...


