# Atlas SAP

Um livro visual e interativo do SAP S/4HANA, feito para estudo: **o que roda por trás de cada transação**. Cada transação tem um raio-X com as tabelas que ela grava e lê, o lançamento contábil que gera e as transações vizinhas.

## O que tem

- **Mapa do SAP em formato de metrô**: 7 processos (compra até pagamento, projeto, produção, qualidade, manutenção, fechamento do mês e venda até recebimento). Cada estação é uma transação, e as baldeações mostram a mesma transação servindo processos diferentes (a MIGO aparece em quatro linhas). Clique numa linha para isolá-la.
- **Todos os módulos** organizados em capítulos: MM, SD, PP, QM, PM, WM, PS, FI, AA, CO, HCM, Fiscal Brasil e Ferramentas. Cada módulo tem uma cor própria, que se repete no mapa, nas cartas e nas fichas.
- **Raio-X de cada transação**: o que faz, quando usar, tabelas que grava e lê, lançamento contábil, tipos de movimento, transações vizinhas, diferenças entre ECC e S/4HANA e em quais linhas do mapa ela aparece.
- **Ficha de cada tabela**: campos principais (com a chave marcada), ligações com outras tabelas, quais transações gravam e leem nela e como consultar na SE16N.
- **Busca rápida**: `Ctrl K` (ou `/`) acha transação, tabela, módulo ou processo.
- **Mapa das tabelas**: a tabela escolhida fica no centro, com todas as ligações em volta e o campo de cada uma. Clique numa vizinha para seguir o caminho. Tem quatro percursos animados: do pedido à contabilidade, da venda à nota fiscal, da ordem ao custo e do estoque à conta contábil.
- **Trilha de estudo**: 10 etapas na ordem certa, de Fundamentos a Pessoas e fiscal, com as transações e tabelas de cada uma e o progresso de cada etapa.
- **Quiz**: 10 perguntas geradas na hora a partir do conteúdo (qual transação faz isto, que tabela ela grava, qual é a chave, se lança na contabilidade, de que módulo é). Por módulo, por etapa da trilha ou o Atlas inteiro. Responde com as teclas 1 a 4, e o melhor resultado de cada assunto fica salvo.
- **Viagens animadas** em cada capítulo: o processo roda estação por estação, mostrando as tabelas que ganham registro e os razonetes.
- **Caderno de estudo**: o botão "Já entendi" marca a transação como estudada, e o progresso aparece no índice, na capa de cada capítulo e na trilha (fica salvo no navegador).
- Tema claro e escuro, e versão para celular.

## Capítulos

**Materiais e compras (MM)**
- A estrutura por trás: empresa, centro, depósito, organização de compras e grupo de compradores
- A viagem do pedido: animação de 10 pneus da requisição ao pagamento, mostrando as tabelas que ganham registro e os razonetes (Estoque, GR/IR, Impostos a recuperar, Fornecedor, Banco)
- Tipos de movimento (101, 102, 122, 201, 261, 311, 551, 561, 601, 701/702) com o lançamento de cada um
- 54 transações com raio-X: cadastro, compras, estoque, inventário e fatura
- Fichas das tabelas do MM (MARA, MARC, MARD, MBEW, EBAN, EKKO, EKPO, EKET, EKKN, EKBE, MATDOC, RBKP, RSEG e outras)

**Contabilidade financeira (FI)**
- A estrutura por trás: empresa, plano de contas, conta do razão, exercício e ledger
- Um mês na vida do razão: energia, venda de sucata, recebimento, pagamento e provisão, com tabelas e razonetes
- Como o MM acha a conta contábil: tipo de movimento → chave de transação (BSX, WRX, GBB, PRD) → classe de avaliação → T030
- 28 transações (razão, contas a pagar, contas a receber, banco e fechamento) e 22 tabelas

**Ativo imobilizado (AA)**
- A estrutura por trás: classe, imobilizado, área de depreciação, chave e vida útil
- A vida de um imobilizado: cadastro, compra, um ano de depreciação e baixa por sucateamento
- 15 transações e 7 tabelas

**Controladoria (CO)**
- A estrutura por trás: área de custos, centro de custo, centro de lucro, ordem e classe de custo
- Para onde vai o custo: folha, consumo para ordem, alocação de horas, rateio e liquidação, mostrando que o total não muda, só muda de lugar
- 21 transações (cadastro, planejamento, lançamentos, fechamento, custo do produto e relatórios) e 18 tabelas

**Vendas e distribuição (SD)**
- A estrutura por trás: organização de vendas, canal, setor, local de expedição e cliente por área de vendas
- Da cotação ao dinheiro no banco: 100 t de açúcar passando por cotação, ordem, remessa, saída (CPV), fatura com nota fiscal e recebimento
- O fluxo de documentos: como a VBFA liga cada documento ao seguinte, e as categorias VBTYP
- 19 transações (cadastro, vendas, expedição e faturamento) e 14 tabelas, mais as da nota fiscal

**Planejamento da produção (PP)**
- A estrutura por trás: centro, planejador MRP, versão de produção, recurso e tipo de ordem
- Uma ordem de açúcar: previsão de demanda, MRP Live, ordem de processo, consumo de cana (261), confirmação das fases, entrada do açúcar (101) e liquidação da diferença
- Os dados mestre da produção (material → versão → lista técnica → receita mestre → recurso) e os movimentos 261, 262, 101 e 531 (subproduto)
- 25 transações (indústria discreta e de processo) e 19 tabelas

**Gestão da qualidade (QM)**
- A estrutura por trás: tipo de inspeção, plano, característica, catálogo e lote de controle
- Um lote de açúcar no laboratório: entrada em controle de qualidade, resultados, nota de qualidade e decisão de utilização (321 e 350)
- Tipos de inspeção (01, 04, 08, 10, 89) e os movimentos entre tipos de estoque
- 12 transações e 12 tabelas

**Manutenção (PM)**
- A estrutura por trás: centro de planejamento, local de instalação, equipamento, centro de trabalho e grupo de planejamento
- Uma ordem na moenda: nota de avaria, ordem, liberação, peças (261), horas dos mecânicos e liquidação no centro de custo da moenda
- A estrutura técnica (local → equipamento → ponto de medição → lista de tarefas → plano) e os tipos de manutenção: corretiva, preventiva, preditiva e solicitação
- 20 transações e 15 tabelas

**Projetos (PS)**
- A estrutura por trás: definição do projeto, elemento PEP, diagrama de rede, atividade e perfil
- Uma reforma na entressafra: estrutura, plano, orçamento, pedido como compromisso, entrega, horas, liquidação para imobilizado em andamento e imobilizado definitivo
- Os cinco números do projeto (plano, orçamento, compromisso, real e disponível) e o caminho do investimento
- 14 transações e 7 tabelas

**Armazém e transporte (WM)**
- A estrutura por trás: número do depósito, tipo, área, posição e quant
- Do caminhão à prateleira e de volta: 40 sacos entrando, sendo guardados e 15 saindo para uma remessa
- 15 transações: WM clássico, EWM (com a observação de que no S/4 o caminho é o EWM) e transporte, e 14 tabelas

**Recursos humanos (HCM)**
- A estrutura por trás: empresa, área e subárea de RH, grupo de empregados e área de processamento da folha
- Um mês de folha: admissão, horas extras, avaliação de tempos, cálculo da folha, execução de lançamento na contabilidade e pagamento
- Os infotipos (0000, 0001, 0002, 0007, 0008, 0014, 0015, 2001, 2002, 2006) e o cluster PCL2
- 11 transações e 15 tabelas

**Fiscal Brasil**
- A estrutura por trás: local de negócios (CNPJ), categoria de nota, CFOP e código de imposto
- Uma nota fiscal de saída: faturamento, envio e autorização da NF-e, apuração e pagamento das guias
- Da transação à SEFAZ, e os impostos da nota (ICMS, IPI, PIS e COFINS, ICMS-ST, ISS)
- 5 transações e 8 tabelas (J_1BNFDOC, J_1BNFLIN, J_1BNFSTX, J_1BNFE_ACTIVE e outras)

**Ferramentas**
- SE16N, SE16H, SE11, SQVI e SU53, com o caminho para descobrir a tabela e o campo por trás de qualquer tela

## Em números

244 transações com raio-X, 190 tabelas com ficha, 13 capítulos, 7 linhas no mapa de metrô e 12 viagens animadas.

## Observação

O conteúdo cobre as transações e tabelas padrão do SAP S/4HANA. Transações Z, autorizações e configurações variam de empresa para empresa. Os valores das viagens são ilustrativos.

## Publicar no GitHub Pages

1. Crie um repositório (sugestão: `atlas-sap`) e envie o `index.html` e este `README.md`.
2. Em **Settings → Pages**, escolha a branch `main` e a pasta raiz.
3. O livro fica em `https://<seu-usuario>.github.io/atlas-sap/`.

Usa as fontes Fraunces, Inter e JetBrains Mono e os ícones Tabler via CDN. Não precisa instalar nada.
