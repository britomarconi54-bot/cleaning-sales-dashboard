# Cleaning Sales Analytics

Dashboard interativo de vendas de materiais de limpeza, higiene e saneantes.

## 1. Objetivo do projeto

O projeto transforma uma base de vendas em uma dashboard interativa publicada no GitHub Pages. A proposta é mostrar o caminho completo do trabalho: tratamento da base, definição das perguntas de negócio, uso da IA para construir a solução, revisão da dashboard e publicação.

## 2. Perguntas de negócio escolhidas

### 1. Como o faturamento evolui ao longo do tempo?

**Por quê:** permite acompanhar a evolução mensal da receita e identificar períodos de maior ou menor faturamento.

### 2. Quais produtos geram mais faturamento?

**Por quê:** ajuda a identificar os produtos que mais contribuem para a receita e fornece uma visão útil para decisões de mix, estoque e vendas.

### 3. Como as vendas se distribuem por categoria?

**Por quê:** permite entender quais grupos de produtos concentram maior faturamento e comparar o desempenho entre categorias.

Essas perguntas foram escolhidas porque cobrem três dimensões complementares: **tempo, produto e categoria**.

## 3. Tratamento da base antes da IA

A base original foi preparada antes de ser utilizada na construção da dashboard. O trabalho de preparação incluiu:

- utilização da aba **Sanitized** como base operacional;
- organização dos campos de venda em colunas estruturadas;
- padronização das datas para permitir análise temporal;
- transformação dos campos numéricos de quantidade e valores para cálculos;
- organização dos nomes de produtos e categorias;
- separação de preços de referência e preços efetivamente vendidos;
- identificação de 30 produtos distintos;
- consolidação de 100 registros de vendas;
- verificação dos campos utilizados nos filtros, indicadores e gráficos;
- retirada de informações pessoais ou sensíveis da base utilizada no projeto.

A planilha de trabalho também possui as abas **Price_Base** e **Fontes**, usadas para documentar preços de referência e suas fontes.

### Estrutura dos dados usados na dashboard

A dashboard trabalha com:

- 100 vendas;
- 30 produtos;
- categorias de limpeza, saneantes, higiene, lavanderia, acessórios, EPI e descartáveis;
- cidades de Pernambuco;
- métodos de pagamento;
- quantidade vendida;
- preço unitário;
- faturamento total;
- vendedor e status de entrega;
- valores em reais (BRL).

Os dados operacionais publicados no site estão em dois arquivos CSV na pasta `data/`. O HTML não contém os registros de vendas diretamente: ele carrega os CSVs publicados no repositório.

## 4. Prompt utilizado para gerar a dashboard

### Prompt inicial

> Crie um dashboard de vendas em HTML, com indicadores de vendas e receita, gráficos para responder perguntas de negócio, filtros por produto, cidade, ano e método de pagamento, e uma interface profissional.

### Prompt/evolução para a versão final

Durante o desenvolvimento, o pedido foi refinado para adaptar o projeto ao novo segmento de materiais de limpeza:

> Transforme a dashboard para uma operação de vendas de materiais de limpeza, higiene e saneantes. Use a base tratada com 100 vendas e 30 produtos. Crie uma interface profissional em HTML com filtros por produto, categoria, cidade, ano e método de pagamento. Mostre KPIs de pedidos, faturamento, ticket médio e unidades vendidas. Inclua três análises: evolução mensal do faturamento, produtos com maior faturamento e faturamento por categoria. A dashboard deve funcionar com dados externos publicados no GitHub e estar preparada para GitHub Pages.

### O que mudou até a versão final

1. O projeto deixou de representar vendas de veículos e passou para **materiais de limpeza e saneantes**.
2. Os indicadores foram adaptados para quantidade de pedidos, faturamento, ticket médio e unidades.
3. Foram adicionados filtros de **produto, categoria, cidade, ano e pagamento**.
4. Os gráficos foram direcionados para as três perguntas de negócio.
5. A base passou a ser carregada por arquivos CSV externos publicados no repositório.
6. O código foi revisado para corrigir o carregamento do segundo arquivo CSV.
7. A interface foi ajustada para apresentação de portfólio e leitura executiva.

## 5. Ferramentas utilizadas

Foi utilizado o **ChatGPT** como apoio para análise da base, definição da estrutura, geração e revisão do código e preparação da documentação.

**Canvas:** não foi utilizado.

**Agente com skill:** não foi utilizado como ferramenta específica do projeto.

Também foi utilizada a integração com **GitHub** para colocar os arquivos no repositório e publicar a solução.

## 6. Funcionalidades da dashboard

- Filtro por produto;
- Filtro por categoria;
- Filtro por cidade;
- Filtro por ano;
- Filtro por método de pagamento;
- botão para limpar filtros;
- KPI de pedidos;
- KPI de faturamento;
- KPI de ticket médio;
- KPI de unidades vendidas;
- evolução mensal do faturamento;
- ranking dos 10 produtos por faturamento;
- faturamento por categoria;
- valores em BRL.

## 7. Pesquisa de preços

Os preços de referência foram utilizados para apoiar a modelagem da base. As referências foram documentadas na aba `Fontes` da planilha e incluem registros públicos de compras e licitações.

Os valores são referências de modelagem e podem variar conforme marca, embalagem, região, especificação e quantidade adquirida.

## 8. Publicação

### Repositório — link que deve ser entregue

**https://github.com/britomarconi54-bot/cleaning-sales-dashboard**

### Dashboard publicada

**https://britomarconi54-bot.github.io/cleaning-sales-dashboard/**

> Na entrega acadêmica/portfólio, o link principal a ser enviado é o **repositório**, e não somente o endereço da dashboard.

## 9. Estrutura do repositório

```
cleaning-sales-dashboard/
├── index.html
├── data/
│   ├── vendas_limpeza_01.csv
│   └── vendas_limpeza_02.csv
├── README.md
└── RELATORIO.md
```

## 10. Evidência de funcionamento

Para a apresentação do projeto, recomenda-se incluir:

1. um print da dashboard aberta pelo GitHub Pages;
2. um print mostrando os KPIs preenchidos;
3. um print com um filtro aplicado, por exemplo **Categoria = Limpeza**;
4. o link do repositório público.

Essas evidências mostram não apenas o código, mas também que a solução está publicada e utilizável.

## 11. Checklist antes da entrega

- [ ] Dashboard abre pelo GitHub Pages.
- [ ] Filtros funcionam.
- [ ] KPIs são preenchidos.
- [ ] Gráficos são exibidos.
- [ ] Arquivos citados no README existem no repositório.
- [ ] Repositório está público.
- [ ] Repositório pertence à conta do aluno.
- [ ] Não há dados sensíveis na base publicada.
- [ ] O link enviado na atividade é o do repositório.
- [ ] Print da dashboard foi separado como evidência.
- [ ] Print com filtro aplicado foi separado como evidência.

## 12. Nome do repositório

O repositório foi renomeado para `cleaning-sales-dashboard`, deixando o nome coerente com o tema final do projeto e em formato legível, em minúsculas e sem acentos.
