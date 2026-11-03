# Venues

A venue is the exchange that runs a market and holds the positions. Perps shows three. Just Stealth It runs none of them.

| | Hyperliquid | Jupiter Perps | Aster |
| --- | --- | --- | --- |
| Chain | HyperCore, Hyperliquid's own chain | Solana | BNB Chain |
| Markets | Every listed perp, and spot pairs with trading in the last 24 hours | SOL, ETH and BTC perps | USDT-margined perps, including some stocks and commodities |
| Trading here | On | On | Coming soon |
| Wallet | EVM | Solana | — |
| Money | USDC in your Hyperliquid account | SOL from your wallet, each trade | — |
| Order types here | Market and limit | Market | — |
| Max leverage here | What Hyperliquid allows for that market | 100x | Up to 50x shown |
| Funding | Every hour | No funding. Jupiter charges borrow fees instead | Every 8 hours |
| Prices on this page | Live, over Hyperliquid's price stream | Refreshed about every 20 seconds | Refreshed about every 20 seconds |
| Positions on this page | Yes | Yes | — |

## Hyperliquid

Hyperliquid is an order book exchange on its own chain. Your account there is tied to your EVM address. You fund it with USDC, and every perp and spot order uses that balance.

On this site you trade Hyperliquid from an EVM wallet you connect. The wallet approves a trading key once, and that key signs your orders from then on. See [Wallets and approvals](wallets.md).

Hyperliquid is the first venue for every coin it lists. It usually has the deepest book.

## Jupiter Perps

Jupiter Perps runs on Solana. There's no account to fund. Each trade is paid in SOL from your wallet, and Jupiter swaps it into the collateral:

| Side | Collateral |
| --- | --- |
| Long | The coin itself: SOL, ETH or BTC |
| Short | USDC |

Each Jupiter position stands alone with its own collateral. Closing pays back in SOL.

Jupiter has no price candles of its own, so its chart is the same coin's Hyperliquid chart. The chart says so. See [Charts](charts.md).

## Aster

Aster's markets, prices, funding and charts are live on the page. Trading Aster from this site is coming soon. Until then the ticket shows "Aster trading opens soon. Its markets and prices are live."

Aster lists some stocks and commodities as perps. They show in the market list by their ticker.

## Fees

Each venue charges its own trading fees, and funding or borrow fees, at its own rates. Those rates change and can depend on your volume. Check them on the venue:

| Venue | Where its fees are listed |
| --- | --- |
| Hyperliquid | [hyperliquid.gitbook.io/hyperliquid-docs/trading/fees](https://hyperliquid.gitbook.io/hyperliquid-docs/trading/fees) |
| Jupiter Perps | [jup.ag/perps](https://jup.ag/perps) and [Jupiter's Perps docs](https://developers.jup.ag/docs/perps) |
| Aster | [docs.asterdex.com](https://docs.asterdex.com/) |

The ticket shows an estimated **Fees** line before you place an order. Deposits through Relay show their own cost in the quote. See [Deposits](deposits-and-withdrawals.md).

You also need a little SOL for Solana network fees when you trade Jupiter.

Next: [Wallets and approvals](wallets.md)
