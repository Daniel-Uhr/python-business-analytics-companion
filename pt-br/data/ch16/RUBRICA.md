## Rubrica de avaliação

A rubrica avalia decisões, coerência, reprodução e comunicação. Aparência visual isolada não substitui qualidade conceitual. Total: **100%**. Os pesos abaixo são preservados; os quatro níveis descrevem a qualidade, sem inventar uma escala numérica adicional por nível.

### 1. Compreensão e unidade de observação — 10%

**Excelente.** Identifica corretamente unidade, período, chaves, tipos e relações de todas as bases.

**Adequado.** Identifica os elementos centrais, com pequenas omissões sem impacto.

**Parcial.** Confunde ou omite parte das unidades, chaves ou cobertura.

**Insuficiente.** Analisa sem compreender a estrutura das bases.

### 2. Qualidade e limpeza — 15%

**Excelente.** Diagnostica problemas relevantes, documenta decisões, impactos e alternativas.

**Adequado.** Trata os principais problemas e justifica a maior parte das decisões.

**Parcial.** Diagnóstico incompleto ou decisões pouco justificadas.

**Insuficiente.** Ignora qualidade ou altera dados arbitrariamente.

### 3. Transformação — 10%

**Excelente.** Cria variáveis e níveis analíticos coerentes, preservando significado e unidades.

**Adequado.** Transformações adequadas com pequenas falhas de documentação.

**Parcial.** Transformações parcialmente corretas ou pouco rastreáveis.

**Insuficiente.** Variáveis incorretas, opacas ou incompatíveis com a pergunta.

### 4. Integração e cardinalidade — 15%

**Excelente.** Identifica unidades, seleciona chaves corretas, compreende cardinalidades, valida linhas e evita multiplicação indevida.

**Adequado.** Integra corretamente e realiza validações essenciais.

**Parcial.** Merge funciona, mas cardinalidade ou validação ficam frágeis.

**Insuficiente.** Chaves incorretas, many-to-many indevido ou base analítica inválida.

### 5. Indicadores — 10%

**Excelente.** Define medidas coerentes, explicita numerador, denominador, unidade e nível de análise.

**Adequado.** Indicadores corretos, com documentação suficiente.

**Parcial.** Alguns indicadores corretos, mas há ambiguidades ou denominadores frágeis.

**Insuficiente.** Indicadores incorretos ou usados sem compreensão.

### 6. Análise exploratória — 10%

**Excelente.** Investiga distribuições, grupos, tempo e observações incomuns com perguntas claras.

**Adequado.** Cobre os principais padrões e interpreta adequadamente.

**Parcial.** EDA limitada, mecânica ou pouco conectada às perguntas.

**Insuficiente.** Apenas exibe tabelas ou números sem investigação.

### 7. Visualização — 10%

**Excelente.** Produz 3–5 gráficos pertinentes, legíveis e interpretados, com pergunta, evidência e limite.

**Adequado.** Gráficos adequados e majoritariamente bem comunicados.

**Parcial.** Há redundância, problemas de escolha ou interpretação incompleta.

**Insuficiente.** Gráficos enganosos, sem unidade ou desconectados da análise.

### 8. Storytelling — 8%

**Excelente.** Cinco conclusões ligam evidência, interpretação e implicação sem causalidade indevida.

**Adequado.** Conclusões claras e sustentadas, com pequenas lacunas.

**Parcial.** Conclusões genéricas, repetitivas ou parcialmente sustentadas.

**Insuficiente.** Afirmações sem evidência ou causalidade indevida.

### 9. Recomendação — 7%

**Excelente.** Apresenta 2–4 ações plausíveis, separadas das evidências e compatíveis com os limites.

**Adequado.** Recomendações coerentes e relacionadas à análise.

**Parcial.** Recomendações vagas ou pouco conectadas às evidências.

**Insuficiente.** Recomendações sem base analítica ou apresentadas como causalidade.

### 10. Limites e reprodutibilidade — 5%

**Excelente.** Registra limites, decisões e caminhos relativos; Restart + Run All funciona sem erros.

**Adequado.** Notebook reproduzível e limitações principais registradas.

**Parcial.** Reprodução exige pequenos ajustes ou limitações são incompletas.

**Insuficiente.** Notebook não reproduzível ou ausência de limites.

### Erros conceituais graves

Podem reduzir substancialmente a avaliação da dimensão correspondente:

- merge many-to-many indevido;
- eliminar uma observação apenas por ser extrema, sem investigação e justificativa substantiva;
- tratar missing estrutural como erro;
- imputar desconto sem justificativa;
- ignorar duplicações;
- usar indicador sem compreender seu denominador;
- confundir receita total com performance média;
- ignorar diferenças de meses ativos;
- fazer afirmação causal;
- apresentar recomendação sem evidência;
- entregar notebook que não executa integralmente.

### Soluções alternativas

Uma decisão diferente do pipeline de referência pode receber pontuação integral quando for substantivamente justificável, documentada, aplicada de forma consistente e acompanhada de seus efeitos sobre os resultados.
