# Cleaning Sales Analytics

Dashboard interativo de vendas de materiais de limpeza, higiene e saneantes.

## Perguntas de negócio

1. **Como o faturamento evolui ao longo do tempo?**  
   Para acompanhar a evolução mensal da receita e identificar períodos de maior ou menor faturamento.

2. **Quais produtos geram mais faturamento?**  
   Para identificar os itens que mais contribuem para a receita e apoiar decisões de mix e estoque.

3. **Como as vendas se distribuem por categoria?**  
   Para entender quais grupos de produtos concentram maior participação no faturamento.

## Funcionalidades

- Filtros por **produto, categoria, cidade, ano e método de pagamento**.
- KPIs de pedidos, faturamento, ticket médio e unidades vendidas.
- Evolução mensal do faturamento.
- Ranking dos 10 produtos com maior faturamento.
- Faturamento por categoria.
- Botão para limpar todos os filtros.
- Valores apresentados em **reais (BRL)**.

## Base de dados

A base foi transformada para o segmento de **materiais de limpeza e saneantes**, com:

- 100 registros de vendas;
- 30 produtos distintos;
- categorias de saneantes, limpeza, lavanderia, higiene, acessórios, EPI e descartáveis;
- cidades de Pernambuco;
- diferentes métodos de pagamento;
- preços de venda em reais.

A planilha possui também uma aba **Price_Base**, com os 30 produtos e seus preços de referência, e uma aba **Fontes**, que documenta as referências utilizadas. A dashboard publicada não depende de dados embutidos no HTML: ela carrega a base operacional diretamente dos dois arquivos CSV publicados na pasta `data/`.

## Pesquisa de preços

Os preços de referência foram levantados em fontes públicas de compras e licitações, principalmente em registros de 2026. Eles servem como referência para a modelagem e podem variar conforme marca, embalagem, região, especificação e volume comprado.

Entre as referências consultadas estão registros do **Portal Nacional de Contratações Públicas (PNCP)** e documentos de processos licitatórios públicos. Por exemplo, registros do PNCP de 2026 apresentam preços unitários para água sanitária, álcool, desinfetantes, detergentes e outros materiais de limpeza.

## Prompt utilizado e evolução

### Prompt inicial

> Crie um dashboard de vendas em HTML, com indicadores de vendas e receita, gráficos para responder perguntas de negócio, filtros por produto, cidade, ano e método de pagamento, e uma interface profissional.

### Evolução

O projeto foi inicialmente desenvolvido para uma base automotiva. Depois, a base foi transformada integralmente para o segmento de materiais de limpeza e saneantes.

A dashboard foi então reconstruída para trabalhar com:

- produtos em vez de modelos de veículos;
- categorias de limpeza e higiene;
- quantidade de unidades vendidas;
- faturamento em BRL;
- ranking de produtos;
- análise por categoria;
- filtros comerciais adequados ao novo negócio.

## Ferramentas utilizadas

- **ChatGPT** para análise, transformação dos dados e construção/revisão da dashboard.
- **Ferramentas de arquivos/código** para trabalhar com a planilha.
- **Integração com GitHub** para publicação do projeto.
- **Canvas:** não foi utilizado.

## Publicação

Repositório:

https://github.com/britomarconi54-bot/porsche-sales-dashboard

Dashboard:

https://britomarconi54-bot.github.io/porsche-sales-dashboard/

## Estrutura

```
porsche-sales-dashboard/
├── index.html
├── data/
│   ├── vendas_limpeza_01.csv
│   └── vendas_limpeza_02.csv
└── README.md
```

> A planilha de trabalho com a nova base de materiais de limpeza contém as abas `Sanitized`, `Price_Base` e `Fontes`.
