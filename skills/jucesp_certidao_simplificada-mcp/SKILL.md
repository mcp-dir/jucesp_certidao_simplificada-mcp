---
name: jucesp_certidao_simplificada-mcp
description: Skill da REST API do JUCESP: Certidão Simplificada na MCP.AI: 1 endpoint em /api/jucesp_certidao_simplificada. Emite a certidão simplificada de uma empresa na JUCESP (comprova registro e situação por CNPJ, NIRE ou nome). Hospedado pela plataforma, sem credenciais, pague por consulta com crédito pré-pago. Autentique com workspace API key (sk_live) gerada em app.mcp.ai/settings/api-keys. Use quando o usuário pedir algo coberto pelos endpoints.
---

# JUCESP: Certidão Simplificada — REST API skill

Você tem acesso à **JUCESP: Certidão Simplificada** REST API na MCP.AI.

> Emite a certidão simplificada de uma empresa na JUCESP (comprova registro e situação por CNPJ, NIRE ou nome). Hospedado pela plataforma, sem credenciais, pague por consulta com crédito pré-pago.

## Base URL

```
https://api.mcp.ai/api/jucesp_certidao_simplificada
```

Todo endpoint é um **POST** na Base URL + o path abaixo. Os parâmetros vão no corpo JSON.

## Autenticação

Inclua em toda request:

```
Authorization: Bearer sk_live_...
Content-Type: application/json
```

> Gere sua chave em **https://app.mcp.ai/settings/api-keys** (workspace API key `sk_live_…`, não expira, revogável). Uma única chave serve pra todos os seus MCPs.

## Formato de resposta

```json
{ "ok": true, "tool": "<tool_id>", "result": <payload> }
```

## Exemplo cURL

```bash
curl -X POST https://api.mcp.ai/api/jucesp_certidao_simplificada/consultar \
  -H "Authorization: Bearer sk_live_..." \
  -H "Content-Type: application/json" \
  -d '{}'
```

## Reportar problemas

Se um endpoint retornar erro, vazio ou dado inesperado, reporte (não desista calado): **POST /api/jucesp_certidao_simplificada/report** com `{ "message": "...", "context"?: "...", "conversation"?: [...] }`. Isso notifica o time da MCP.AI.

## Endpoints (1)

#### `jucesp_certidao_simplificada_consultar`

Emite a certidão simplificada de uma empresa na JUCESP (comprova registro e situação por CNPJ, NIRE ou nome). _(POST /api/jucesp_certidao_simplificada/consultar)_

| Parâmetro | Tipo | Obrigatório | Descrição |
|---|---|---|---|
| `login_cpf` | string | Não | Parâmetro de consulta "login_cpf". |
| `login_senha` | string | Não | Parâmetro de consulta "login_senha". |
| `pkcs12_cert` | string | Não | Parâmetro de consulta "pkcs12_cert". |
| `pkcs12_pass` | string | Não | Parâmetro de consulta "pkcs12_pass". |
| `nire` | string | Não | Parâmetro de consulta "nire". |
| `name` | string | Não | Parâmetro de consulta "name". |
| `cnpj` | string | Não | Parâmetro de consulta "cnpj". |

---

Este MCP também funciona via **conexão MCP** (Claude / Cursor) em `https://api.mcp.ai/p_jucesp_certidao_simplificada` — veja o [README](../../README.md). A skill acima é pra consumir a **REST API** direto (agente próprio / código).
