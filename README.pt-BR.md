# Dashboard – Vendas, Custo, Margem de Lucro e KPI

## 1. Visão Geral do Projeto
Este projeto apresenta um dashboard analítico desenvolvido no Microsoft Power BI com o objetivo de apoiar a tomada de decisão empresarial por meio da análise de desempenho de vendas, custos logísticos, lucro e margem de lucro ao longo do tempo.

O dashboard foi desenvolvido como parte do **LAB II – Capítulo 3** do programa *Microsoft Power BI para Business Intelligence e Data Science* da **Data Science Academy (DSA)**.

A solução foca em transformar dados transacionais brutos em insights acionáveis por meio de visualizações claras e orientadas ao negócio.
---
## 2. Perguntas de Negócio
O dashboard foi projetado para responder às seguintes perguntas de negócio:

* Qual é o valor total de vendas por modo de envio?
* Quais mercados apresentam o maior custo médio de envio?
* A empresa está atingindo sua meta de valor médio de vendas mensal de 350?
* Qual categoria de produto possui o maior lucro médio?
* Como a margem de lucro se comportou ao longo do tempo?
---
## 3. Conjuntos de Dados (Datasets)
Quatro conjuntos de dados em formato CSV foram fornecidos para esta análise:

### 3.1 Clientes (Customers)
**Campos:**
* ID do Cliente (PK)
* Nome do Cliente
* Segmento
* Cidade
* Estado
* País
* Mercado
* Região

**Registros:** 1.590  
**Qualidade dos Dados:** Sem valores nulos, sem campos vazios, sem duplicatas.
---
### 3.2 Produtos (Products)
**Campos:**
* ID do Produto (PK)
* Categoria
* Subcategoria
* Nome do Produto

**Registros:** 10.293  
**Qualidade dos Dados:** Sem valores nulos; chaves primárias duplicadas identificadas.
---
### 3.3 Pedidos (Orders)
**Campos:**
* ID do Pedido (PK)
* Data do Pedido
* Data de Envio
* Modo de Envio
* Prioridade do Pedido

**Registros:** 25.036  
**Qualidade dos Dados:** Sem valores nulos; chaves primárias duplicadas identificadas.
---
### 3.4 Vendas (Sales)
**Campos:**
* ID do Pedido (FK)
* ID do Cliente (FK)
* ID do Produto (FK)
* Valor de Venda
* Quantidade Vendida
* Custo de Envio

**Registros:** 51.290  
**Qualidade dos Dados:** Sem valores nulos; registros duplicados identificados.
---
## 4. Preparação e Modelagem de Dados
Durante a fase exploratória, foram identificadas chaves primárias duplicadas nas tabelas de Produtos e Pedidos. Como chaves duplicadas comprometem a integridade relacional no Power BI, esses registros foram removidos após validação.

Além disso, o Power BI não reconheceu automaticamente os cabeçalhos das colunas, exigindo a aplicação manual da opção "Usar a Primeira Linha como Cabeçalho".
---
### 4.1 Medidas Calculadas (DAX)
Com base nos requisitos de negócio, duas medidas adicionais foram criadas:

* **Lucro** = `Sales[Valor de Venda] - Sales[Custo de Envio]`
* **Margem de Lucro (%)** = `ROUND(DIVIDE([Lucro], Sales[Valor de Venda]) * 100, 2)`

Essas medidas permitiram a análise de lucro e margem entre categorias, mercados e períodos de tempo.
---
## 5. Visualizações do Dashboard
O dashboard inclui os seguintes componentes visuais:

* **Gráfico de Cascata (Waterfall):** Valor total de vendas por modo de envio.
* **Treemap:** Custo médio de envio por mercado.
* **Indicador de KPI:** Valor médio de vendas comparado à meta.
* **Gráfico de Rosca:** Lucro médio por categoria de produto.
* **Gráfico de Linhas:** Tendência da margem de lucro ao longo do tempo.

Cada visualização foi selecionada com base nas melhores práticas de visualização de dados e está alinhada a uma pergunta de negócio específica.

Para uma explicação detalhada da lógica das visualizações, consulte:  
📄 [Lógica de Visualização de Dados](LINK_PARA_SEU_ARQUIVO)
---
## 6. Filtros e Interatividade
O dashboard permite que os usuários filtrem os dados por:
* Ano
* Trimestre
* Outras dimensões temporais

Esses filtros possibilitam a exploração dinâmica do desempenho em diferentes períodos.
---
## 7. Ferramentas e Tecnologias
* Microsoft Power BI
* DAX (Data Analysis Expressions)
* Datasets em CSV
---
## 8. Principais Conclusões (Insights)
* O modo de envio tem um impacto significativo na contribuição total de vendas.
* Os custos logísticos variam consideravelmente entre os mercados.
* O valor médio de vendas permanece abaixo da meta definida.
* A lucratividade difere substancialmente entre as categorias de produtos.
* A margem de lucro apresenta flutuações ao longo do tempo, exigindo monitoramento contínuo.
---
## 9. Autor
**Leandro Álax** Data Analytics | Business Intelligence | Power BI
---
## 10. Aviso Legal (Disclaimer)
Os conjuntos de dados utilizados neste projeto foram fornecidos exclusivamente para fins educacionais pela Data Science Academy e não representam dados reais de uma empresa.
