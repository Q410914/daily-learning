# Claude Code 常用命令

> 除 `/clear`（清屏）和 `/compact`（压缩上下文）外的常用命令。

## 对话控制

| 命令 | 功能 | 用法 |
|------|------|------|
| `/undo` | 撤销上一条消息及其所有操作 | 直接输入 `/undo` |
| `/resume [消息]` | 中断对话后让 Claude 恢复或回答指定问题 | `/resume 我们刚才改到哪了？` |
| `/retry` | 重新生成上一条回复 | 直接输入 |
| `/compact` | 压缩对话历史以释放上下文窗口 | 对话太长时使用 |
| `/clear` | 清空整个对话历史，重新开始 | 直接输入 |

## 模式切换

| 命令 | 功能 | 用法 |
|------|------|------|
| `/fast` | 切换到快速模式（Opus 4.6，更快输出） | 直接输入切换，再输一次切回 |
| `/config` | 打开设置面板，修改主题、模型等偏好 | 直接输入 |
| `/doctor` | 检查 Claude Code 环境配置是否正常 | 遇到异常时先跑这个 |

## 技能与插件

| 命令 | 功能 | 用法 |
|------|------|------|
| `/skills` | 打开技能弹窗，查看所有已安装技能 | 直接输入 |
| `/plugin` | 管理插件市场（安装/列出/删除） | `/plugin marketplace list` 列出市场 |
| `/plugin marketplace add <市场名>` | 添加插件市场 | `/plugin marketplace add anthropics/skills` |
| `/plugin install <技能名@市场名>` | 从市场安装技能 | `/plugin install pdf@anthropic-agent-skills` |
| `/reload-plugins` | 重新加载所有插件和技能 | 安装新插件后需要执行 |

## 系统与文件

| 命令 | 功能 | 用法 |
|------|------|------|
| `/help` | 显示帮助信息或具体话题 | `/help` 或 `/help mcp` |
| `/memory` | 打开记忆管理界面 | 查看/搜索/删除记忆条目 |
| `/loop <间隔> <指令>` | 按间隔重复执行指令 | `/loop 5m 检查部署状态` |

## MCP（Model Context Protocol）

| 命令 | 功能 | 用法 |
|------|------|------|
| `/mcp` | 查看已配置的 MCP 服务器 | 直接输入 |
| `claude mcp add` | CLI 中配置 MCP 服务器 | 详见 `claude mcp --help` |

## 快捷键

| 快捷键 | 功能 |
|--------|------|
| `Ctrl+C` | 中断当前回复 |
| `Alt+T` / `Win+T` | 切换思考模式（展示推理过程） |
| `! <命令>` | 将命令交给本地 shell 执行（非 Claude 运行） |

> **提示**：`!` 前缀很实用——把你想在终端跑的命令用 `!` 开头，Claude 会直接把命令交给你的 shell 执行，输出会回到对话里。
