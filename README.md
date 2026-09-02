# 喜蜘蛛 · Money Flow Map

**全球资金网络与金融基础设施关系地图**

**Xizhizhu · Money Flow Map**

Open-source map of global money flows and financial infrastructure.

---

## 出入金链路图（源稿 · 一条一行）

**[money-flow-map.html](https://github.com/leijimu/money-flow-map/blob/main/money-flow-map.html)** — 出入金实测链路数据稿「一条一行」版：38 条链路 / 112 个节点，覆盖入金到券商、稳定币出金互转、卡产品商户落地与片段待闭环链路，状态含已到账 / 片段 / 待闭环 / 未完整实测。

> 使用方式：浏览器直接打开即可（GitHub Pages 在线预览：https://leijimu.github.io/money-flow-map/money-flow-map.html ），无需下载。

---

## 喜蜘蛛是什么？

**喜蜘蛛** 是一张开放的全球资金网络地图。

它尝试把分散在不同国家、地区和金融体系中的：

- 法定货币
- 银行
- 支付平台
- 金融服务
- 加密货币交易所
- 稳定币
- 加密资产
- 区块链
- 数字钱包
- 卡产品
- Visa / Mastercard
- 商户

放到同一张网络中进行观察。

```text
货币
 ↓
银行
 ↓
金融服务
 ↓
交易所
 ↓
数字资产
 ↓
钱包 / 区块链
 ↓
卡 / 支付网络
 ↓
商户
```

## 数据

- [`data/nodes.md`](data/nodes.md) — 节点词典（16 类 / 64 个实体）
- [`data/relations.md`](data/relations.md) — 关系词典（8 类资金关系）

## 版本

- V0.3.1 — 主文件替换为出入金链路源稿（一条一行版，112 节点 / 38 链路）
- V0.3 — 出入金链路泳道图（Bloomberg 终端风，已在 git 历史中可回溯）
