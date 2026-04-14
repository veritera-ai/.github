<p align="center">
  <img src="https://raw.githubusercontent.com/veritera-ai/forge-python/main/assets/demo.gif" alt="Forge — verify and block an AI agent action in real-time" width="700">
</p>

<h3 align="center">Trustless verification for AI agents</h3>

<p align="center">
  Content-blind. Sub-15ms. 13 framework integrations.
  <br>
  <a href="https://github.com/veritera-ai/forge-python"><strong>Get started &rarr;</strong></a>
</p>

---

AI agents send emails, move money, and call APIs. No framework verifies what they do. **Forge** checks every action before execution — without seeing your code, prompts, data, or outputs. Policies enforced outside the agent. Independently verifiable with Ed25519.

```python
from veritera import Forge
forge = Forge(api_key="vt_live_...")

result = forge.verify_sync(action="database.drop", agent_id="bot", policy="safety")
# result.verified = False
# result.reason = "Action 'database.drop' is blacklisted"
```

### SDKs

| | Package | Install |
|-|---------|---------|
| **Python** | [forge-python](https://github.com/veritera-ai/forge-python) | `pip install veritera` |
| **TypeScript** | [forge-js](https://github.com/veritera-ai/forge-js) | `npm install @veritera.ai/forge-verify` |
| **LangChain** | [forge-langchain](https://github.com/veritera-ai/forge-langchain) | `pip install langchain-forge` |
| **MCP** | [forge-mcp-server](https://github.com/veritera-ai/forge-mcp-server) | Claude Code, Cowork, ChatGPT, Cursor |

[**13 framework integrations**](https://github.com/veritera-ai/forge-python#13-framework-integrations) including OpenAI, CrewAI, LlamaIndex, n8n, Mastra, Google ADK, Agno, and Pydantic AI.

---

<p align="center">
  <a href="https://forge.veritera.ai">Website</a> &middot; <a href="https://github.com/veritera-ai/forge-python">Documentation</a> &middot; <a href="https://forge.veritera.ai/trust">Trust & Security</a>
</p>
