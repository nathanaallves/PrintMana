# PrintMana – Controle Inteligente de Outsourcing de Impressoras  
**Azure Frontier Girls – Build Your First Copilot Challenge**  
Entrega individual – 23/11/2025

## Objetivo do Agente
Assistente corporativo que controla o consumo de impressões por setor (RH, TI, Comercial, Financeiro), calcula excedentes do contrato de outsourcing e gera automaticamente:
- Fatura mensal completa
- Gráfico de consumo por setor
- E-mail de alerta quando houver excedentes

**Contrato configurado:**
- 10.000 páginas inclusas → R$ 1.200,00/mês
- Excedente → R$ 0,04 por página

## Ação Funcional Implementada (Code Interpreter)
- Cálculo automático de excedentes e fatura
- Geração de gráficos de barras comparativos
- Geração de e-mail profissional de alerta

### Diagrama de Arquitetura do PrintMana
(Fluxo completo do agente no Azure AI Foundry)

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/c9722012-2b83-484e-8978-9dec4fcb9efa" />

| Etapa                                    | Print               |
|------------------------------------------|---------------------|
| Criação do projeto Foundry               | 01-projeto          |
| Instruções completas                     | 02-instrucoes       |
| Tool Code Interpreter ativada            | 03-tool             |
| Teste 1 – Dentro da cota (9.000 páginas) | 04-normal           |
| Teste 2 – Com excedente + e-mail + gráfico | 05-excedente      |


