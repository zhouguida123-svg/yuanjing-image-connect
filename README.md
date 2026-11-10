# 源景 AI 作图连接器 · Yuanjing AI Image Connect

面向支持本地技能的 Agent。连接源景账号后，可以用自然语言发起生图、改图和商品视觉任务。可用模型及费用以账户实时结果为准。

```bash
npx skills add zhouguida123-svg/yuanjing-image-connect --skill yuanjing-image-connect
```

安装后，在支持本地命令和安全凭据的 Agent 中说「帮我连接源景 AI」。首次连接通过官网提供的本机交互程序完成，安装完整版需要相应的源景账户权益。

This public Agent Skill guides compatible desktop agents through the official Yuanjing AI connection flow. It can hand off image generation, editing, and product visual requests to the official skill once the user has connected. The repository contains the connection instructions. The full skill is distributed by Yuanjing AI based on account access.

- [源景 AI 官网](https://yuanjing-ai.com)
- [官方安装与连接细则](https://yuanjing-ai.com/.well-known/yuanjing-agent-install.md)
- [官方实时清单](https://yuanjing-ai.com/.well-known/yuanjing-agent-skill.json)

The [desktop plugin bundle](./plugin) provides portable Agent Plugins and Claude Code manifests.
