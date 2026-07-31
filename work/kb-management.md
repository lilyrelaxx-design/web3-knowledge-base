# 知识库管理工作流

## 在线查看

GitHub 地址：**https://github.com/lilyrelaxx-design/web3-knowledge-base**

打开仓库首页直接显示知识库目录（README.md），点链接跳转各章节，手机浏览器可用。

⚠️ 当前仓库为**公开**。work/ 板块会沉淀 BD 实务经验（谈判、返佣、合作细节），建议在 GitHub → 仓库 Settings 底部将 Visibility 改为 **Private**，避免敏感信息外露。

## 推送本地更新到 GitHub

```bash
cd /Users/lilyrelaxx/cc-test/knowledge-base && git push
```

本地知识库每次自动更新都会 git commit（不 push）。定期手动 push 一次即可同步到线上。

## 知识同步方式

### Claude Code 对话 → 全自动

Stop hook 全局生效，任意目录的 Claude Code 会话结束后自动检查内容并写入知识库。
- 不需要任何操作
- 触发条件：对话含 Web3 / 调研 / BD / 运营相关内容（纯写代码、改配置、闲聊不触发）
- 节流：20 分钟内最多触发一次
- 日志：`cat ~/.claude/kb_update_state/kb_update.log`

如需立即写入（不等自动触发）：直接在对话里说"把刚才的内容写进知识库"。

### Claude 网页版 / App 对话 → 手动搬运

网页版对话内容无法被 Stop hook 获取，有三种手动方式：

**方式 A — 粘贴（最快，适合单次调研）**
1. 在网页对话里说"帮我总结这段调研的核心结论"
2. 复制结论粘贴到 Claude Code 里
3. 说"把这段内容写进知识库"

**方式 B — 拖文件（适合已有完整文档）**
把网页对话里整理好的 .md 文件拖入 Claude Code，说"把这个文件写进知识库"。（同 08-project-fundamentals.md 的入库方式）

**方式 C — 批量导出（适合清理历史积压）**
claude.ai → Settings → Privacy → **Export data**，可一次性导出全部聊天记录，发给 Claude Code 批量提取知识点分类归档。

*（2026-07-31 补充方式 B/C）*
