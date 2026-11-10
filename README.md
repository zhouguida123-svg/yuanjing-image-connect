# 源景 AI 作图连接器 · Yuanjing AI Image Connect

面向支持本地技能的 Agent。连接源景账号后，可以用自然语言发起生图、改图和商品视觉任务。可用模型及费用以账户实时结果为准。

```bash
npx skills add zhouguida123-svg/yuanjing-image-connect --skill yuanjing-image-connect
```

安装后，在支持本地命令和安全凭据的 Agent 中说「帮我连接源景 AI」。首次连接通过官网提供的本机交互程序完成，安装完整版需要相应的源景账户权益。

## 做第一张商品图

连接自检成功后，发一张商品参考图给同一个 Agent，并复制下面这句话。

> 请用源景 AI 根据我上传的商品参考图做 1 张白底商品主图。保留产品外形、颜色、标识和包装文字。先给出本次准确报价，等我确认后再生成。完成后给我原图下载入口；如果等待超时，请继续查询原任务，不重新提交。

This public Agent Skill guides compatible desktop agents through the official Yuanjing AI connection flow. It can hand off image generation, editing, and product visual requests to the official skill once the user has connected. The repository contains the connection instructions. The full skill is distributed by Yuanjing AI based on account access.

- [源景 AI 官网](https://yuanjing-ai.com)
- [官方安装与连接细则](https://yuanjing-ai.com/.well-known/yuanjing-agent-install.md)
- [官方实时清单](https://yuanjing-ai.com/.well-known/yuanjing-agent-skill.json)

The [desktop plugin bundle](./plugin) provides portable Agent Plugins and Claude Code manifests.

## 在桌面 Agent 中安装为插件

Codex CLI

```bash
codex plugin marketplace add zhouguida123-svg/yuanjing-image-connect
codex plugin add yuanjing-image-connect@yuanjing-ai
```

Claude Code

```bash
claude plugin marketplace add zhouguida123-svg/yuanjing-image-connect
claude plugin install yuanjing-image-connect@yuanjing-ai
```

GitHub Copilot CLI 可直接添加同一个 GitHub 插件目录。

```bash
copilot plugin marketplace add zhouguida123-svg/yuanjing-image-connect
copilot plugin install yuanjing-image-connect@yuanjing-ai
```

也可以为当前项目安装固定版本的 Skill。

```bash
gh skill install zhouguida123-svg/yuanjing-image-connect yuanjing-image-connect@v1.0.0 --agent github-copilot --scope project
```

首次连接按官网安装细则执行。
