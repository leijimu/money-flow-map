# money-flow-map
Open-source map of global money networks and financial infrastructure.
开放的全球资金网络与金融基础设施关系地图。

## Network Map

```mermaid
flowchart LR

CN["中国大陆银行"]
HK["香港银行"]
MO["澳门银行"]
OS["国外银行"]

PAY["微信 / 支付宝"]

CEX["加密货币交易所"]

USDT["USDT"]
USDC["USDC"]

WALLET["数字钱包"]
CHAIN["区块链"]

WISE["Wise"]

UCARD["U卡"]

CN --> HK
CN --> MO

CN --> PAY

HK --> OS
MO --> OS

OS --> CEX

CEX --> USDT
CEX --> USDC

USDT --> WALLET
USDC --> WALLET

WALLET --> CHAIN

USDT --> UCARD
USDC --> UCARD

OS --> UCARD
HK --> WISE
WISE --> CEX
