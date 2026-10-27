# Dicionário de dados — Grupo Comercial Arandu

## Contexto

O Grupo Comercial Arandu é um grupo varejista e distribuidor multirregional, com filiais em cinco regiões brasileiras e portfólio composto por diferentes linhas de produtos. As bases são sintéticas e foram preparadas para fins educacionais.

## Período

Janeiro de 2024 a dezembro de 2025. Algumas filiais podem ter iniciado suas operações durante a janela observada.

## `vendas.csv`

Uma linha representa um pedido/transação registrado por uma filial.

| Coluna | Significado |
|---|---|
| `pedido_id` | identificador do pedido |
| `data` | data da transação, formato `YYYY-MM-DD` |
| `filial_id` | código da filial |
| `produto_id` | código do produto |
| `segmento_cliente` | segmento comercial informado no cadastro da venda |
| `quantidade` | unidades vendidas |
| `preco_unitario` | preço bruto por unidade, em reais |
| `desconto_pct` | desconto como proporção entre 0 e 1 |

Regra de negócio: descontos válidos estão entre 0% e 40%, inclusive. Não há devoluções ou quantidades negativas nesta base. Segmentos empresariais de referência: Varejo, Pequena Empresa e Corporativo.

## `cadastro_operacional.xlsx`

### Aba `filiais`

Uma linha representa uma filial. `data_abertura` registra o início da operação. Antes dessa data, a filial não deve possuir atividade.

### Aba `produtos`

Uma linha representa um produto. `preco_referencia` é um valor cadastral em reais, não necessariamente igual ao preço observado em cada venda.

## `custos.csv`

Arquivo UTF-8 com separador `;` e decimal `,`. Uma linha representa produto × mês. `custo_unitario` está em reais e pode variar ao longo do tempo.

## `metas.csv`

Uma linha representa filial × mês. `meta_receita` está em reais; `meta_margem_pct` é proporção entre 0 e 1. Valores ausentes antes da abertura da filial representam ausência legítima de operação e não devem ser imputados automaticamente.

## Relações entre as bases

- vendas e filiais: `filial_id`;
- vendas e produtos: `produto_id`;
- vendas e custos: `produto_id` e mês da venda;
- realizado mensal e metas: `filial_id` e mês.

Antes de combinar tabelas, confirme a unidade de observação e a unicidade da chave no lado cadastral. Não há necessidade de inferência, previsão ou informação externa.

## Indicadores possíveis

As bases fornecem componentes para construir receita bruta, receita líquida, custo total, margem, ticket médio, quantidade e realizado versus meta. As métricas derivadas não estão entregues prontas.
