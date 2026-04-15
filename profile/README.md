<p align="center">
  <img src="https://raw.githubusercontent.com/veritera-ai/eydii-python/main/assets/demo.gif" alt="EYDII — verify and block an AI agent action in real-time" width="700">
</p>

<h3 align="center">Trustless verification for AI agents</h3>

<p align="center">
  Content-blind. Sub-15ms. 13 framework integrations.
  <br>
  <a href="https://github.com/veritera-ai/eydii-python"><strong>Get started &rarr;</strong></a>
</p>

---

AI agents send emails, move money, and call APIs. No framework verifies what they do. **EYDII** checks every action before execution — without seeing your code, prompts, data, or outputs. Policies enforced outside the agent. Independently verifiable with Ed25519.

```python
from veritera import EydiiVerify
eydii = EydiiVerify(api_key="vt_live_...")

result = eydii.verify_sync(action="database.drop", agent_id="bot", policy="safety")
# result.verified = False
# result.reason = "Action 'database.drop' is blacklisted"
```

### SDKs

| | Package | Install |
|-|---------|---------|
| **Python** | [eydii-python](https://github.com/veritera-ai/eydii-python) | `pip install veritera` |
| **TypeScript** | [eydii-js](https://github.com/veritera-ai/eydii-js) | `npm install @veritera.ai/eydii-verify` |
| **LangChain** | [eydii-langchain](https://github.com/veritera-ai/eydii-langchain) | `pip install langchain-eydii` |
| **MCP** | [eydii-mcp-server](https://github.com/veritera-ai/eydii-mcp-server) | Claude Code, Cowork, ChatGPT, Cursor |

[**13 framework integrations**](https://github.com/veritera-ai/eydii-python#13-framework-integrations) including OpenAI, CrewAI, LlamaIndex, n8n, Mastra, Google ADK, Agno, and Pydantic AI.

---

<p align="center">
  <a href="https://id.veritera.ai">Website</a> &middot; <a href="https://github.com/veritera-ai/eydii-python">Documentation</a> &middot; <a href="https://id.veritera.ai/trust">Trust & Security</a>
</p>
