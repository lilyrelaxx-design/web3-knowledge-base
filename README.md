# 知识库

> 对话结束后由 Stop hook 自动整理更新（脚本：`/Users/lilyrelaxx/cc-test/update_knowledge_base.sh`）。用于复习回顾，不替代原始对话。

---

## 一、Web3 基础（编号文件）

概念、协议、项目的系统性理解。

| 文件 | 内容 | 最后更新 |
|------|------|----------|
| [01-bitcoin-rgb.md](01-bitcoin-rgb.md) | 比特币不可编程 / RGB协议 / Client-Side Validation | 2026-06-10 |
| [02-arbitrum-rollup.md](02-arbitrum-rollup.md) | Rollup原理 / Arbitrum / 以太坊扩展方案 | 2026-06-10 |
| [03-defi-basics.md](03-defi-basics.md) | DEX / 借贷协议 / 稳定币 / 收益聚合 | 2026-06-10 |
| [04-hyperliquid.md](04-hyperliquid.md) | Hyperliquid全解析 / 技术难点 / 自建链条件 | 2026-06-12 |
| [05-project-due-diligence.md](05-project-due-diligence.md) | 项目尽调方法论 / CocoCat案例 / CaryPact-BOT Chain案例 / 资金盘红旗清单 | 2026-06-16 |
| [06-ftx-and-exchange-tokens.md](06-ftx-and-exchange-tokens.md) | FTX事件全解析 / 交易所平台币逻辑 / Backpack BP代币分析 | 2026-06-18 |
| [07-restaking-eigenlayer.md](07-restaking-eigenlayer.md) | Restaking原理 / EigenLayer / AVS / LRT（eETH/ezETH）/ 上币尽调维度 | 2026-07-27 |
| [08-project-fundamentals.md](08-project-fundamentals.md) | 项目基本面完整手册：TVL / 市值与FDV / 收入费用 / 用户指标 / 交易量刷量识别 / 代币经济学 / 团队融资金库 / 流动性 / 安全审计 / 分赛道速查 / 数据源清单 / 红旗清单 | 2026-07-27 |

（[web3-knowledge-all.md](web3-knowledge-all.md) 是早期合并版快照，不再自动维护）

## 二、调研沉淀（research/）

每次调研的核心结论和洞察。规则见 [research/README.md](research/README.md)。

| 文件 | 主题 | 日期 |
|------|------|------|
| [2026-07-cmc-cber.md](research/2026-07-cmc-cber.md) | CMC/Cber平台币研报：流通市值/回撤/2.0升级催化/销毁口径拆解 | 2026-07-29 |

## 三、工作实务（work/）

BD / 运营 / 内容生产的方法论和踩坑记录。规则见 [work/README.md](work/README.md)。

| 文件 | 内容 | 最后更新 |
|------|------|----------|
| [kb-management.md](work/kb-management.md) | 知识库在线查看（GitHub）/ 推送命令 / 自动同步机制 / 网页版手动搬运三种方式（粘贴/拖文件/批量导出） | 2026-07-31 |
| [research-writing.md](work/research-writing.md) | 研报写作规范：来源标注 / 可比公司估值表 / 列名规范 / 极端情景处理 / 销毁数据口径陷阱 | 2026-07-29 |

---

## 快速概念索引

- **UTXO** → [比特币RGB](01-bitcoin-rgb.md#utxo与防双花)
- **Client-Side Validation** → [比特币RGB](01-bitcoin-rgb.md#client-side-validation)
- **Single-Use Seal** → [比特币RGB](01-bitcoin-rgb.md#single-use-seal)
- **Rollup** → [Arbitrum](02-arbitrum-rollup.md#rollup是什么)
- **AMM / 资金池** → [DeFi基础](03-defi-basics.md#dex)
- **超额抵押 / 清算** → [DeFi基础](03-defi-basics.md#借贷协议)
- **HyperBFT / 共识算法** → [Hyperliquid](04-hyperliquid.md#技术难点)
- **MEV** → [Hyperliquid](04-hyperliquid.md#技术难点)
- **Oracle** → [Hyperliquid](04-hyperliquid.md#技术难点)
- **资金盘尽调五步法** → [项目尽调](05-project-due-diligence.md#一项目尽调五步法)
- **传销/资金盘红旗清单** → [项目尽调](05-project-due-diligence.md#四通用红旗清单两个案例共同特征)
- **FTX事件** → [FTX与平台币](06-ftx-and-exchange-tokens.md#一ftx-事件加密行业的暴雷银行)
- **交易所平台币** → [FTX与平台币](06-ftx-and-exchange-tokens.md#二什么是交易所平台币)
- **Backpack / BP分析** → [FTX与平台币](06-ftx-and-exchange-tokens.md#三backpack-和-bp-代币分析)
- **Restaking / 再质押** → [Restaking与EigenLayer](07-restaking-eigenlayer.md#核心概念restaking再质押)
- **EigenLayer / AVS** → [Restaking与EigenLayer](07-restaking-eigenlayer.md#eigenlayer)
- **LRT / 流动性再质押凭证** → [Restaking与EigenLayer](07-restaking-eigenlayer.md#lrt液态再质押凭证流动性再质押凭证)
- **TVL 怎么读/怎么被造假** → [项目基本面](08-project-fundamentals.md#第二章-tvl总锁仓量)
- **MC/FDV / 低流通高估值** → [项目基本面](08-project-fundamentals.md#第三章-市值fdv与供应结构)
- **解锁压力算术（90天解锁÷日均交易量）** → [项目基本面](08-project-fundamentals.md#72-解锁表vesting)
- **价值捕获五档** → [项目基本面](08-project-fundamentals.md#73-价值捕获value-accrual q2的核心问题)
- **Real Yield / 真实收益** → [项目基本面](08-project-fundamentals.md#74-通胀与真实收益)
- **wash trading / 刷量识别** → [项目基本面](08-project-fundamentals.md#第六章-交易量)
- **分赛道速查表** → [项目基本面](08-project-fundamentals.md#第十二章-分赛道速查表)
- **数据源操作清单（DefiLlama/Dune/Tokenomist等）** → [项目基本面](08-project-fundamentals.md#第十三章-数据源操作清单)
- **基本面红旗清单** → [项目基本面](08-project-fundamentals.md#第十四章-红旗清单q5快速排查)
