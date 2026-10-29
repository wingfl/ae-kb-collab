# ae-kb-collab

飞书「材料 → 完整文档 → 审核 → 台账」协同台的一键部署包。给能操作终端的 AI Agent 用，它按说明把知识库、协同台、权限和 Skill 一次装好。

## 需要什么

- 一个能操作终端、能读写文件的 AI Agent（Codex、Claude Code、Trae、WorkBuddy 等）
- `lark-cli`（未装时说明里给了安装与登录步骤）
- 执行者本人有飞书云空间写权限；建知识库空间需要管理员在后台开开关

## 一步

把 [prompt.md](prompt.md) 里那段话复制给 Agent，不用改。它读 [onboard.md](onboard.md)，按 §0 检查环境、§1–§5 部署，最后用 §0.3 的命令把 [SKILL.md](SKILL.md) 装进 skills 目录。

唯一需要人动手的是登录授权：Agent 会把链接发过来，点一次即可。

## 文件

| 文件 | 作用 |
| --- | --- |
| `prompt.md` | 可直接复制的口令，四个参数位 |
| `onboard.md` | 五步部署手册：环境检查、建知识库、建三张表、建自动化、权限、验收、回滚 |
| `SKILL.md` | 材料整合 Skill 包，装进 Agent 后按四态流转执行 |

## 不做什么

- 不改动执行者现有的 Base、文档和云盘目录
- 不用应用身份代替本人建资源
- 不在仓库里存任何真实 token、open_id 或租户信息
