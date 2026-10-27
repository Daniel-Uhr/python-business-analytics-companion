## Roteiro do projeto

### Propósito

Este roteiro organiza a investigação sem determinar as ferramentas. Registre suas decisões e preserve uma sequência que outra pessoa consiga reproduzir.

### Entrega

- arquivo: `projeto_final_nome_sobrenome.ipynb`;
- em uma turma, o professor define o prazo; no estudo autônomo, tente resolver antes de consultar a resolução;
- preferencialmente um único notebook, usando caminhos relativos para `data/ch16`;
- executar **Restart Kernel and Run All** antes da entrega.

### 1. Compreensão dos dados

**Orientação.**

Compreenda cada base antes de analisar resultados.

**Dica.**

O que representa uma linha? Qual período está coberto? Quais variáveis identificam registros? Quais tabelas são complementares? Quais unidades de observação são diferentes?

**Alerta.**

**Duas tabelas possuírem uma coluna com o mesmo nome não significa automaticamente que podem ser combinadas daquela maneira.**

### 2. Qualidade

**Orientação.**

Investigue problemas capazes de alterar os resultados.

**Dica.**

Há registros repetidos, valores ausentes, categorias semanticamente iguais com grafias diferentes, violações das regras documentadas ou observações incomuns?

**Alerta.**

**Não modifique a base antes de compreender o problema. Uma observação extrema não é necessariamente um erro.**

### 3. Limpeza

**Orientação.**

Documente cada decisão importante: problema, decisão, justificativa e possível perda ou alteração de informação.

**Dica.**

Sua decisão é necessária para todas as métricas ou apenas para uma parte da análise? Existe uma alternativa defensável?

**Alerta.**

**Não existe uma regra universal para tratamento de missing.**

### 4. Integração

**Orientação.**

Construa uma base analítica coerente e valide o resultado de cada combinação.

**Dica.**

Qual é a chave correta? Qual é a cardinalidade? O número de linhas deveria mudar? Custos variam apenas por produto ou também no tempo? Metas pertencem à transação ou a filial × mês?

**Alerta.**

**Um merge pode executar sem erro e ainda produzir uma base substantivamente incorreta.**

### 5. Indicadores

**Orientação.**

Construa indicadores capazes de responder às perguntas empresariais.

**Dica.**

Considere atividade, receita, custos, margem, volume, ticket, metas e desempenho temporal. Em toda razão, identifique numerador, denominador e unidade.

**Alerta.**

**Maior valor absoluto não significa necessariamente melhor performance.**

### 6. Filiais e regiões

**Orientação.**

Compare o desempenho entre unidades e explicite a pergunta respondida por cada medida.

**Dica.**

Regiões possuem o mesmo número de filiais? Todas estiveram ativas durante o mesmo período? Total acumulado e performance média respondem à mesma pergunta?

**Alerta.**

**Comparações de totais podem refletir escala e exposição temporal.**

### 7. Produtos e categorias

**Orientação.**

Investigue o desempenho do portfólio por mais de uma dimensão.

**Dica.**

Liderança em quantidade é igual à liderança em receita? Maior receita significa necessariamente maior margem? A composição das vendas importa?

**Alerta.**

**“Melhor produto” depende do indicador utilizado.**

### 8. Tempo

**Orientação.**

Analise a evolução da atividade no período observado.

**Dica.**

Existem meses de maior atividade? Há mudança entre 2024 e 2025? Algum padrão recorrente aparece visualmente?

**Alerta.**

**Descrever tendência não significa prever o futuro.**

### 9. Metas

**Orientação.**

Avalie o desempenho em relação às metas e declare o denominador utilizado.

**Dica.**

Atingir em um mês é diferente de atingir sistematicamente. Frequência de atingimento e razão realizado/meta respondem perguntas diferentes. Como tratar períodos anteriores à abertura?

**Alerta.**

**Missing estrutural não é necessariamente erro.**

### 10. Observações que merecem investigação

**Orientação.**

Identifique observações incomuns antes de decidir mantê-las ou removê-las.

**Dica.**

Elas violam regras? Possuem chaves válidas? Podem representar eventos empresariais legítimos? Qual é seu impacto?

**Alerta.**

**Extremo não é sinônimo de erro.**

### 11. Visualizações

**Orientação.**

Produza de três a cinco visualizações não redundantes.

**Dica.**

Para cada gráfico, registre pergunta, escolha visual, evidência, interpretação e limite. Escolha o gráfico a partir da pergunta.

**Alerta.**

**Um gráfico correto tecnicamente pode ser inadequado para a pergunta ou induzir uma leitura exagerada.**

### 12. Conclusões, recomendações e limites

**Orientação.**

Apresente cinco conclusões executivas e de duas a quatro recomendações. Cada conclusão deve seguir evidência → interpretação → implicação gerencial.

**Dica.**

Separe o que os dados mostram da ação recomendada. Inclua uma seção específica de limitações: dados sintéticos, caráter descritivo, decisões de limpeza, cobertura, ausência de causalidade e ausência de previsão.

**Alerta.**

**Associação descritiva não demonstra causalidade, e recomendação sem evidência não é conclusão analítica.**

### Checklist antes da entrega

- [ ] As unidades de observação foram identificadas.
- [ ] As decisões de limpeza foram justificadas.
- [ ] As cardinalidades foram verificadas.
- [ ] Numeradores, denominadores e unidades foram declarados.
- [ ] Diferenças de cobertura foram consideradas.
- [ ] Observações incomuns foram investigadas.
- [ ] Os gráficos respondem a perguntas explícitas.
- [ ] Há cinco conclusões e de duas a quatro recomendações.
- [ ] Limitações estão registradas.
- [ ] O notebook executa do início ao fim em kernel limpo.
