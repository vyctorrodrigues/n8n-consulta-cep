# n8n-consulta-cep
Workflow criado no n8n para consulta de endereço via CEP.

## Como funciona
1. Recebe um CEP via webhook (GET)
2. Consulta a API pública do ViaCEP
3. Retorna o endereço completo em JSON

## Tecnologias
- n8n (self-hosted)
- API ViaCEP (gratuita)
## Como usar
Faça uma requisição GET substituindo o CEP:

http://localhost:5678/webhook/consulta-cep?cep=SEU_CEP_AQUI

**Exemplo:**
http://localhost:5678/webhook/consulta-cep?cep=24020971
