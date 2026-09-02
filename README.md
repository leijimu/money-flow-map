# 喜蜘蛛 · Money Flow Map

**全球资金网络与金融基础设施关系地图**

**Xizhizhu · Money Flow Map**

Open-source map of global money flows and financial infrastructure.

---

## 出入金链路泳道图（Bloomberg 终端风）

**[money-flow-map.html](https://github.com/leijimu/money-flow-map/blob/main/money-flow-map.html)** — 出入金实测链路全景泳道图，Bloomberg 终端视觉风格，单文件零外链（全内联，离线可用）。

- 112 个节点 / 38 条实测链路，覆盖支付、银行卡、金融机构、银行、交易所、公链、经纪商等渠道
- 顶部菜单按渠道分组筛选，图表区支持通道 / 分组切换、标签显隐
- 状态语义：绿 = 已完成、琥珀 = 部分、红 = 待办、灰 = 未实测
- 文件顶栏含分组徽章、LIVE 指示灯、UTC+北京双时钟与 KPI

> 使用方式：下载 `money-flow-map.html` 用浏览器直接打开即可，无需联网。

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

- [`data/lanes-source.html`](data/lanes-source.html) — 出入金泳道原始数据稿（38 组链路 / 112 节点）
- [`data/nodes.md`](data/nodes.md) — 节点词典（16 类 / 64 个实体）
- [`data/relations.md`](data/relations.md) — 关系词典（8 类资金关系）

## 版本

- V0.3 — 出入金链路泳道图（Bloomberg 终端风，112 节点 / 38 链路）
- V0.2 — 64 节点交互式总图
