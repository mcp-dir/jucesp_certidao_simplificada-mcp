# JUCESP: Certidão Simplificada

### JUCESP: Certidão Simplificada for Claude, ChatGPT and AI agents

Issues the simplified certificate of a company at JUCESP. Platform-hosted, no credentials, pay per query with prepaid credit.

- 📊 **1 tool**
- 🔒 **Read-only**
- 💬 **Works with any MCP client**: Claude Desktop, Cursor, VS Code, Cline, Continue
- 🔑 **Magic-link login (no password)**

[Portuguese version](README.md) · [Full docs (PT-BR)](docs/)

---

## One-click install

### Claude (Web and Desktop)

[➕ Open in Claude and connect](https://claude.ai/new?modal=add-custom-connector#settings/customize-connectors)

Manual: [claude.ai/customize/connectors](https://claude.ai/customize/connectors?surface=cowork) → **+** → **Add custom connector** → name `JUCESP: Certidão Simplificada`, URL `https://api.mcp.ai/p_jucesp_certidao_simplificada`.

### Cursor

[➕ Install in Cursor](cursor://anysphere.cursor-deeplink/mcp/install?name=jucesp_certidao_simplificada&config=eyJ1cmwiOiJodHRwczovL2FwaS5tY3AuYWkvcF9qdWNlc3BfY2VydGlkYW9fc2ltcGxpZmljYWRhIn0=)

### VS Code (Copilot Chat)

[➕ Install in VS Code](vscode:mcp/install?name=jucesp_certidao_simplificada&config=%7B%22type%22%3A%22http%22%2C%22url%22%3A%22https%3A%2F%2Fapi.mcp.ai%2Fp_jucesp_certidao_simplificada%22%7D)

### Any other MCP-over-HTTP client

```
https://api.mcp.ai/p_jucesp_certidao_simplificada
```

---

## 1 tool

| Tool | Description |
|---|---|
| `jucesp_certidao_simplificada_consultar` | Emite a certidão simplificada de uma empresa na JUCESP (comprova registro e situação por CNPJ, NIRE ou nome). |

---

## Pricing

See [docs/precos.md](docs/precos.md) (PT-BR).

---

## License

MIT — see [LICENSE](LICENSE). The MCP server at `api.mcp.ai/p_jucesp_certidao_simplificada` is proprietary (hosted); this repo (manifests, docs, skills) is MIT.
