# Safety and risk

## Who holds what

| | Held by |
| --- | --- |
| Your Hyperliquid account and positions | Hyperliquid, under your own EVM address |
| Your Jupiter positions | Jupiter Perps on Solana, owned by your Solana address |
| Your wallets' keys | You |
| The Hyperliquid trading key | Your browser |
| Money in flight during a deposit | Relay, until it's credited or refunded |

Just Stealth It doesn't hold your perps money or your positions. It shows the venues' markets and builds orders that your wallet, or the trading key your wallet approved, signs in your browser. The order goes to the venue, and the venue fills it.

## What the site can and can't do

| It can | It can't |
| --- | --- |
| Read public market data and your accounts from the venues | Withdraw from your Hyperliquid account |
| Ask your wallet to sign an approval, a deposit or a Jupiter trade | Sign anything with your wallet without your approval |
| Place, cancel and close Hyperliquid orders with the trading key in your browser, when you press the button | Use the trading key to move or withdraw funds. Hyperliquid doesn't allow it |
| | Undo a trade or a liquidation |

The venues run their own systems. If a venue is down or refuses an order, the site shows the venue's reason. If Hyperliquid's or Jupiter's own app works and this page doesn't, you can manage the same positions there.

## Risks

- **Leverage cuts both ways.** At 10x, a 10% move against you is about 100% of your margin. Fees and funding make it sooner.
- **Liquidation.** If the price reaches your liquidation price, the venue closes the position and you lose the margin in it. On Hyperliquid, cross margin means losses can use the rest of your account's balance too.
- **Estimates are estimates.** The ticket's Hyperliquid liquidation price and fees are estimates. Prices can gap past them.
- **Funding and borrow fees** are charged while a position is open, and can add up over days.
- **Slippage.** Market orders can fill worse than the price you saw, within the limits on [the ticket page](order-ticket.md#market-and-limit).
- **Venue and bridge risk.** Hyperliquid, Jupiter, Aster and Relay are separate systems with their own risks.
- **Charts can differ.** The TradingView chart may come from another source than the venue. See [Charts](charts.md#tradingview).
- **Where you live.** Perpetuals are not available in every country. Check your local rules.

Only trade what you can afford to lose. Nothing here is financial advice or a promise of any return.

## Staying safe

- Nobody from Just Stealth It will ever ask for your recovery phrase.
- Support is only the form on [juststealthit.xyz/status](https://juststealthit.xyz/status). Automated accounts on X and Telegram aren't support.
- Check the address bar says `juststealthit.xyz` before you connect a wallet.
- Read every wallet prompt before you sign.

Next: [FAQ](faq.md)
