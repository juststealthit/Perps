# Getting started

Open **Perps** from the side rail on a computer, or from the dock on a phone. The page opens on BTC.

What you can trade depends on the wallet you connect.

| You connect | You can trade |
| --- | --- |
| A Solana wallet | Jupiter Perps: SOL, ETH and BTC |
| An EVM wallet | Hyperliquid perps and spot |
| Both | Both. The Solana wallet can also pay for Hyperliquid deposits |
| No wallet | Nothing yet. Markets, prices and charts still load |

## Trade Jupiter from a Solana wallet

1. Connect a Solana wallet such as Phantom, Solflare or Backpack.
2. Open the market list and pick SOL, ETH or BTC. If the coin is on more than one venue, pick **Jupiter** in the venue switch.
3. Pick **Long** or **Short**.
4. Enter what you pay in **SOL** and set the leverage. Jupiter needs at least $10 of collateral.
5. Check **Size** and **Liq. price**, then press the button, for example **Long SOL 5x**.
6. Approve the trade in your wallet. The position shows under **Positions** once Jupiter fills it.

There's no deposit on Jupiter. Each trade is paid from your wallet, and closing pays back in SOL.

## Trade Hyperliquid from an EVM wallet

1. Connect an EVM wallet.
2. Pick a market. Hyperliquid is the first venue for every coin it lists.
3. Press **Deposit** and fund the account. You can pay in SOL from a Solana wallet, or in your EVM wallet's own coin. See [Deposits](deposits-and-withdrawals.md).
4. Press **Enable trading** and sign once or twice in your wallet. This is a one-time setup. It moves no funds and costs no gas. See [Approvals](wallets.md#one-time-approvals-on-hyperliquid).
5. Pick **Long** or **Short**, **Market** or **Limit**, enter an amount in USD and set the leverage.
6. Press the button. Orders after setup don't open a wallet prompt.

The button always shows the next thing that's missing: **Connect**, **Deposit**, **Enable trading**, then your order.

## Only a Solana wallet, and you want Hyperliquid

Today, connect an EVM wallet next to your Solana wallet and deposit SOL into it through Relay. The full path is in [Solana users on Hyperliquid](wallets.md#solana-users-on-hyperliquid).

Perps accounts for Solana wallets, so you won't need an EVM wallet, are coming soon.

## Share a market

The page address names the market, so you can bookmark or share it.

| Address | Opens |
| --- | --- |
| `juststealthit.xyz/perps?m=ETH` | ETH perps on the first venue that lists it |
| `juststealthit.xyz/perps?m=SOL&v=jupiter` | SOL perps on Jupiter |
| `juststealthit.xyz/perps?m=HYPE/USDC&k=spot` | The HYPE/USDC spot pair |

`m` is the coin, or the pair for spot. `k=spot` asks for spot. `v` is `hyperliquid`, `aster` or `jupiter`.

Next: [Venues](venues.md)
