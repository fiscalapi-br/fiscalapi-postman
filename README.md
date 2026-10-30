# FiscalAPI — coleção Postman e OpenAPI

Coleção Postman e especificação OpenAPI 3.1 da [FiscalAPI](https://fiscalapi.com.br): Inscrição Estadual nos 27 estados, CNPJ, certidões (CND estadual, CND Federal, CNDT, CRF/FGTS), XML de NF-e por chave, SIGEF, CNIR e perfil do produtor rural.

| Arquivo | O que é |
|---|---|
| `FiscalAPI.postman_collection.json` | Coleção Postman v2.1, com exemplos de resposta (sucesso e erros) |
| `openapi-publico.json` | OpenAPI 3.1 dos endpoints públicos da API |

## Como usar

1. Crie sua conta em [app.fiscalapi.com.br](https://app.fiscalapi.com.br) e copie a chave de API no painel.
2. No Postman, clique em **Import** e escolha `FiscalAPI.postman_collection.json` (ou `openapi-publico.json`).
3. Na coleção, abra **Variables** e cole a chave em `apiKey`, na coluna *Current value*.
4. Envie qualquer requisição. A chave vai no cabeçalho `X-API-Key`.

O uso pela API exige um plano ativo ou créditos. Planos, limites e consumo de créditos estão na [documentação](https://docs.fiscalapi.com.br).

## SDKs

- Python: [fiscalapi-python](https://github.com/fiscalapi-br/fiscalapi-python)
- Node.js / TypeScript: [fiscalapi-node](https://github.com/fiscalapi-br/fiscalapi-node)
- PHP: [fiscalapi-php](https://github.com/fiscalapi-br/fiscalapi-php)
- n8n: [n8n-nodes-fiscalapi](https://github.com/fiscalapi-br/n8n-nodes-fiscalapi)

## Licença

MIT. Suporte: contato@fiscalapi.com.br
