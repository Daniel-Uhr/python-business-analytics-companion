# Dados do Capítulo 15

Material complementar do livro Python para Business Analytics, de Daniel de Abreu Pereira Uhr. Os arquivos empresariais são fictícios e autorais. Receita/meta de receita: reais em unidades monetárias, sem escala de milhares. Margem do CSV: porcentagem (28,4 significa 28,4%); meta_margem_pct do Excel: fração (0,29 significa 29%). CSV UTF-8, ponto e vírgula e vírgula decimal; Excel abas unidades/metas. Dez registros filial–mês; março de 2026 somente Norte/Sul. Nenhuma observação ausente foi inventada.

IBGE: API de Localidades, https://servicodados.ibge.gov.br/api/v1/localidades/estados ; JSON recebido pelo autor em 17/08/2026, 27 UFs incluindo DF. Documentação: https://servicodados.ibge.gov.br/api/docs/localidades .

Banco Central do Brasil: SGS 24363, IBC-Br, índice 2022=100, mensal, sem ajuste sazonal. Endpoint: https://api.bcb.gov.br/dados/serie/bcdata.sgs.24363/dados . Snapshot recebido pelo autor em 17/08/2026, janeiro de 2023–dezembro de 2024, já tabulado em CSV data/ibc_br. As datas ISO no dia 1 representam meses. A leitura deste arquivo não é nova aquisição do serviço.

Preserve estes arquivos. Consultas atuais podem divergir por revisão; uma nova aquisição deve ter data real, outro nome, fonte e transformações documentadas. O notebook padrão não faz solicitações de rede nem sobrescreve os snapshots. A opção online usa GET público, sem credenciais. Consulte ../../DATA-NOTICES.md para as condições dos dados oficiais e o escopo de licenças do repositório para os materiais autorais.
