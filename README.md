# 喜蜘蛛 · Money Flow Map

**全球资金网络与金融基础设施关系地图**

**Xizhizhu · Money Flow Map**

Open-source map of global money flows and financial infrastructure.

---

## 交互式总图

**[money-flow-map.html](https://github.com/leijimu/money-flow-map/blob/main/money-flow-map.html)** — 64 节点交互式资金网络总图，支持拖拽平移、滚轮缩放、点击节点高亮相邻链路。

> 使用方式：下载 `money-flow-map.html` 后用浏览器打开即可（需联网加载 ECharts CDN）。或在仓库 Settings → Pages 中启用 GitHub Pages，即可通过网页直接访问。

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

- V0.2 — 64 节点交互式总图
