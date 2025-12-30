# Racional de Visualização – Dashboard Vendas, Custo, Margem de Lucro e KPI

Este documento descreve o racional por trás da escolha e uso de cada visualização presente no **Dashboard - Vendas, Custo, Margem de Lucro e KPI**, desenvolvido no Microsoft Power BI como parte do LAB II – CAP 3 da Escola Data Science Academy.

## 1. Visão Geral

O objetivo deste dashboard é apoiar a análise de desempenho comercial sob a perspectiva de vendas, custos logísticos, lucro e margem de lucro, permitindo que gestores avaliem eficiência operacional e resultados financeiros ao longo do tempo.

Cada visual foi selecionado com base na pergunta de negócio que deveria responder, priorizando clareza, comparabilidade e suporte à tomada de decisão.

---

## 2. Racional por Visualização

### 2.1 Gráfico de Cascata – Total de Vendas por Modo de Envio

**Pergunta de negócio:** Qual foi o total de valor de venda considerando cada modo de envio dos pedidos?

**Justificativa:**
O gráfico de cascata é adequado para demonstrar como valores intermediários contribuem para um total acumulado. Neste contexto, ele permite visualizar de forma clara a contribuição de cada modo de envio (Classe Padrão, Segunda Classe, Primeira Classe e Mesmo Dia) até o valor total de vendas.

**Valor para o negócio:**
Facilita a identificação dos modos de envio mais relevantes em termos de faturamento e apoia decisões relacionadas à estratégia logística e comercial.

---

### 2.2 Treemap – Média do Custo de Envio por Mercado

**Pergunta de negócio:** Quais mercados tiveram o maior custo médio de envio dos produtos vendidos?

**Justificativa:**
O treemap é indicado para comparações hierárquicas e proporcionais. Ele permite comparar rapidamente o custo médio de envio entre diferentes mercados, utilizando área e cor como elementos visuais de destaque.

**Valor para o negócio:**
Auxilia na identificação de mercados com maior pressão de custo logístico, apoiando estratégias de renegociação, revisão de rotas ou ajustes de preço.

---

### 2.3 KPI – Média do Valor de Venda versus Meta

**Pergunta de negócio:** A empresa manteve a média de valor de venda mensal dentro da meta de 350?

**Justificativa:**
O visual de KPI é apropriado para comparação direta entre um valor observado e uma meta definida. Ele fornece leitura imediata do desempenho atual em relação ao objetivo estratégico.

**Valor para o negócio:**
Permite rápida avaliação de aderência à meta corporativa e facilita a comunicação executiva sobre performance mensal.

---

### 2.4 Gráfico de Rosca – Média de Lucro por Categoria

**Pergunta de negócio:** Qual categoria de produto apresentou maior lucro médio?

**Justificativa:**
O gráfico de rosca é adequado para análises categóricas com poucas variáveis, permitindo comparação proporcional entre categorias sem comprometer a legibilidade.

**Valor para o negócio:**
Evidencia quais categorias são mais rentáveis em média, apoiando decisões de portfólio, precificação e foco comercial.

---

### 2.5 Gráfico de Linha – Evolução da Margem de Lucro ao Longo do Tempo

**Pergunta de negócio:** Qual foi o comportamento da margem de lucro ao longo do tempo?

**Justificativa:**
O gráfico de linha é o mais indicado para análises temporais, pois evidencia tendências, variações e possíveis padrões sazonais na margem de lucro.

**Valor para o negócio:**
Permite monitorar estabilidade ou volatilidade da margem ao longo dos períodos, apoiando ações corretivas e planejamento estratégico.

---

## 3. Considerações Finais

A combinação de diferentes tipos de gráficos neste dashboard foi pensada para equilibrar visão executiva e capacidade analítica. Cada visual cumpre um papel específico, evitando redundância e maximizando o valor informacional entregue ao usuário final.
