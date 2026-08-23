# Money Network Map

Open-source map of global money networks and financial infrastructure.

开放的全球资金网络与金融基础设施关系地图。

> 本项目用于金融基础设施与资金网络的可视化研究。
> 图中的连接表示概念上的网络关系，不代表特定机构、账户或产品一定支持该路径。
> 具体业务能力、地域限制、监管要求及服务条款应以相关机构官方信息为准。

---

## Network Overview

```mermaid
flowchart LR

%% =========================================================
%% Money Network Map
%% V0.1
%% =========================================================

%% -------------------------
%% Fiat
%% -------------------------

subgraph FIAT["法币体系"]

    CNY["CNY 人民币"]
    HKD["HKD 港币"]
    USD["USD 美元"]
    EUR["EUR 欧元"]

end


%% -------------------------
%% Banks
%% -------------------------

subgraph BANKS["银行体系"]

    CN_BANK["中国大陆银行"]

    HK_BANK["香港银行"]

    MO_BANK["澳门银行"]

    US_BANK["美国银行"]

    EU_BANK["欧洲银行"]

    SG_BANK["新加坡银行"]

end


%% -------------------------
%% Financial Services
%% -------------------------

subgraph SERVICES["金融服务"]

    WISE["Wise"]

    N26["N26"]

    IFAST["iFast"]

end


%% -------------------------
%% Payment
%% -------------------------

subgraph PAYMENT["支付体系"]

    WECHAT["微信支付"]

    ALIPAY["支付宝"]

    APPLEPAY["Apple Pay"]

end


%% -------------------------
%% Crypto Exchange
%% -------------------------

subgraph EXCHANGE["加密资产交易"]

    CEX["中心化交易所 CEX"]

end


%% -------------------------
%% Crypto Assets
%% -------------------------

subgraph ASSETS["数字资产"]

    USDT["USDT"]

    USDC["USDC"]

    BTC["BTC"]

    ETH["ETH"]

end


%% -------------------------
%% On-chain
%% -------------------------

subgraph ONCHAIN["钱包 / 区块链"]

    WALLET["数字钱包"]

    CHAIN["公链"]

end


%% -------------------------
%% Cards
%% -------------------------

subgraph CARDS["卡体系"]

    UCARD["U卡"]

    VISA["Visa"]

    MASTERCARD["Mastercard"]

end


%% -------------------------
%% Merchant
%% -------------------------

MERCHANT["全球商户"]


%% =========================================================
%% Bank → Fiat
%% =========================================================

CN_BANK --> CNY

HK_BANK --> HKD
HK_BANK --> USD

MO_BANK --> HKD

US_BANK --> USD

EU_BANK --> EUR

SG_BANK --> USD


%% =========================================================
%% Fiat Exchange Relationships
%% =========================================================

CNY <--> HKD
CNY <--> USD
CNY <--> EUR

HKD <--> USD
HKD <--> EUR

USD <--> EUR


%% =========================================================
%% Mainland Payment
%% =========================================================

CN_BANK --> WECHAT
CN_BANK --> ALIPAY


%% =========================================================
%% Banking Network
%% =========================================================

CN_BANK --> HK_BANK
CN_BANK --> MO_BANK

HK_BANK --> US_BANK
HK_BANK --> EU_BANK
HK_BANK --> SG_BANK

MO_BANK --> HK_BANK


%% =========================================================
%% Financial Services
%% =========================================================

HK_BANK --> WISE
HK_BANK --> N26
HK_BANK --> IFAST

US_BANK --> WISE
EU_BANK --> N26
SG_BANK --> WISE


%% =========================================================
%% Financial Services → Exchange
%% =========================================================

WISE --> CEX
N26 --> CEX
IFAST --> CEX

US_BANK --> CEX
EU_BANK --> CEX
SG_BANK --> CEX


%% =========================================================
%% Fiat → Exchange
%% =========================================================

USD --> CEX
EUR --> CEX
HKD --> CEX


%% =========================================================
%% Exchange → Crypto
%% =========================================================

CEX --> USDT
CEX --> USDC
CEX --> BTC
CEX --> ETH


%% =========================================================
%% Crypto → Wallet
%% =========================================================

USDT --> WALLET
USDC --> WALLET
BTC --> WALLET
ETH --> WALLET


%% =========================================================
%% Wallet ↔ Blockchain
%% =========================================================

WALLET --> CHAIN
CHAIN --> WALLET


%% =========================================================
%% Stablecoin → Card
%% =========================================================

USDT --> UCARD
USDC --> UCARD


%% =========================================================
%% Card Network
%% =========================================================

UCARD --> VISA
UCARD --> MASTERCARD

VISA --> APPLEPAY
MASTERCARD --> APPLEPAY


%% =========================================================
%% Traditional Bank → Card
%% =========================================================

US_BANK --> VISA
EU_BANK --> VISA

US_BANK --> MASTERCARD
EU_BANK --> MASTERCARD


%% =========================================================
%% Payment → Merchant
%% =========================================================

WECHAT --> MERCHANT
ALIPAY --> MERCHANT
APPLEPAY --> MERCHANT

VISA --> MERCHANT
MASTERCARD --> MERCHANT
