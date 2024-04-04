# Modelagem Dimensional: Entendendo os Principais Modelos

![dimensional](https://github.com/CarlosJuncher03/ModelosDimensionais/assets/145303814/ed1baf8b-6643-4d25-b459-91056446ea0c)

A modelagem dimensional é uma técnica de design de banco de dados amplamente utilizada em sistemas de Data Warehouse e Business Intelligence (BI). Ela organiza dados de forma intuitiva para facilitar a análise e o reporting, tornando-a essencial para o suporte à tomada de decisões baseadas em dados. Neste artigo, exploraremos os principais modelos de modelagem dimensional, explicando suas características, por que receberam esses nomes, e como cada um funciona.

## Modelo de Esquema Estrela (Star Schema)

![STAR](https://github.com/CarlosJuncher03/ModelosDimensionais/assets/145303814/0fa7184d-7159-49b8-b6a5-e43d97d4b975)

### Descrição
O modelo de esquema estrela é o estilo de modelagem dimensional mais simples e comum. Consiste em uma tabela de fatos central, que armazena medidas quantitativas e chaves estrangeiras para tabelas de dimensão relacionadas, que contêm atributos descritivos.

### Como Funciona
As tabelas de dimensão são ligadas à tabela de fatos por meio de chaves estrangeiras. Cada tabela de dimensão representa um vetor de análise (como tempo, produto, ou cliente), enquanto a tabela de fatos registra eventos ou transações, incluindo métricas como vendas ou custos.

## Modelo de Esquema Floco de Neve (Snowflake Schema)

![neve](https://github.com/CarlosJuncher03/ModelosDimensionais/assets/145303814/516db72e-b961-4d2b-ae77-48211c2832cc)

### Descrição
O esquema floco de neve é uma variação do esquema estrela, onde as tabelas de dimensão são normalizadas, dividindo-as em sub-dimensões. Isso reduz a redundância de dados e pode melhorar a eficiência do armazenamento.

### Como Funciona
Além da tabela de fatos central, as tabelas de dimensão podem ser ligadas a outras tabelas que fornecem informações mais granulares.

## Modelo de Esquema Galáxia/Constelação (Galaxy Schema)

![galaxia](https://github.com/CarlosJuncher03/ModelosDimensionais/assets/145303814/f923edca-7373-47c9-b0f7-e560c6e38a6b)

### Descrição
O esquema de galáxia, ou constelação, é uma estrutura mais complexa que permite múltiplas tabelas de fatos, cada uma com suas próprias tabelas de dimensão.

### Como Funciona
Em uma constelação de esquemas, diferentes tabelas de fatos compartilham tabelas de dimensão comuns, permitindo análises cruzadas entre diferentes áreas de negócios.

## Final

Este artigo forneceu uma visão geral dos principais modelos de modelagem dimensional, cada um adequado para diferentes necessidades de análise de dados e design de Data Warehouse.
