<div align="center">
  <img src="assets/logo.png" width="148" alt="0xMiller Labs mark">
  <h3>Mark Miller</h3>
  <p>Senior Backend Engineer · AI systems · Web3 infrastructure</p>
  <p>
    <strong>Python</strong> · <strong>Go</strong> · <strong>FastAPI</strong> ·
    <strong>Ollama / vLLM</strong> · <strong>Kafka</strong> · <strong>Kubernetes</strong> ·
    <strong>EVM</strong>
  </p>
  <p>
    <a href="https://0xmmiller.github.io">site</a> ·
    <a href="https://github.com/0xmmiller/architecture">architecture</a> ·
    <a href="https://github.com/0xmmiller/agentkit">agentkit</a> ·
    <a href="https://github.com/0xmmiller/architecture/blob/main/adr/008-local-model-runtime.md">ADR-008</a>
  </p>
</div>

---

**Currently building**

| | | |
| --- | --- | --- |
| **Atlas** | Digital asset operations. Python domain, Go notify, operator UI, **agent tools on local models** | [arch](https://github.com/0xmmiller/architecture) · [web](https://github.com/0xmmiller/atlas-web) · [notify](https://github.com/0xmmiller/notification-service) |
| **AgentKit** | Durable agent backend. Ollama/vLLM first, MCP-shaped tools, Atlas `get_portfolio` / `create_intent` | [repo](https://github.com/0xmmiller/agentkit) |
| **PyScale** | Backend performance lab — p50/p95/p99 | [repo](https://github.com/0xmmiller/pyscale) |
| **ChainKit** | Reorgs, RPC failover, log splitters | [repo](https://github.com/0xmmiller/chainkit) |

```mermaid
flowchart TB
  MM[Mark Miller]
  LAB[0xMiller Labs]
  MM --> LAB
  LAB --> A[Atlas]
  LAB --> P[PyScale]
  LAB --> C[ChainKit]
  LAB --> K[AgentKit]
  A --> PY[Python domain]
  A --> GO[Go notify]
  A --> WEB[atlas-web]
  K --> LOCAL[Ollama / vLLM]
  K --> TOOLS[Atlas tools]
```

Agents are a **runtime behind Atlas**, not a chatbot page. Local models are the default; a vendor URL is an env var ([ADR-008](https://github.com/0xmmiller/architecture/blob/main/adr/008-local-model-runtime.md)).

**0xMiller Labs is a personal engineering lab, not an employer.**
