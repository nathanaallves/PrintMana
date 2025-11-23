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

## Prints do Processo

| Etapa                                    | Print                                            |
|------------------------------------------|--------------------------------------------------|
| Criação do projeto Foundry               | ![01-projeto](prints/01-projeto.png)             |
| Instruções completas                     | ![02-instrucoes](prints/02-instruções.png)       |
| Tool Code Interpreter ativada            | ![03-tool](prints/03-tool.png)                   |
| Teste 1 – Dentro da cota (9.000 páginas) | ![04-normal](prints/04-normal.png)               |
| Teste 2 – Com excedente + e-mail + gráfico | ![05-excedente](prints/05-excedente.png)       |
| Gráfico gerado automaticamente           | ![06-grafico](prints/06-grafico.png)             |
| E-mail de alerta gerado                  | ![07-email](prints/07-email.png)                 |
| Recursos deletados (zero custo)          | ![08-delete](prints/08-delete.png)               |

## Demonstração Real – Mês com excedente (13.600 páginas)

![Gráfico + e-mail gerado pela PrintMana](prints/06-grafico.png)

**E-mail automático gerado:**
