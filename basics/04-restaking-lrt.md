# Restaking、EigenLayer 与 LRT

---

## 核心概念：Restaking（再质押）

把已质押在以太坊上的 ETH（或 stETH 等流动性质押凭证）再次用来为其他协议提供安全性，换取额外收益，代价是承担额外的罚没（slashing）风险。

---

## EigenLayer

Restaking 赛道的开创者。机制：

- 验证者通过 EigenLayer 智能合约**选择加入（opt-in）**，把质押暴露给额外的罚没条件
- 换取为 **AVS（Actively Validated Services，主动验证服务）** 提供安全的额外收益

**AVS 典型案例**：预言机、数据可用性层（EigenDA）、跨链桥等

**核心逻辑**：以太坊的信任可以"出租"给新协议 — 新协议不用从零启动自己的验证者网络

**主要风险**：
- 罚没风险叠加（一个验证者承担多重 slashing 条件）
- 收益来源不透明时容易变成积分庞氏

---

## LRT（Liquid Restaking Token，流动性再质押凭证）

用户把 ETH 存入 Ether.fi、Renzo 等协议 → 协议替用户去 EigenLayer 做 restaking → 用户拿到 eETH、ezETH 等 LRT，**既赚 restaking 收益又保持流动性，还能拿去 DeFi 套娃**。

| 协议 | LRT | 代币 |
|------|-----|------|
| Ether.fi | eETH | ETHFI |
| Renzo | ezETH | REZ |
| EigenLayer 本身 | — | EIGEN |

**LRT 特有风险**：
- **脱锚风险**：ezETH 于 2024年4月因空投规则争议发生脱锚
- **多层套娃放大清算**：LRT → DeFi 借贷 → 杠杆，连锁清算风险高于单层质押

---

## 对 BD 的意义（上币尽调维度）

```
2024-2025 上币热点赛道，代表项目：EIGEN、ETHFI、REZ

尽调时要区分真实需求 vs 积分挖矿堆出的 TVL：
- 关键指标：积分活动结束后 TVL 留存率
- 关键指标：AVS 的实际采用量（有哪些真实项目在用）
- 不要只看锁仓峰值，要看活动结束后的留存曲线
```
