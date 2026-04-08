# Análise de Vendas – Mercado do Ponto

## Descrição do Projeto
Este projeto tem como objetivo analisar os dados de vendas de um mercado de bairro, utilizando informações transacionais e agregadas por horário. A análise busca identificar padrões de vendas, comportamento dos clientes e oportunidades de melhoria.

Os dados abrangem o período de **janeiro a março de 2026** e incluem:

- Volume de vendas por horário
- Quantidade de clientes
- Transações via cartão

---

## Estrutura dos Dados

### 1. `vendas-por-horario-jan-mar.csv`
Base agregada com informações por hora:

| Coluna            | Descrição                          |
|------------------|----------------------------------|
| mes              | Mês da venda                     |
| hora             | Hora da venda                    |
| qtd_clientes     | Número de clientes               |
| qtd_produtos     | Quantidade de produtos vendidos  |
| total_venda      | Valor total vendido (R$)         |

Essa base permite análises de:
- Horários de pico
- Ticket médio
- Volume de vendas por período

---

### 2. `vendas-cartoes-jan-mar.csv`
Base detalhada de transações com cartão:

| Coluna                  | Descrição                          |
|------------------------|----------------------------------|
| Data da Transação      | Data da venda                    |
| Bandeira               | Bandeira do cartão               |
| Forma de Pagamento     | Crédito, débito ou PIX           |
| Valor Bruto            | Valor total da venda             |
| Valor Taxa             | Taxa cobrada                    |
| Valor Líquido          | Valor recebido                  |
| Status                 | Situação da transação            |

Essa base permite análises de:
- Meios de pagamento mais usados
- Taxas e custos financeiros
- Receita líquida real

---

## Objetivos do Projeto

- Identificar horários de maior faturamento
- Analisar comportamento de compra dos clientes
- Calcular ticket médio por hora
- Avaliar impacto das taxas de cartão
- Criar previsões de vendas futuras
- Apoiar decisões estratégicas do negócio

---

**A base de dados de vendas de cartão logicamente só mostram vendas de Débito, Crédito, Voucher e Pix. A base de dados de vendas por horário mostra todas as vendas nas maquininhas e as vendas em dinheiro no período de 01/01/26 até 31/03/26**

---

## Análises Realizadas

### Análise Exploratória (EDA)
- Distribuição de vendas por hora
- Evolução mensal de faturamento
- Correlação entre clientes, produtos e vendas
- Identificação de horários de pico

### Análise Financeira
- Receita bruta vs líquida
- Impacto das taxas de cartão
- Comparação entre formas de pagamento

### Comportamento do Cliente
- Média de produtos por cliente
- Ticket médio por horário
- Padrões de consumo ao longo do dia

---

## Possibilidades - Machine Learning

Este projeto pode evoluir para modelos preditivos:

### Previsão de Vendas
- Modelos de regressão (Linear, Random Forest, XGBoost)
- Séries temporais (ARIMA, Prophet)

### Clusterização de Horários
- Identificar padrões de consumo (K-Means)

### Classificação
- Prever dias/horários de alta demanda

---

## Dashboard (Power BI)

Indicadores (KPIs):

- Faturamento total
- Ticket médio
- Total de clientes
- Produtos vendidos
- Vendas por hora
- Distribuição por forma de pagamento
- Taxas totais pagas
- Comparação mensal

---

## Tecnologias Utilizadas

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Power BI
- Excel / CSV
- Machine Learning (Scikit-Learn)

---

## Conclusão

Este projeto demonstra como dados simples de um mercado de bairro podem gerar insights valiosos para aumentar faturamento, reduzir custos e melhorar a tomada de decisão.

---

## Autor

Projeto desenvolvido por **Rafael Porfirio**  
Focado em Análise de Dados, Ciência de Dados e Inteligência de Negócios.
