# FiscalAPI — coleção Postman e OpenAPI

Coleção Postman e especificação OpenAPI 3.1 da [FiscalAPI](https://fiscalapi.com.br): Inscrição Estadual nos 27 estados, CNPJ, certidões (CND estadual, CND Federal, CNDT, CRF/FGTS), XML de NF-e por chave (com certificado, ou cópia para leitura sem certificado), NFS-e por chave, Simples Nacional, SIGEF, CNIR e perfil do produtor rural.

| Arquivo | O que é |
|---|---|
| `FiscalAPI.postman_collection.json` | Coleção Postman v2.1, com exemplos de resposta (sucesso e erros) |
| `openapi-publico.json` | OpenAPI 3.1 dos endpoints públicos da API |

A coleção também está publicada no Postman: [FiscalAPI na Postman API Network](https://www.postman.com/fiscalapi-2630264/workspace/fiscalapi). Dá para abrir direto no navegador ou fazer um fork para o seu workspace.

## Como usar

1. Crie sua conta em [app.fiscalapi.com.br](https://app.fiscalapi.com.br) e copie a chave de API no painel.
2. No Postman, clique em **Import** e escolha `FiscalAPI.postman_collection.json` (ou `openapi-publico.json`).
3. Na coleção, abra **Variables** e cole a chave em `apiKey`, na coluna *Current value*.
4. Envie qualquer requisição. A chave vai no cabeçalho `X-API-Key`.

Pela API, toda consulta pede plano ou saldo de recarga, a partir de R$ 50 por mês. As 10 consultas grátis do mês são só no painel: teste lá antes de assinar. Sem plano nem saldo, a API responde `402` (`LIMITE_ATINGIDO`). Sem chave, `403` (`API_KEY_ERROR`). Planos, limites e consumo de créditos estão na [documentação](https://docs.fiscalapi.com.br).

## SDKs

- Python: [fiscalapi-python](https://github.com/fiscalapi-br/fiscalapi-python)
- Node.js / TypeScript: [fiscalapi-node](https://github.com/fiscalapi-br/fiscalapi-node)
- PHP: [fiscalapi-php](https://github.com/fiscalapi-br/fiscalapi-php)
- n8n: [n8n-nodes-fiscalapi](https://github.com/fiscalapi-br/n8n-nodes-fiscalapi)

## Links

- Documentação: [docs.fiscalapi.com.br](https://docs.fiscalapi.com.br)
- Guias (Excel, Google Sheets, n8n, Make, Power Automate, Python, Node.js, PHP): [docs.fiscalapi.com.br/docs/guias](https://docs.fiscalapi.com.br/docs/guias)
- Especificação OpenAPI sempre atualizada: [docs.fiscalapi.com.br/openapi.json](https://docs.fiscalapi.com.br/openapi.json)
- Servidor MCP: [fiscalapi-br/fiscalapi-mcp](https://github.com/fiscalapi-br/fiscalapi-mcp)
- Para desenvolvedores: [fiscalapi.com.br/desenvolvedores](https://fiscalapi.com.br/desenvolvedores/)

## Licença

MIT. Suporte: contato@fiscalapi.com.br
