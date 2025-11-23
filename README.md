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

```mermaid
flowchart TD
    A[Usuária no Playground] 
    --> B{PrintMana\n(GPT-4o + Code Interpreter)}
    
    B --> C[Recebe mensagem\nex: “Dezembro: RH 2800...”]
    C --> D[Parseia os números dos setores]
    D --> E[Code Interpreter ativado automaticamente]
    
    subgraph "Intérprete de Código (ação funcional)"
        E --> F1[Cálculo do total\n13.600 páginas]
        E --> F2[Verifica excedente\n3.600 páginas]
        E --> F3[Valor excedente\nR$ 144,00]
        E --> F4[Fatura total\nR$ 1.344,00]
        E --> F5[Gera gráfico de barras\nmatplotlib]
        E --> F6[Monta e-mail de alerta]
    end
    
    F1 & F2 & F3 & F4 & F5 & F6 --> G[Resposta completa no chat]
    G --> H[Gráfico colorido + tabela + e-mail pronto]
    
    style B fill:#e91e63,stroke:#fff,color:#fff
    style E fill:#ff9800,stroke:#fff,color:#000
    style H fill:#4caf50,stroke:#fff,color:#fff### Diagrama de Arquitetura do PrintMana
(Fluxo completo do agente no Azure AI Foundry)

```mermaid
flowchart TD
    A[Usuária no Playground] 
    --> B{PrintMana\n(GPT-4o + Code Interpreter)}
    
    B --> C[Recebe mensagem\nex: “Dezembro: RH 2800...”]
    C --> D[Parseia os números dos setores]
    D --> E[Code Interpreter ativado automaticamente]
    
    subgraph "Intérprete de Código (ação funcional)"
        E --> F1[Cálculo do total\n13.600 páginas]
        E --> F2[Verifica excedente\n3.600 páginas]
        E --> F3[Valor excedente\nR$ 144,00]
        E --> F4[Fatura total\nR$ 1.344,00]
        E --> F5[Gera gráfico de barras\nmatplotlib]
        E --> F6[Monta e-mail de alerta]
    end
    
    F1 & F2 & F3 & F4 & F5 & F6 --> G[Resposta completa no chat]
    G --> H[Gráfico colorido + tabela + e-mail pronto]
    
    style B fill:#e91e63,stroke:#fff,color:#fff
    style E fill:#ff9800,stroke:#fff,color:#000
    style H fill:#4caf50,stroke:#fff,color:#fff

## Prints do Processo

| Etapa                                    | Print               |
|------------------------------------------|---------------------|
| Criação do projeto Foundry               | 01-projeto          |
| Instruções completas                     | 02-instrucoes       |
| Tool Code Interpreter ativada            | 03-tool             |
| Teste 1 – Dentro da cota (9.000 páginas) | 04-normal           |
| Teste 2 – Com excedente + e-mail + gráfico | 05-excedente      |




## Demonstração Real – Mês com excedente (13.600 páginas)

![Gráfico + e-mail gerado pela PrintMana](prints/06-grafico.png)

**E-mail automático gerado:**
