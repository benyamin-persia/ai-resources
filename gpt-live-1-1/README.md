# GPT-Live-1.1 Voice API

Shared in [Code Cloud's X post](https://x.com/codecloude/status/2123519727029145832), which points to the [official OpenAI Live API guide](https://developers.openai.com/api/docs/guides/live). GPT-Live supports full-duplex voice conversations and can delegate tasks to a backend model or agent. The official [GPT-Live-1.1 model page](https://developers.openai.com/api/docs/models/gpt-live-1.1) currently lists $0.05/minute active and $0.02/minute standby; the lower standby rate applies to WebRTC sessions while inference is paused. Backend model and tool usage is billed separately. Pricing and availability can change.

The post links to documentation and a Telegram invite, not a GitHub repository, so there were no GitHub projects to fork. For implementation, the official guide covers session setup, WebRTC/WebSocket connections, backend delegation, and keeping project API keys on a trusted server.
