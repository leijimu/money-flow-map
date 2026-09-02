# 喜蜘蛛 · Money Flow Map

**全球出入金链路与资金基础设施地图**

**Xizhizhu · Money Flow Map**

Open-source map of global money-in / money-out lanes and financial infrastructure.

---

## 在线预览

**https://leijimu.github.io/money-flow-map/money-flow-map.html**

GitHub Pages 直接渲染，浏览器打开即用，无需下载。每次推送后约 1~2 分钟自动更新。

---

## 出入金链路图（源稿 · 一条一行）

**[money-flow-map.html](money-flow-map.html)** — 出入金实测链路数据稿，一链路一行。共 **38 条链路 / 112 个节点**，四组覆盖：

| 组 | 内容 |
|---|---|
| A | 入金到券商（法币 / 电汇 / 通道） |
| B | 稳定币出金互转 |
| C | 卡产品商户落地 |
| D | 片段 · 待闭环链路 |

状态标记：已到账 / 片段 / 待闭环 / 未完整实测。节点类型涵盖支付、卡产品、金融机构、银行、交易所、公链、经纪商等。

> 使用方式：浏览器直接打开文件即可（纯静态单文件，无需联网）。

---

## 历史版本

- **V0.3 · Bloomberg 终端风泳道图**：深色终端视觉、分组菜单筛选、LIVE 灯与双时钟，112 节点 / 38 链路。保存在 git 历史（commit `ce627ee`），可用 `git checkout ce627ee -- money-flow-map.html` 取回
- **V0.2 · 64 节点交互式总图**：资金网络全景图

## 数据

- [`data/nodes.md`](data/nodes.md) — 节点词典（16 类 / 64 个实体）
- [`data/relations.md`](data/relations.md) — 关系词典（8 类资金关系）

## 版本

- V0.3.1 — 主文件为出入金链路源稿（一条一行版）
- V0.3 — 出入金链路泳道图（Bloomberg 终端风）
- V0.2 — 64 节点交互式总图

---

*本仓库仅作链路梳理与信息整理，不构成任何操作或投资建议。*
