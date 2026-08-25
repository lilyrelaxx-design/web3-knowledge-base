# Web3 知识库

> 交易所 BD 的个人知识库。基础概念 + 分析方法 + 案例 + 调研档案 + 工作实务。
> 对话结束后由 Stop hook 自动沉淀新知识（脚本：`../update_knowledge_base.sh`）。

---

## 怎么用这个库

| 场景 | 去哪 |
|------|------|
| 日报/群里看到不懂的词 | [基础知识](#一基础知识-basics) → 找概念 |
| 要评估一个项目该不该上 | [分析方法](#二分析方法-methods) → 01 基本面手册 + 02 尽调五步法 |
| 怀疑是资金盘 | [方法 02](methods/02-due-diligence.md) 五步法 + [方法 01 第十四章](methods/01-project-fundamentals.md) 红旗清单 |
| 写研报 / 做赛道调研 | [方法 03](methods/03-research-writing.md) 框架与写作规范 |
| 想看某个赛道现在什么情况 | [调研档案](#四调研档案-research) |
| 干活遇到具体问题 | [工作实务](#五工作实务-work) |

---

## 一、基础知识 `basics/`

> **概念和原理，不带时效性**。这部分是打底的，看懂了才能读懂后面所有内容。

| 文件 | 讲什么 | 关键概念 |
|------|--------|---------|
| [01-bitcoin-rgb.md](basics/01-bitcoin-rgb.md) | 比特币为什么"不可编程"，RGB 协议怎么绕过这个限制在比特币上发资产 | UTXO 防双花、Client-Side Validation、Single-Use Seal ⚠️含 2026-07-28 复核修正 |
| [02-rollup-l2.md](basics/02-rollup-l2.md) | 以太坊为什么需要扩容，Rollup 的原理和 Arbitrum 的挑战期机制 | Rollup、L2、挑战期、与 RGB 的路线对比 |
| [03-defi.md](basics/03-defi.md) | DeFi 五大件的运作原理 | AMM/资金池、超额抵押与清算、稳定币三类、收益聚合、可组合性 |
| [04-restaking-lrt.md](basics/04-restaking-lrt.md) | 再质押赛道的机制与风险 | Restaking、EigenLayer、AVS、LRT（eETH/ezETH）、脱锚风险 |

**另有一份基础概念速成**在 [方法 01 第一章](methods/01-project-fundamentals.md)：链上vs链下、智能合约、AMM/LP/无常损失、质押与LST、Gas、L1/L2、预言机、跨链桥、稳定币三型、Perp/OI/资金费率、空投撸毛、合约权限——按日报出现频率排序，看不懂的词先查这里。

---

## 二、分析方法 `methods/`

> **可复用的框架**。判断任何项目都用得上，是这个库最该反复翻的部分。

### [01-project-fundamentals.md](methods/01-project-fundamentals.md) — 项目基本面完整手册 ⭐

配合 Q1–Q5 框架的主力工具。每个指标按「是什么 → 数据在哪看 → 怎么读（带基准数字）→ 怎么被造假 → 迷你案例」展开：

- **指标详解**：TVL / 市值·FDV·供应结构 / 收入与费用 / 用户指标 / 交易量 / 代币经济学 / 团队·融资·金库 / 流动性与市场结构 / 安全与合约风险
- **实操工具**：竞品对比五步法、分赛道速查表（10 个赛道的主指标与常见死法）、数据源操作清单（13 个工具去哪看什么）
- **核心心法**：任何单一指标都不能下结论，指标互相验证才有意义
- **[第十四章红旗清单](methods/01-project-fundamentals.md#第十四章-红旗清单q5快速排查)**：结构/数据/代币/团队四类，命中 ≥3 条基本可以下结论

### [02-due-diligence.md](methods/02-due-diligence.md) — 尽调五步法与资金盘识别

专治"这个项目看着不太对"。含两个完整案例拆解（CocoCat、CaryPact/BOT Chain）和通用红旗清单。和 01 的关系：**01 判断正经项目值不值，02 判断是不是骗局**。

### [03-research-writing.md](methods/03-research-writing.md) — 研报写作规范与赛道调研框架

- **单项目研报**（第一～六节）：来源标注标准、可比公司估值表怎么列、列名规范、极端情景放脚注、销毁数据口径陷阱
- **赛道调研**（第七～九节）：16 环节固定框架、来源三级制 A/B/C + 五条硬规则、事件触发制检查点

---

## 三、案例分析 `cases/`

> **具体项目和事件的深度拆解**。看方法论看不明白的地方，看案例就懂了。

| 文件 | 讲什么 | 为什么值得看 |
|------|--------|------------|
| [01-hyperliquid.md](cases/01-hyperliquid.md) | Hyperliquid 全解析：双层架构、HIP-1/2/3/4、HLP、回购模型、Coinbase/Circle 绑定、美国合规、风险清单（数据截至 2026-08-25） | 理解"什么样的项目才有资格自建链"；Perp DEX 技术门槛；交易所如何变成"交易所的基础设施" |
| [02-ftx-exchange-tokens.md](cases/02-ftx-exchange-tokens.md) | FTX 暴雷全过程 + 交易所平台币的价值逻辑 + Backpack/BP 分析 | 平台币是 BD 的主场，这篇讲清了平台币凭什么值钱、以及交易所怎么死的 |

---

## 四、调研档案 `research/`

> **带时效性**，每篇标注调研日期。活跃跟踪的档案会持续更新，不另起新档。规则见 [research/README.md](research/README.md)。

| 文件 | 主题 | 状态 |
|------|------|------|
| [2026-07-rgb-track.md](research/2026-07-rgb-track.md) | **RGB 赛道完整档案**：v0.11.1/v0.12 路线分裂、Tether-USDT 落地进度、UTEXO 定位、vs Taproot Assets 与 Tron、生态盘点、可交易敞口、五阶段划分、监控清单 | 🔴 活跃跟踪<br>2026-07-28 |
| [2026-08-exchange-launchpad.md](research/2026-08-exchange-launchpad.md) | **各大交易所打新现状**：Launchpool 整体降温、入口换道三叉路（快照持仓/积分行为/上币奖池）、代币化美股成新战场、Gate 当前最活跃 | 2026-08-02 |
| [2026-07-cmc-cber.md](research/2026-07-cmc-cber.md) | CMC/Cber 平台币研报：流通市值、回撤幅度、2.0 升级催化、销毁数据口径拆解 | 2026-07-29 |

---

## 五、工作实务 `work/`

> **怎么干活**。BD、运营、内容生产的方法和踩过的坑。规则见 [work/README.md](work/README.md)。

| 文件 | 内容 |
|------|------|
| [kb-management.md](work/kb-management.md) | 知识库自己的使用说明：GitHub 在线查看、推送命令、自动同步机制、网页版对话手动搬运的三种方式 |

*待沉淀：`bd-playbook.md`（上币流程/谈判/返佣/做市商）、`twitter-ops.md`、`xhs-ops.md`、`content-creation.md`*

---

## 六、归档 `archive/`

[web3-knowledge-all-2026-06.md](archive/web3-knowledge-all-2026-06.md) — 2026-06 的早期合并版快照，内容已被 basics/ 和 cases/ 各文件取代，仅作历史留存，不再维护。

---

## 快速概念索引

**比特币 / RGB**
- UTXO 与防双花 → [基础 01](basics/01-bitcoin-rgb.md#utxo与防双花)
- Client-Side Validation → [基础 01](basics/01-bitcoin-rgb.md#client-side-validation)
- Single-Use Seal → [基础 01](basics/01-bitcoin-rgb.md#single-use-seal一次性封印)
- RGB vs RGB++（易混淆）→ [RGB档案](research/2026-07-rgb-track.md#五rgb-与-rgb-的区别)
- RGB v0.11.1 vs v0.12 分裂 → [RGB档案](research/2026-07-rgb-track.md#六rgb-v0111-与-v012-分裂)
- USDT-on-RGB 落地状态 → [RGB档案](research/2026-07-rgb-track.md#九usdt-on-rgb-当前状态)
- Taproot Assets → [RGB档案](research/2026-07-rgb-track.md#十竞争格局)

**以太坊 / 扩容**
- Rollup 原理 → [基础 02](basics/02-rollup-l2.md#rollup-是什么)
- 挑战期 → [基础 02](basics/02-rollup-l2.md#arbitrum-的安全机制挑战期)

**DeFi**
- AMM / 资金池 → [基础 03](basics/03-defi.md#dex去中心化交易所)
- 超额抵押 / 清算 → [基础 03](basics/03-defi.md#借贷协议如aave)
- 可组合性 → [基础 03](basics/03-defi.md#defi的可组合性乐高积木)
- Restaking / EigenLayer / AVS → [基础 04](basics/04-restaking-lrt.md)
- LRT / 流动性再质押凭证 → [基础 04](basics/04-restaking-lrt.md)

**估值与指标**
- TVL 怎么读 / 怎么被造假 → [方法 01](methods/01-project-fundamentals.md#第二章-tvl总锁仓量)
- MC/FDV、低流通高估值 → [方法 01](methods/01-project-fundamentals.md#第三章-市值fdv与供应结构)
- 解锁压力算术（90天解锁÷日均交易量）→ [方法 01](methods/01-project-fundamentals.md#72-解锁表vesting)
- 价值捕获五档 → [方法 01](methods/01-project-fundamentals.md#73-价值捕获value-accrualq2的核心问题)
- Real Yield / 真实收益 → [方法 01](methods/01-project-fundamentals.md#74-通胀与真实收益)
- wash trading / 刷量识别 → [方法 01](methods/01-project-fundamentals.md#第六章-交易量)
- 分赛道速查表 → [方法 01](methods/01-project-fundamentals.md#第十二章-分赛道速查表)
- 数据源清单 → [方法 01](methods/01-project-fundamentals.md#第十三章-数据源操作清单)

**风险识别**
- 基本面红旗清单 → [方法 01](methods/01-project-fundamentals.md#第十四章-红旗清单q5快速排查)
- 尽调五步法 → [方法 02](methods/02-due-diligence.md#一项目尽调五步法)
- 资金盘红旗清单 → [方法 02](methods/02-due-diligence.md#四通用红旗清单两个案例共同特征)

**写作与调研**
- 赛道调研固定框架 → [方法 03](methods/03-research-writing.md#七赛道调研固定框架rgb赛道调研-2026-07-28-固化)
- 来源三级制 + 五条硬规则 → [方法 03](methods/03-research-writing.md#八信息分级与写作准确性硬规则)
- 事件触发制检查点 → [方法 03](methods/03-research-writing.md#九检查点用事件触发制不用硬日期)
- 销毁数据口径陷阱 → [方法 03](methods/03-research-writing.md#六销毁数据口径陷阱代币经济学常见坑)

**交易所 / BD**
- 交易所平台币逻辑 → [案例 02](cases/02-ftx-exchange-tokens.md#二什么是交易所平台币)
- FTX 事件 → [案例 02](cases/02-ftx-exchange-tokens.md#一ftx-事件加密行业的暴雷银行)
- 自建链需要什么条件 → [案例 01](cases/01-hyperliquid.md#自建链需要的条件)
- HyperCore vs HyperEVM 双层架构 → [案例 01](cases/01-hyperliquid.md#两层架构hypercore-vs-hyperEVM)
- HIP-1 / HIP-2 代币标准 → [案例 01](cases/01-hyperliquid.md#当前业务结构)
- HLP 金库机制与风险 → [案例 01](cases/01-hyperliquid.md#当前业务结构)
- HIP-3 建设者自建永续市场 → [案例 01](cases/01-hyperliquid.md#hip-3从一个交易所变成交易所的基础设施)
- HIP-4 结果市场/预测市场 → [案例 01](cases/01-hyperliquid.md#hip-4结果市场预测市场)
- 手续费回购模型（援助基金）→ [案例 01](cases/01-hyperliquid.md#商业模式手续费--回购-hype)
- USDH 清盘与 Coinbase/Circle 绑定 → [案例 01](cases/01-hyperliquid.md#生态与外部关系)
- OI 份额 vs 交易量份额的口径陷阱 → [案例 01](cases/01-hyperliquid.md#生态与外部关系)
- 各所打新现状 → [调研](research/2026-08-exchange-launchpad.md)
