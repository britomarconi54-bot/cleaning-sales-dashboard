# RELATORIO.md — Entrega do projeto

## Cleaning Sales Analytics

### 1. O que foi entregue

Foi desenvolvida uma dashboard interativa para análise de vendas de materiais de limpeza, higiene e saneantes.

A solução possui:

- 100 registros de vendas;
- 30 produtos;
- filtros por produto, categoria, cidade, ano e método de pagamento;
- indicadores de pedidos, faturamento, ticket médio e unidades vendidas;
- gráfico de evolução mensal do faturamento;
- ranking de produtos por faturamento;
- análise de faturamento por categoria;
- publicação no GitHub Pages.

## 2. Perguntas de negócio

### Pergunta 1 — Como o faturamento evolui ao longo do tempo?

Escolhida para acompanhar a receita mensal e observar mudanças no comportamento das vendas.

### Pergunta 2 — Quais produtos geram mais faturamento?

Escolhida para identificar os itens que mais contribuem para a receita e apoiar análises de mix e estoque.

### Pergunta 3 — Como as vendas se distribuem por categoria?

Escolhida para comparar os grupos de produtos e entender a concentração do faturamento.

## 3. Tratamento da base

A base foi preparada e organizada antes da construção da dashboard. Foi utilizada a estrutura da aba **Sanitized**, com padronização de campos, datas e valores numéricos.

Também foram organizados os produtos e categorias, separados os preços de referência dos preços de venda e estruturados os campos necessários para filtros, KPIs e gráficos.

A base final contém 100 vendas e 30 produtos. Não foram incluídos dados pessoais ou sensíveis na base publicada.

A planilha de trabalho possui ainda as abas **Price_Base** e **Fontes** para documentar preços de referência.

## 4. Prompt e evolução

### Prompt inicial

> Crie um dashboard de vendas em HTML, com indicadores de vendas e receita, gráficos para responder perguntas de negócio, filtros por produto, cidade, ano e método de pagamento, e uma interface profissional.

### Evolução

O projeto começou com uma estrutura de dashboard de vendas automotivas. Durante o desenvolvimento, a base e a finalidade foram alteradas para materiais de limpeza e saneantes.

Foram então incluídos:

- categorias de produtos;
- quantidade vendida;
- faturamento em BRL;
- ticket médio;
- ranking de produtos;
- análise por categoria;
- filtro de categoria;
- carregamento dos dados por CSV externo.

Na revisão final, também foi corrigido o carregamento dos dois arquivos CSV para que o segundo arquivo fosse interpretado corretamente como continuação da base.

## 5. Ferramentas

- ChatGPT: análise, estruturação, geração e revisão do código e documentação.
- GitHub: armazenamento do código e publicação.
- GitHub Pages: hospedagem da dashboard.
- Canvas: não utilizado.
- Agente com skill: não utilizado como ferramenta específica.

## 6. Endereços

**Repositório público:**

https://github.com/britomarconi54-bot/porsche-sales-dashboard

**Dashboard:**

https://britomarconi54-bot.github.io/porsche-sales-dashboard/

## 7. Estrutura

```
porsche-sales-dashboard/
├── index.html
├── data/
│   ├── vendas_limpeza_01.csv
│   └── vendas_limpeza_02.csv
├── README.md
└── RELATORIO.md
```

## 8. Evidências recomendadas

Para a submissão, devem ser anexados:

- print da dashboard funcionando;
- print dos KPIs preenchidos;
- print de um filtro aplicado, por exemplo Categoria = Limpeza;
- link do repositório público.

## 9. Checklist final

- [ ] Dashboard publicada no GitHub Pages.
- [ ] Filtros funcionando.
- [ ] KPIs preenchidos.
- [ ] Gráficos funcionando.
- [ ] README completo.
- [ ] Arquivos citados no README presentes no repositório.
- [ ] Repositório público.
- [ ] Sem dados sensíveis.
- [ ] Link de submissão aponta para o repositório.

