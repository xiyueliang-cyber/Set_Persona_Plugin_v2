# Set Persona Plugin

智能 Agent 配置插件 - 通过自然语言对话配置 Agent 的人设、能力和知识库。

## 功能

- 配置 Agent 的名称、角色、人格、说话风格
- 管理 Agent 的知识库
- 安装和管理 Agent 的 Capability

## 使用方式

### 1. 自动触发
用户在对话中提到配置相关内容（如"帮我改个名字"），Plugin 自动激活。

### 2. Slash 命令
使用 `/set-persona` 命令显式进入配置模式。

## 核心原则

- **确认机制**：所有配置操作需要用户明确确认
- **逐步引导**：一次只问一个问题，循序渐进
- **立即生效**：配置完成后立即以新身份交互

## 详细文档

请查看 marketplace 根目录的文档：
- `INTEGRATION.md` - 集成指南
- `QUICKSTART.md` - 快速开始
- `docs/ARCHITECTURE.md` - 架构设计
- `docs/API.md` - API 文档
