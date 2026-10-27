# 🚀 Automação e Orquestração de IA B2B (Multi-Agente)

## 📋 Visão Geral

Este repositório apresenta uma arquitetura avançada de automação corporativa e orquestração de Inteligência Artificial desenvolvida em um ciclo ágil de **duas semanas** para o setor atacadista de grande porte. O sistema atua como uma central de atendimento B2B multi-agente via WhatsApp, roteando e resolvendo demandas de múltiplos departamentos com foco em eficiência, escalabilidade e redução de atrito operacional.

## 🏗️ Arquitetura e Tecnologias

* **Orquestrador:** n8n (Self-hosted em VPS)

* **Modelos de IA (LLMs):** Google Gemini (via Google AI Studio)

* **Integração WhatsApp:** Evolution API

* **Gerenciamento de Contexto:** Google Sheets / PostgreSQL

* **Infraestrutura:** Docker & Docker Compose

* **Técnicas Aplicadas:** Arquitetura Multi-Agente, RAG (Retrieval-Augmented Generation), Fine-Tuning e Prompt Engineering avançado.

## 🤖 Agentes e Roteamento Departamental

O fluxo orquestra o atendimento inicial (Triagem Nível 1) e distribui as demandas de forma inteligente para os seguintes especialistas:

1. **Financeiro (Joy):** Tratativa de 2ª via de boletos, recepção de comprovantes PIX, status de faturamento e negociação de pendências.

2. **Comercial / Representantes:** Encaminhamento de orçamentos, disponibilidade de estoque, tabelas de preço e novos pedidos.

3. **Marketing:** Distribuição automatizada de catálogos promocionais e materiais de mídia.

4. **SAC & Suporte:** Triagem de atrasos logísticos, avarias, trocas e devoluções com escalonamento de prioridade.

5. **Recursos Humanos (RH):** Recepção de currículos e informações sobre vagas.

## ⚙️ Implementação Técnica e Segurança (Guardrails)

* **Design Multi-Agente:** Orquestração de múltiplos agentes especializados operando de forma colaborativa no mesmo pipeline de atendimento.

* **RAG (Retrieval-Augmented Generation):** Ingestão de contexto dinâmico para consultas precisas de status de clientes e faturamento.

* **Fine-Tuning Comportamental:** Especialização dos agentes para adequação ao tom de voz corporativo e fluxos de decisão departamentais.

* **Zero Alucinação Financeira:** Travas rígidas via prompt engineering que impedem o modelo de confirmar pagamentos ou inventar valores comerciais.

* **Consciência Temporal:** Injeção de variáveis de tempo real (`$now`) para adaptação do tom de voz e respostas fora do horário comercial.

* **Memória de Contexto:** Implementação de `Memory Buffer Window` no n8n para manter coerência no histórico recente da conversa.

**Desenvolvido por:**
**Thiago Rafael de Souza Gomes**
*AI and Systems Architect | AI Agents and LLM Integration | Industrial Automation | Process Automation with n8n | ERP/CRM and API Integrations*
