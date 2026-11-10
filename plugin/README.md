# Yuanjing AI Image Connect

This skill helps users connect a compatible desktop agent to Yuanjing AI, check an existing connection, and hand off image generation, editing, or product visual requests to the installed Yuanjing AI skill.

When a user requests a connection, the workflow fetches the public release manifest and installation guide from yuanjing-ai.com. A capable desktop host can follow that guide to download and verify the official authentication bootstrap, then install the official skill after the user connects in a local prompt. The plugin bundle itself contains instructions and a logo. It stores no credentials. The official client stores the user's credential locally and connects to Yuanjing AI. Image requests can upload user-authorized assets and consume account credits after the user approves the quoted cost.

In a hosted client without local execution and credential storage, the skill provides the official desktop setup guide. The bundle does not provide a hosted MCP endpoint.

- [Official setup guide](https://yuanjing-ai.com/.well-known/yuanjing-agent-install.md)
- [Publisher and support](https://yuanjing-ai.com)

Install in Claude Code:

/plugin install yuanjing-image-connect --marketplace zhouguida123-svg/yuanjing-image-connect
