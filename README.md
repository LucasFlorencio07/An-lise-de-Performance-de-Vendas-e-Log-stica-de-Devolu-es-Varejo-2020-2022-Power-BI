# Analise-de-Performance-de-Vendas-e-Logistica-de-Devolucoes-Varejo-2020-2022-Power-BI

**Descrição do Projeto:** 
Análise consolidada de vendas e devoluções para uma rede global de varejo. O objetivo principal é avaliar a trajetória do negócio (crescimento ou retração), apoiando a tomada de decisão executiva por meio de KPIs de performance comercial, distribuição geográfica e impacto financeiro de trocas/devoluções.

**KPIs e Métricas Analisadas:**  
- Performance Financeira & Tempo (DoD, MoM, QoQ, YoY): Faturamento Total, Lucro Total, Quantidade de Vendas, Margem de Lucro Anual e variação Mês Atual vs. Mês Anterior (LM-MA).   

- Visão Geográfica e Produto: Faturamento, Lucro e Volume de Vendas por Continente, País, Lojas, Categoria, Tipo de Produto, Marca e Item.   

- Gestão de Devoluções: Faturamento Perdido, Quantidade Devolvida, Taxa de Devolução (%) e Ofensores por Categoria, Marca e Produto. 

**Linguagens e Ferramentas:** 
Power BI, DAX, Linguagem M, Power Query e Excel.

**Observação:** A base de dados é fictícia e foi criada por IA via prompt. O objetivo do projeto é demonstrar raciocínio lógico-analítico e domínio das ferramentas.

**Navegação e Estrutura do Dashboard:**
O dashboard começa em uma Capa e a navegação entre as telas é feita pelos ícones do menu lateral esquerdo. Ele é dividido em 3 abas principais:

- Visão Geral (Vendas): Exibe o faturamento, lucro e total de vendas do ano selecionado, comparando com o ano anterior (YoY), além do canal de vendas (física vs. online), resumo por continente, entre outras informações.

- Indicadores: Aba detalhada com um gráfico de árvore para analisar vendas/faturamento por categoria, marca e produto. Traz um scroller de notícias com a variação do último mês, filtros retráteis no canto superior direito e cartões dinâmicos que mostram o melhor produto e a melhor loja.

- Devoluções: Focada no prejuízo financeiro com trocas, quantidade de itens devolvidos, evolução mensal do problema e mapa de devoluções por região.

**Linha de Raciocínio e Construção do Projeto** 

1. Tratamento de Dados (Power Query)Importação e Parâmetro: 

    - Importação de 4 bases fatos (3 de vendas e 1 de devoluções) e 4 bases dimensionais (Clientes, Lojas, Produtos e Localidades). Foi criado um Parâmetro de Caminho para alterar o diretório dos arquivos de forma simples, sem quebrar o projeto.   

    - Limpeza: Remoção de colunas e linhas desnecessárias, verificação do tipo de dado de cada coluna (datas, números, textos) e auditoria de erros via Qualidade da Coluna.

2. Modelagem e Cálculos (Power BI & DAX)

    - Relacionamentos e dCalendario: Criação do modelo estrela (Star Schema) e de uma tabela de calendário em DAX para permitir inteligência de tempo.

    - Fórmulas DAX: Aplicação de funções matemáticas (SUM, DIVIDE, SUMX), condicionais (IF, SWITCH), filtros (CALCULATE, ALL, TOPN, HASONEVALUE) e inteligência temporal (DATEADD, TOTALYTD) para gerar todos os cartões e visuais dinâmicos do relatório.   

3. Design Visual e Escolha dos Gráficos

    - Adequação dos Visuais aos Dados: Seleção estratégica do tipo de gráfico para cada tipo de informação — visuais de barras/colunas para comparações categóricas e ranqueamento, gráficos de linha para evolução temporal, matrizes hierárquicas (Treemap) para detalhar categorias/marcas/produtos, e mapas para distribuição geográfica.

    - Layout e Telas de Fundo: Design das telas de fundo (backgrounds) criado utilizando Inteligência Artificial e PowerPoint, garantindo um visual limpo, moderno e com hierarquia visual organizada.

