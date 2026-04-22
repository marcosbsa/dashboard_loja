# 🛍️ Projeto Loja — Dashboard de Análise de vendas, clientes e desempenho comercial

> Análise completa de vendas, clientes e desempenho comercial de uma loja de moda — com dashboards interativos, projeções de faturamento e plano de ação estratégico.

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![DAX](https://img.shields.io/badge/DAX-25%20medidas-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Em%20análise-orange?style=for-the-badge)

---

<img width="1150" height="650" alt="1" src="https://github.com/user-attachments/assets/b1dc443b-930e-4042-87af-dbc57d8e3214" />
<img width="1151" height="648" alt="2" src="https://github.com/user-attachments/assets/2a80465b-1279-4298-88a0-3ae3a3ee9f54" />
<img width="1151" height="648" alt="3" src="https://github.com/user-attachments/assets/39f89096-f03f-41e4-ac9c-146202461917" />
<img width="1151" height="649" alt="4" src="https://github.com/user-attachments/assets/74582175-04ce-44e8-bfed-f09ef3c7f991" />

## 📊 Visão Geral

Este projeto contém a análise de dados de uma loja de moda cobrindo o período de **janeiro de 2022 a fevereiro de 2024**, com foco em:

- Evolução de faturamento e volume de vendas
- Segmentação de clientes por sexo, faixa etária e tipo (novo, recorrente, recuperado, retido)
- Desempenho por categoria de produto, marca e vendedor
- Diagnóstico da queda de vendas em 2024
- Projeções de faturamento em 3 cenários
- Plano de ação estratégico para reversão da queda

---

## 🔢 Métricas Principais

| Indicador | Valor |
|-----------|-------|
| Faturamento total (jan/22 – fev/24) | **R$ 1.219.860,87** |
| Produtos vendidos | **24.832 unidades** |
| Clientes únicos | **3.140** |
| Transações registradas | **5.000** |
| Vendedores ativos | **5** |
| Categorias | **3** (Acessórios, Roupas, Calçados) |
| Marcas | **10** |

---

## ⚠️ Diagnóstico da Queda

| Período | Faturamento | Variação |
|---------|-------------|----------|
| 2022 (12 meses) | R$ 584.933 | — |
| 2023 (12 meses) | R$ 553.084 | **-5,4%** |
| Jan/2024 | R$ 53.273 | +19,0% vs jan/23 |
| Fev/2024 | R$ 28.569 | **-46,3% vs jan/24** |

> 🚨 O colapso de fevereiro/2024 é o principal sinal de alerta. Uma queda de -46,3% em um único mês não é tendência — é evento. Investigação imediata necessária.

---

## 📈 Projeções 2024–2027

| Cenário | 2024E | 2025E | 2026E |2027E |
|---------|-------|-------|-------|-------|
| 🔴 Pessimista (sem ações) | R$ 490K | R$ 4350K | R$ 385K | R$ 342K |
| 🟡 Base (tendência histórica) | R$ 523K | R$ 494K | R$ 468K | R$ 442K |
| 🟢 Otimista (com plano de ação) | R$ 580K | R$ 609K | R$ 640K | R$ 672K |


---

## 🏆 Top Insights

1. **Público feminino** representa **70,6%** do faturamento — principal alavanca de crescimento
2. **Acessórios** é a categoria líder com R$ 456K (37% do total)
3. **49,3%** das vendas usam desconto — sem ganho proporcional de volume (problema de margem)

---

## 🛠️ Modelo de Dados (Power BI)

Esquema estrela com 5 tabelas principais:

```
dim_cliente     ──┐
dim_produto     ──┤── fato_venda ── dCalendario
dim_vendedor    ──┘
```

**25 medidas DAX** organizadas em pasta `Medidas`, incluindo:
- Segmentação de clientes: `Clientes_Novos`, `Clientes_Recorrentes`, `Clientes_Recuperados`, `Clientes_Retidos`
- Comparação temporal: `Total_Venda_Trimestre_Ant`, `Total_Vendas_Trimestre_Atual`
- Análise hierárquica: `%_Hierarquia_Sexo_Categoria`, `Pct_Qtd_Vendida_Sexo_Categoria`

---

## 📋 Plano de Ação (Resumo)

| # | Ação | Prioridade | Impacto |
|---|------|-----------|---------|
| 01 | Investigar colapso Fev/2024 | 🔴 Urgente | Alto |
| 02 | Campanha reativação público feminino | 🟠 Alta | Alto |
| 03 | Revisar política de descontos | 🟠 Alta | Médio |
| 04 | Capacitar equipe de vendas | 🟡 Média | Médio |
| 05 | Expandir Marcas 7, 8 e 1 | 🟡 Média | Médio |

 - O faturamento caiu 5,4% de 2022 para 2023, mas o problema agravou-se em fevereiro de 2024, colapsando 46,3% em relação a janeiro do mesmo ano. 
 - Para reverter essa situação de queda será necessário focar em estratégias visando campanhas bem trabalhadas e segmentadas, já que 70,6% do faturamento vem do público feminino, principalmente a faixa etária que corresponde as jovens-adultas e adultas, podendo dessa maneira ocorrer uma recuperação imediata do faturamento.
 - É necessário focar também na política de descontos, já que quase metade das vendas usa desconto, sem ganho proporcional de volume.

---

## 🔗 Fonte dos Dados

Os dados utilizados foram extraídos da plataforma de Cursos Xperiun

Os dados.csv foram tratados para análise no Power Query antes da modelagem e análise.
