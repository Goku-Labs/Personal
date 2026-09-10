# mimocode 对话存档（个人知识库项目）

本目录保存了 mimocode（Mimo AI）中关于本项目 `D:\documents\Knowledge\Personal` 的对话记录，
由 `mimocode.db`（`C:\Users\wukon\.local\share\mimocode\mimocode.db`）导出保存，2026-08-17 导出。

## 会话文件（可读的 Markdown 存档）

| 文件 | 会话 | 时间范围 | 说明 |
|------|------|----------|------|
| `个人知识库搭建建议-完整对话.md` | `ses_0718a4312ffewlq3XO1kVNX3aB`（fork #1） | 2026-06-23 → 2026-08-17 | **主对话完整版**，690 条消息（用户 150 / 助手 540），含全部文本、思考过程（折叠）、工具调用与结果（折叠） |
| `个人知识库搭建建议-原始会话.md` | `ses_10c5957d2ffeD6LZ81u0pXgOaH` | 2026-06-23 → 2026-07-23 | 原始会话（fork #1 之前的版本），612 条消息 |
| `其他相关会话.md` | 3 个小会话 | 2026-07-08 / 2026-08-17 | 今天（08-17）的两个 fork #2 小会话（含「你还记得我们的对话吗」）+ 7月股市亏损吐槽 |

## 原始数据（无损备份，JSONL）

每个会话的 `会话原始数据-<会话ID>.jsonl`：逐条保存 message 与 part 的完整 JSON 原文，
可据此重新导入或精确检索（含被折叠/截断的长内容）。

## mimocode 记忆与检查点（mimocode 侧沉淀的摘要）

- `mimocode项目记忆-MEMORY.md` — 本项目在 mimocode 中的项目记忆（13 KB，最浓缩的上下文）
- `checkpoint-主会话-fork1.md` / `notes-主会话-fork1.md` — 主会话检查点
- `checkpoint-原始会话.md` / `notes-原始会话.md` — 原始会话检查点

## 阅读说明

- Markdown 文件按日期分节（`## YYYY-MM-DD`），每条消息标注角色与时间。
- 「🧠 思考过程」「🔧 工具调用」「📝 文件变更」为折叠块（`<details>`），默认收起，点击展开；
  工具输出超过 6000 字符、输入超过 2000 字符的部分已截断，完整内容见对应的 JSONL 原始数据。
- 导出脚本：`D:\documents\Knowledge\Personal\.mimocode\_export.py`（如需重新导出可再次运行）。

> 说明：Inbox 为临时区，如需长期保留建议归档到 `Topics/` 或移动到合适位置。
