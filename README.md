# Porsche Sales Dashboard

Dashboard interativo de vendas Porsche desenvolvido a partir da planilha fornecida para o projeto.

## Perguntas de negócio

1. **Como a receita evolui ao longo do tempo?**  
   Para identificar a variação mensal da receita e observar períodos de maior ou menor faturamento.

2. **Quais modelos geram mais receita?**  
   Para comparar a contribuição financeira dos diferentes modelos e apoiar a análise do mix de produtos.

3. **Como as vendas se distribuem por método de pagamento?**  
   Para entender a composição dos pagamentos e visualizar a frequência de cada modalidade.

## Funcionalidades

- Filtros por **modelo, cidade, ano da venda e método de pagamento**.
- Indicadores de total de vendas, receita total, ticket médio e quilometragem média.
- Gráfico de evolução da receita.
- Ranking de modelos por receita.
- Distribuição das vendas por método de pagamento.
- Botão para limpar os filtros.

## Tratamento dos dados antes da IA

Foi utilizada a aba **Sanitized** da planilha.

- Foram usados os campos sanitizados de data, modelo, ano, preço de venda, quilometragem, pagamento, cidade, estado e status.
- Registros com data **INVALID** foram preservados para os indicadores e análises agregadas.
- As 24 linhas com data INVALID foram excluídas somente do gráfico temporal, pois não seria correto inventar uma data para elas.
- Para a publicação pública, nomes de clientes e vendedores foram removidos do HTML, pois não são necessários para responder às perguntas de negócio.
- Os valores de venda foram tratados como valores monetários em USD, conforme os dados da planilha.

## Prompt utilizado e evolução

### Prompt inicial

> Crie um dashboard de vendas Porsche em HTML, com indicadores de vendas e receita, gráficos para responder perguntas de negócio, filtros por modelo, cidade, ano e método de pagamento, e uma interface profissional.

### Evolução do prompt

Depois da primeira versão, o dashboard foi ajustado para usar a planilha real enviada, responder explicitamente às três perguntas de negócio, tratar datas inválidas sem criar dados artificiais, melhorar a organização visual e preparar a página para publicação no GitHub Pages.

Também foi feita uma revisão dos dados incorporados ao HTML antes da publicação, removendo campos de identificação de clientes e vendedores.

## Ferramentas utilizadas

- **ChatGPT** para análise dos dados, tratamento, construção e revisão do dashboard.
- **Ferramentas de arquivos/código** para trabalhar com a planilha e gerar o HTML.
- **Integração com GitHub** para publicar o projeto no repositório.
- **Canvas:** não foi utilizado.

## Publicação

Repositório:

https://github.com/britomarconi54-bot/porsche-sales-dashboard

Dashboard:

https://britomarconi54-bot.github.io/porsche-sales-dashboard/

> Observação: o endereço do GitHub Pages passa a funcionar depois que o GitHub Pages estiver habilitado para a branch `main`.

## Estrutura

```
porsche-sales-dashboard/
├── index.html
└── README.md
```
