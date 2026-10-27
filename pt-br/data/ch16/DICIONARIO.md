## Dicionário de dados

O Grupo Comercial Arandu é um varejista e distribuidor multirregional fictício, com filiais nas cinco regiões brasileiras e diferentes linhas de produtos. As bases autorais são sintéticas e educacionais. O período é janeiro de 2024 a dezembro de 2025; algumas filiais podem ter iniciado sua operação durante a janela. Valores monetários estão em reais, sem escala de milhares implícita.

### vendas.csv

Uma linha representa um pedido/transação registrado por uma filial.

| Campo | Significado |
|---|---|
| `pedido_id` | Identificador do pedido |
| `data` | Data da transação, YYYY-MM-DD |
| `filial_id` | Código da filial |
| `produto_id` | Código do produto |
| `segmento_cliente` | Segmento comercial informado na venda |
| `quantidade` | Unidades vendidas |
| `preco_unitario` | Preço bruto por unidade, em reais |
| `desconto_pct` | Desconto como proporção entre 0 e 1 |

Descontos válidos: 0% a 40%, inclusive. Não há devoluções nem quantidades negativas. Segmentos de referência: Varejo, Pequena Empresa e Corporativo.

### cadastro_operacional.xlsx — aba filiais

Uma linha representa uma filial. Antes da abertura não deve haver atividade.

| Campo | Significado |
|---|---|
| `filial_id` | Código da filial |
| `filial` | Nome da filial |
| `regiao` | Região da filial |
| `cidade` | Cidade da filial |
| `data_abertura` | Data de início da operação, YYYY-MM-DD |

### cadastro_operacional.xlsx — aba produtos

Uma linha representa um produto. O preço cadastral não é necessariamente o preço observado em cada venda.

| Campo | Significado |
|---|---|
| `produto_id` | Código do produto |
| `produto` | Nome do produto |
| `categoria` | Categoria comercial |
| `preco_referencia` | Preço cadastral de referência, em reais |

### custos.csv

Uma linha representa produto × mês. UTF-8, separador `;`, decimal `,`; o custo pode variar no tempo.

| Campo | Significado |
|---|---|
| `produto_id` | Código do produto |
| `mes` | Mês de referência, YYYY-MM-01 |
| `custo_unitario` | Custo por unidade no mês, em reais |

### metas.csv

Uma linha representa filial × mês. Ausências antes da abertura representam ausência legítima de operação e não devem ser imputadas automaticamente.

| Campo | Significado |
|---|---|
| `filial_id` | Código da filial |
| `mes` | Mês de referência, YYYY-MM-01 |
| `meta_receita` | Meta de receita mensal, em reais |
| `meta_margem_pct` | Meta de margem como proporção entre 0 e 1 |

### Relações e indicadores possíveis

- Vendas e filiais: `filial_id`.
- Vendas e produtos: `produto_id`.
- Vendas e custos: `produto_id` e mês da venda.
- Realizado mensal e metas: `filial_id` e mês.

Antes de combinar, confirme unidade de observação e unicidade da chave cadastral. Não é necessária inferência, previsão ou informação externa. As bases permitem construir receita bruta, receita líquida, custo total, margem, ticket médio, quantidade e realizado versus meta. Essas métricas não são entregues prontas. A proporção de desconto e a meta de margem são frações: 0,10 representa 10%, não 0,10%.
