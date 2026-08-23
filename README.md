# Money Network Map

Open-source map of global money networks and financial infrastructure.

开放的全球资金网络与金融基础设施关系地图。

## Network Map

```mermaid
flowchart LR

%% =========================
%% 银行体系
%% =========================

subgraph BANKS["银行体系"]

    CN["中国大陆银行"]

    HK["香港银行"]

    MO["澳门银行"]

    US["美国银行"]

    EU["欧洲银行"]

    SG["新加坡银行"]

end


%% =========================
%% 金融服务
%% =========================

subgraph SERVICES["金融服务"]

    WISE["Wise"]

    N26["N26"]

    IFAST["iFast"]

end


%% =========================
%% 支付
%% =========================

subgraph PAYMENT["支付体系"]

    WX["微信支付"]

    ALI["支付宝"]

    APPLE["Apple Pay"]

end


%% =========================
%% 加密资产
%% =========================

subgraph CRYPTO["数字资产"]

    CEX["中心化交易所 CEX"]

    USDT["USDT"]

    USDC["USDC"]

    BTC["BTC"]

    ETH["ETH"]

end


%% =========================
%% 钱包与区块链
%% =========================

subgraph ONCHAIN["钱包 / 区块链"]

    WALLET["数字钱包"]

    CHAIN["公链"]

end


%% =========================
%% 卡体系
%% =========================

subgraph CARD["卡体系"]

    UCARD["U卡"]

    VISA["Visa"]

    MC["Mastercard"]

end


%% =========================
%% 银行网络
%% =========================

CN --> HK
CN --> MO

HK --> US
HK --> EU
HK --> SG

MO --> HK

US --> EU
US --> SG


%% =========================
%% 金融服务
%% =========================

HK --> WISE
HK --> N26
HK --> IFAST

US --> WISE
EU --> N26
SG --> WISE


%% =========================
%% 支付
%% =========================

CN --> WX
CN --> ALI

US --> APPLE
EU --> APPLE
SG --> APPLE


%% =========================
%% 交易所
%% =========================

US --> CEX
EU --> CEX
SG --> CEX

WISE --> CEX
N26 --> CEX


%% =========================
%% 数字资产
%% =========================

CEX --> USDT
CEX --> USDC
CEX --> BTC
CEX --> ETH


%% =========================
%% 钱包 / 区块链
%% =========================

USDT --> WALLET
USDC --> WALLET
BTC --> WALLET
ETH --> WALLET

WALLET --> CHAIN
CHAIN --> WALLET


%% =========================
%% U卡
%% =========================

USDT --> UCARD
USDC --> UCARD

UCARD --> VISA
UCARD --> MC

VISA --> APPLE
MC --> APPLE

US --> UCARD
EU --> UCARD
SG --> UCARD
