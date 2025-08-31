# 🧠 Terapeuta Automatizado com N8N + IA (Groq)

Este projeto é um fluxo completo de automação criado com N8N que simula um atendimento terapêutico automatizado. Através da integração com a API de IA da Groq, o sistema interpreta mensagens recebidas via WhatsApp e responde com empatia, acolhimento e insights profundos, como um terapeuta humanizado.

## 🔧 Tecnologias utilizadas
- [N8N](https://n8n.io) (ferramenta de automação low-code)
- API da [Groq](https://groq.com) para geração de resposta com IA (modelo de linguagem open source)
- Webhook para entrada de mensagens
- Google Sheets para armazenamento e histórico
- API da z-API para envio da resposta via WhatsApp
- JSON e HTTP Requests (API REST)
- Memória contextual com `Simple Memory` para manter coerência nas conversas

## 🔁 Fluxo resumido

1. **Mensagem recebida** via Webhook (z-API)
2. **Verificação** se é conversa válida (não é grupo, broadcast, etc.)
3. **Extração e tratamento** da mensagem (nome, número, conteúdo)
4. **Armazenamento** dos dados no Google Sheets (Nome e número + ddd)
5. **Envio da mensagem para a IA** da Groq (via API REST + JSON)
6. **Resposta gerada com memória contextual**
7. **Envio da resposta** ao usuário pelo WhatsApp (via z-API)

## 🧠 Objetivo
Explorar na prática projetos com automação de processos utilizando APIs REST, integração com IA e manipulação de dados via N8N, de forma a simular um fluxo completo de atendimento inteligente e humanizado.

## 📸 Screenshots
*

## 📂 Estrutura de arquivos
- `.json` do workflow exportado
- Imagens (prints do fluxo)
- Código de exemplo da chamada para a API 

## ✨ Autor
Desenvolvido por Isaque Barbosa, como projeto pessoal de estudo e preparação para desenvolvimento com foco em automações, APIs e inteligência artificial.
