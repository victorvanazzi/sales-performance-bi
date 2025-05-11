# Análise de Desempenho de Vendas

![](https://img.shields.io/badge/Power%20BI-Dashboard-yellow.svg)

![](https://img.shields.io/badge/DAX-Avan%C3%A7ado-blue.svg)

![](https://img.shields.io/badge/Status-Completo-brightgreen.svg)

> Dashboard analítico para monitoramento de desempenho financeiro e segmentação estratégica de produtos para uma varejista global de eletrônicos.

## Ecossistema de Projetos

Este repositório faz parte de um ecossistema com três projetos modulares:

| Repositório | Função | Descrição |
| --- | --- | --- |
| [`core-data-pipeline`](https://github.com/victorvanazzi/core-data-pipeline) | Ingestão e Transformação | Pipeline de dados com arquitetura Medallion (Bronze → Silver → Gold) |
| **`sales-performance-bi`** | **Visualização** | **Análise de desempenho comercial no Power BI** |
| [`sales-demand-forecasting`](https://github.com/victorvanazzi/sales-demand-forecasting) | Modelagem Preditiva | Previsão de vendas mensais com séries temporais |

## Objetivo do Projeto

O dashboard desenvolvido visa auxiliar a varejista global de eletrônicos na tomada de decisões estratégicas para aumentar receitas e impulsionar o crescimento do negócio através de:

1. **Monitoramento de KPIs financeiros** - Acompanhamento de receita, lucro bruto, ticket médio e volume de vendas
2. **Análise de segmentação de produtos** - Classificação estratégica do portfólio para identificar oportunidades
3. **Identificação de padrões de sazonalidade** - Reconhecimento de ciclos de vendas para melhor planejamento
4. **Avaliação geográfica de mercados** - Mapeamento de desempenho por país e canal de vendas

## Estrutura do Repositório

```
sales-performance-bi/
│
├── powerbi/                    # Arquivos do projeto no Power BI
│
└── README.md                    # Documentação do projeto
```

## Estrutura do Dashboard

O dashboard está estruturado em duas páginas principais:

### 1. Dashboard Financeiro

- **KPIs principais:** Receita Total, Lucro Bruto, Ticket Médio, Clientes Únicos, Volume de Vendas
- **Gráfico de Desempenho Financeiro:** Visualização da evolução mensal da Receita e Lucro Bruto
- **Participação de Receita:** Distribuição percentual por categoria de produtos
- **Receita por Mercado:** Análise detalhada das receitas geradas por país/canal
- **Top 5 Subcategorias:** Identificação das subcategorias de produtos mais rentáveis

### 2. Dashboard de Produtos

- **KPIs principais:** Receita Total, Lucro Bruto, Ticket Médio, Margem Bruta
- **Segmentação Estratégica:** Classificação dos produtos em categorias estratégicas (Estrela, Nicho, Problema e Descontinuar)
- **Ranking de Produtos:** Análise hierárquica detalhada por categoria e subcategoria
- **Receita por Categoria e Subcategoria:** Exploração interativa detalhada do faturamento

## Principais Insights

### Desempenho Financeiro

1. **Impacto da Pandemia:** Queda de 49% na receita em 2020 em relação a 2019; lucro bruto se manteve positivo, indicando controle eficiente de custos.
2. **Sazonalidade:** Vendas caem no primeiro semestre e aumentam no segundo semestre, impulsionadas por datas comerciais e festividades.
3. **Distribuição geográfica**: Mercados com maior concentração de receita são EUA (4,2 milhões), vendas online (2,1 milhões) e Reino Unido (0,8 milhões). Reino Unido e Canadá apresenta potencial subexplorado.
4. **Estabilidade de margens**: Consistência notável na margem bruta ao longo do período analisado (2016-2021), oscilando entre 58-60%.

### Análise de Produtos

1. **Categorias dominantes**: As cinco principais categorias em receita são:
    - Computers
    - Cell phones
    - Cameras and camcorders
    - Home Appliances
    - TV and Video
2. **Subcategorias mais lucrativas**:
    - Desktops
    - Projectors and Screens
    - Laptops
    - Touch Screen Phones
    - Camcorders
3. **Produtos estrela**: Identificados 9 produtos (códigos 444, 416, 428, 422, 433, 455, 433, 450, 438) da categoria Computers com alta margem (67%) e alto volume de vendas.
4. **Produtos de nicho**: Identificados produtos com potencial inexplorado, principalmente nas categorias Home Appliances e TV & Video, que poderiam ter seu potencial melhor aproveitado.
5. **Produtos problema**: Diversos produtos (principalmente da categoria Computers) que possuem grande volume de venda mas têm margem baixa, necessitando revisão de margem de lucro.
6. Produtos que necessitam revisão: Diversos produtos (principalmente da categoria Home Appliances) possuem baixa margem e baixo volume de vendas.

## Recomendações de Negócio

### 1. Aproveitar o Potencial dos Produtos Estrela

**Ação**: Implementar estratégia de "compre e leve junto" (bundle) relacionando produtos estrela com produtos de nicho ou com produtos problema.

**Benefício**: Alavancar o sucesso das linhas de computadores de alta margem para impulsionar a venda de outros produtos com margem menor ou menos expostos.

**Implementação**: Desenvolver pacotes promocionais que combinem desktops ou laptops (estrelas) com produtos relacionados de outras categorias.

### 2. Revisão do Portfólio de Produtos

**Ação**: Conduzir revisão completa do portfólio, especialmente da categoria Home Appliances, que concentra a maioria dos produtos candidatos à descontinuação.

**Benefício**: Redução de custos operacionais e de inventário, com foco em produtos de maior rentabilidade.

**Implementação**: Estabelecer comitê de revisão trimestral e definir critérios claros de descontinuação para produtos com baixa margem e baixo volume por período contínuo.

### 3. Expansão Estratégica no Canadá

**Ação**: Desenvolver plano de expansão específico para o mercado canadense, aproveitando a proximidade geográfica e cultural com os EUA.

**Benefício**: Diversificação de mercados com menor custo operacional em comparação à expansão para mercados mais distantes.

**Implementação**: Utilizar a infraestrutura logística existente nos EUA e adaptar estratégias bem-sucedidas do mercado americano.

### 4. Estratégia para Produtos Problema

**Ação**: Revisar a estrutura de preços ou custos dos produtos da categoria Computers identificados como "problema" (códigos 434, 423, 458, 424, 425, 446, 440, 452, 419, 436).

**Benefício**: Aumento de margem bruta em produtos que já possuem bom volume de vendas.

**Implementação**: Negociar melhores condições com fornecedores ou ajustar preços gradualmente de forma a não impactar negativamente o volume de vendas.

### 5. Estratégia Sazonal Ajustada

**Ação**: Adaptar estratégias de marketing e promoções de acordo com a sazonalidade identificada, aumentando investimentos no Q3 e Q4 e utilizando Q1 e Q2 para testar novos produtos ou liquidar estoque.

**Benefício**: Otimização do orçamento de marketing e maior eficiência nas ações promocionais.

**Implementação**: Desenvolver calendário anual de marketing e promoções alinhado com os ciclos de compra identificados.

## Tecnologias e Ferramentas

| Categoria | Ferramentas |
| --- | --- |
| **Visualização** | Power BI Desktop |
| **Modelagem de Dados** | Modelo Star Schema via Databricks |
| **Linguagem de Consulta** | DAX (Data Analysis Expressions) |
| **Integrações** | Databricks (Camada Gold) |
| **Controle de Versão** | Git/GitHub |

## Modelo Dimensional

### Tabelas Principais

- **Dimensões:** `dim_date`, `dim_product`, `dim_store`
- **Fatos:** `fact_sales`

## Melhorias Futuras

1. **Integração com modelos preditivos** - Incorporar dados de previsão do projeto `sales-demand-forecasting` para análise prospectiva.
2. **Expansão para análise geográfica** - Aprofundar análises do desempenho do negócio por países, cidades e lojas, com o objetivo de apresentar insights mais precisos no tema.
3. Expansão para análise de clientes - Fazer análises que buscam compreender os clientes mais valiosos, procurar oportunidades e entender padrões de consumo.

## Observações

- Os dados foram extraídos do [Maven Analytics Data Playground](https://www.mavenanalytics.io/data-playground), dataset "Global Electronics Retailer".
- A análise considera dados até fevereiro de 2021, o que limita a visualização completa do cenário pós-pandemia.