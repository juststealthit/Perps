# Glossary

| Term | Meaning |
| --- | --- |
| **Borrow fee** | Jupiter's charge for holding a position, in place of funding. It builds up while the position is open |
| **Collateral** | What backs a Jupiter position: the coin itself for a long, USDC for a short. Paid in SOL from your wallet |
| **Cross margin** | One balance backs every position in the account. Gains in one help the others, and losses in one can use the whole balance. Hyperliquid positions opened here use cross margin |
| **Enable trading** | The one-time Hyperliquid setup: a trading key for this browser and an approval so orders can be placed from this site |
| **Entry price** | Your average price into the position |
| **Funding** | A payment between longs and shorts that keeps a perp's price near the spot price. Positive: longs pay shorts. Negative: shorts pay longs. Hyperliquid charges it every hour, Aster every 8 hours |
| **Isolated margin** | Each position has its own margin, and only that margin is at risk. Jupiter positions work this way |
| **Leverage** | How much bigger the position is than your margin. $100 at 10x is a $1,000 position, and a 1% move is $10 |
| **Limit order** | An order at your price. It waits on the book until it fills or you cancel it |
| **Liquidation** | The venue closing a position whose margin can no longer cover its loss. The margin is lost |
| **Liquidation price** | The price at which that happens. An estimate on the Hyperliquid ticket, the venue's own figure under Positions |
| **Margin** | The money behind a position. On the ticket it's the amount you enter |
| **Mark price** | The venue's fair price for a perp, used for PnL and liquidation. It can differ a little from the last trade |
| **Market order** | An order that fills now at the best price available, within a slippage limit |
| **Notional** | The full value of a position: margin × leverage. The ticket shows it next to Size |
| **Open interest** | The value of all open positions in a market |
| **Perp, perpetual** | A futures contract with no expiry. You go long or short on a coin's price without holding the coin |
| **Perps balance** | Your Hyperliquid account value, including open PnL |
| **PnL** | Profit and loss. Unrealized while the position is open, realized once closed |
| **Reduce-only** | An order that can only shrink a position, never open or flip one. **Close** on Hyperliquid uses it |
| **Relay** | The bridge that moves deposits from Solana or an EVM chain into Hyperliquid |
| **Slippage** | The gap between the price you saw and the price you got |
| **Spot** | Buying or selling the coin itself, with no leverage or funding |
| **Trading key** | A key kept in your browser that your wallet approved on Hyperliquid. It can place and cancel orders and set leverage. It can't withdraw |
| **Venue** | The exchange that runs a market and holds its positions: Hyperliquid, Jupiter Perps or Aster |

## Cross and isolated

| | Cross | Isolated |
| --- | --- | --- |
| Margin | Shared by every position in the account | Kept per position |
| What a liquidation can take | Up to the whole account balance | That position's margin |
| Liquidation price | Depends on every position and your balance | Depends on that position only |
| Here | Hyperliquid perps | Jupiter Perps |

The Hyperliquid ticket's **Liq. price (est.)** treats the position as if it stood alone. Under cross margin your real liquidation price moves with the rest of your account.
