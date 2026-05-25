# n8n - Consulta CEP

Workflow criado no n8n para consulta de endereço via CEP com validação de entrada.

## Como funciona
1. Recebe um CEP via webhook (GET)
2. Valida se o CEP tem exatamente 8 dígitos
3. Se válido: consulta a API pública do ViaCEP e retorna o endereço completo
4. Se inválido: retorna mensagem de erro clara

## Como usar
Faça uma requisição GET substituindo o CEP:

http://localhost:5678/webhook/consulta-cep?cep=SEU_CEP_AQUI

**Exemplo válido:**
http://localhost:5678/webhook/consulta-cep?cep=24020971

**Exemplo inválido:**
http://localhost:5678/webhook/consulta-cep?cep=123

## Tecnologias
- n8n (self-hosted)
- API ViaCEP (gratuita)
