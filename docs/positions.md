# Positions and orders

Under the chart are three tabs: **Positions**, **Orders** and **History**. The tab shows a count when there's something in it.

They read your accounts on every venue you have a wallet connected for. Hyperliquid refreshes about every 5 seconds, Jupiter about every 6.

## Positions

Every open position on Hyperliquid and Jupiter, together. Each row has the venue's logo.

| Column | What it shows |
| --- | --- |
| Coin | The coin, its venue, the side and the leverage, such as Long 10x |
| Size | The position's value in USD |
| Entry | Your average entry price |
| Liq. price | The venue's own liquidation price |
| PnL | Unrealized profit or loss in USD, and as a percent of margin |
| Close | Closes the whole position at market |

On a phone a row shows the coin, its PnL and **Close**. Size, entry and liquidation price show on wider screens.

On Jupiter, PnL is shown after Jupiter's fees.

### Closing

**Close** closes the whole position at market. Partial closes aren't on the page yet.

| Venue | What Close does | Signed by |
| --- | --- | --- |
| Hyperliquid | A reduce-only market order for the full size | The trading key in this browser. No wallet prompt |
| Jupiter | A full close. You're paid back in SOL | Your Solana wallet. You approve it |

You need the venue's wallet connected to close: the EVM wallet for Hyperliquid, the Solana wallet for Jupiter. You'll see **Position closed** once it's done.

You can also close a Hyperliquid position on Hyperliquid's own app, or a Jupiter position on Jupiter's. They're the same positions.

## Orders

Your open Hyperliquid limit orders: coin, side, size and price. **Cancel** removes one from the book, signed by the trading key. You'll see **Order cancelled**.

Jupiter orders here fill straight away, so they never rest.

## History

Your last 50 Hyperliquid fills: coin, buy or sell, size and price, realized PnL where the fill closed something, and the time.

Jupiter trades don't show in History yet. Jupiter's own app has your full Jupiter history.

## Nothing showing?

| You see | Why |
| --- | --- |
| No open positions | None open, or the venue's wallet isn't connected |
| A position you opened elsewhere | Expected. Positions opened on Hyperliquid's or Jupiter's own app show here too, for the same wallet |
| A Hyperliquid position, but no Close works | Connect the EVM wallet that owns it and **Enable trading** in this browser |

Next: [Deposits and withdrawals](deposits-and-withdrawals.md)
