# Relations

## Fiat

| From | Relation | To | Asset | Region |
|---|---|---|---|---|
| CNY | FX | HKD | CNY/HKD | CN/HK |
| CNY | FX | USD | CNY/USD | CN/GLOBAL |
| HKD | FX | USD | HKD/USD | HK/GLOBAL |
| USD | FX | EUR | USD/EUR | GLOBAL/EU |

## Banking

| From | Relation | To | Region |
|---|---|---|---|
| CN | BANKING | HK | CN/HK |
| HK | BANKING | US | HK/US |
| HK | BANKING | EU | HK/EU |
| HK | BANKING | SG | HK/SG |

## Financial Services

| From | Relation | To |
|---|---|---|
| HK | SERVICE | WISE |
| EU | SERVICE | N26 |
| SG | SERVICE | IFAST |

## Exchange

| From | Relation | To |
|---|---|---|
| USD | FIAT_ACCESS | COINBASE |
| USD | FIAT_ACCESS | KRAKEN |
| USD | FIAT_ACCESS | BITGET |
| EUR | FIAT_ACCESS | COINBASE |
| EUR | FIAT_ACCESS | KRAKEN |

## Stablecoin

| From | Relation | To |
|---|---|---|
| COINBASE | TRADE | USDC |
| COINBASE | TRADE | BTC |
| COINBASE | TRADE | ETH |
| KRAKEN | TRADE | USDC |
| KRAKEN | TRADE | BTC |
| KRAKEN | TRADE | ETH |

## Blockchain

| Asset | Network |
|---|---|
| USDC | Ethereum |
| USDC | Solana |
| USDC | Base |
| USDC | Arbitrum |
| USDC | Optimism |
| USDC | Avalanche |
| USDT | Ethereum |
| USDT | Tron |

## Wallet

| From | Relation | To |
|---|---|---|
| USDC | ONCHAIN_TRANSFER | WALLET |
| USDT | ONCHAIN_TRANSFER | WALLET |
| BTC | ONCHAIN_TRANSFER | WALLET |
| ETH | ONCHAIN_TRANSFER | WALLET |

## Card

| From | Relation | To |
|---|---|---|
| UCARD | NETWORK | VISA |
| UCARD | NETWORK | MASTERCARD |

## Payment

| From | Relation | To |
|---|---|---|
| WECHAT | PAYMENT | MERCHANT |
| ALIPAY | PAYMENT | MERCHANT |
| VISA | PAYMENT | MERCHANT |
| MASTERCARD | PAYMENT | MERCHANT |
| APPLEPAY | PAYMENT | MERCHANT |
