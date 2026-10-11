# Projeto 1 — Evolução do Ensino Superior Brasileiro (2009–2024)

## 1. Sobre o projeto

Este projeto tem como objetivo analisar a evolução do ensino superior brasileiro entre 2009 e 2024, utilizando dados do Censo da Educação Superior, disponibilizados pelo Instituto Nacional de Estudos e Pesquisas Educacionais Anísio Teixeira (INEP).

A análise busca compreender as transformações ocorridas na oferta e na demanda por ensino superior no Brasil, identificando tendências temporais e diferenças entre regiões, instituições públicas e privadas e modalidades de ensino.

A pergunta de negócio que orienta o projeto é:

> **Como a oferta e a demanda por ensino superior no Brasil evoluíram entre 2009 e 2024, e quais segmentos apresentaram as maiores mudanças?**

O projeto foi desenvolvido em Python, com ênfase em análise exploratória de dados (EDA), tratamento de dados, construção de indicadores, análise temporal e visualização de informações.

## 2. Objetivos

### Objetivo geral

Investigar a evolução do ensino superior brasileiro entre 2009 e 2024, identificando tendências, diferenças regionais e mudanças na composição da oferta e da demanda.

### Objetivos específicos

- Analisar a evolução do número de cursos de graduação e de vagas ofertadas.
- Investigar o comportamento do número de ingressantes, matrículas e concluintes.
- Examinar diferenças regionais e estaduais na oferta e na demanda por ensino superior.
- Comparar a evolução das matrículas nas instituições públicas e privadas.
- Investigar diferenças entre as modalidades presencial e educação a distância (EAD).
- Analisar a distribuição das matrículas segundo características dos estudantes, como sexo, faixa etária e turno.
- Investigar a evolução das matrículas associadas a programas de financiamento e bolsas.
- Construir indicadores de crescimento, participação relativa e relações entre variáveis.

## 3. Fonte dos dados

Os dados utilizados são provenientes do **Censo da Educação Superior**, produzido pelo INEP, com foco na base de Cadastro de Cursos.

A base contém informações sobre cursos de graduação e instituições de educação superior, incluindo variáveis relacionadas a:

- Ano de referência do censo;
- Localização geográfica;
- Características dos cursos e das instituições;
- Vagas ofertadas;
- Ingressantes;
- Matrículas;
- Concluintes;
- Modalidade de ensino;
- Distribuição das matrículas por sexo, faixa etária e turno;
- Programas de financiamento e bolsas estudantis.

**Período analisado:** 2009 a 2024.

**Fonte oficial:** [INEP — Censo da Educação Superior](https://www.gov.br/inep/pt-br/areas-de-atuacao/pesquisas-estatisticas-e-indicadores/censo-da-educacao-superior).

## 4. Metodologia

O desenvolvimento do projeto foi organizado em etapas, desde a preparação dos dados até a interpretação dos resultados.

### 4.1. Preparação e integração dos dados

Inicialmente, foram organizados os conjuntos de dados anuais referentes ao período de 2009 a 2024. Em seguida, os arquivos foram preparados e concatenados verticalmente, formando uma base consolidada para as análises.

### 4.2. Seleção e limpeza dos dados

Foram selecionadas as variáveis relevantes para responder à pergunta de negócio. O tratamento dos dados incluiu:

- Verificação dos tipos das variáveis;
- Identificação e tratamento de valores ausentes;
- Verificação de registros duplicados;
- Análise da consistência temporal;
- Investigação das categorias das variáveis qualitativas;
- Análise de valores extremos;
- Verificação da consistência de totais e indicadores.

As decisões de tratamento foram realizadas considerando as características das variáveis e as limitações das informações disponíveis.

### 4.3. Análise exploratória de dados

A análise exploratória foi conduzida por meio de operações de agrupamento e agregação, principalmente com a biblioteca Pandas.

Foram construídas séries temporais e comparações entre diferentes segmentos do ensino superior, permitindo investigar a evolução dos principais indicadores ao longo do período.

### 4.4. Construção de indicadores

Foram calculadas medidas para analisar a variação temporal e a participação relativa de diferentes segmentos.

A taxa de crescimento percentual entre dois anos consecutivos foi calculada por:

\[
g_t = \frac{X_t-X_{t-1}}{X_{t-1}}\times 100.
\]

A participação percentual de um segmento em relação ao total foi calculada por:

\[
P_t = \frac{X_t}{X_{\text{total},t}}\times 100.
\]

Também foi examinada a razão anual entre concluintes e ingressantes, considerando sua evolução nas instituições públicas e privadas. Essa razão é utilizada como indicador descritivo de dois fluxos anuais distintos, não como uma taxa de conclusão de uma mesma coorte de estudantes.

### 4.5. Visualização e interpretação

Foram utilizados gráficos de linhas, barras e outras visualizações para representar tendências temporais, diferenças entre grupos e mudanças na composição do ensino superior.

As visualizações foram acompanhadas de interpretações destinadas a responder às questões formuladas durante a análise.

## 5. Principais análises e resultados

### 5.1. Evolução dos ingressantes

O número de ingressantes apresentou tendência geral de crescimento, passando de aproximadamente **2,08 milhões em 2009 para 4,86 milhões em 2024**.

A análise também identificou diferenças entre as regiões brasileiras, com maior concentração de ingressantes no Sudeste e menor volume na região Norte.

### 5.2. Evolução do número de cursos

O número de cursos apresentou tendência geral de crescimento ao longo do período. A maior expansão anual ocorreu em 2018, quando o crescimento foi de aproximadamente 6,82%.

Nos anos finais, observou-se desaceleração, com variação praticamente nula em 2023 e redução aproximada de 1,01% em 2024.

### 5.3. Evolução das vagas ofertadas

A quantidade de vagas ofertadas aumentou de aproximadamente **4,75 milhões em 2009 para mais de 23,66 milhões em 2024**.

Entretanto, a expansão da oferta não foi acompanhada por crescimento proporcional da ocupação. A taxa de ocupação passou de aproximadamente 59% em 2012 para 17,4% em 2021, apresentando recuperação moderada e chegando a aproximadamente 21,2% em 2024.

Esse resultado evidencia a importância de analisar conjuntamente a quantidade de vagas disponibilizadas e sua efetiva ocupação.

### 5.4. Evolução das matrículas

O total de matrículas aumentou de aproximadamente **5,99 milhões em 2009 para 10,23 milhões em 2024**.

Na distribuição por faixa etária, os estudantes de 18 a 29 anos representaram aproximadamente 70% das matrículas consideradas, com predominância da faixa de 18 a 24 anos.

Também foi observada maior participação feminina no total de matrículas, além de uma quantidade de matrículas em cursos noturnos superior à observada em cursos diurnos.

### 5.5. Financiamento e bolsas estudantis

A análise das matrículas associadas ao FIES, FINANC e PROUNI identificou trajetórias distintas.

O FIES apresentou crescimento expressivo até 2015, seguido por redução. O FINANC apresentou tendência geral de crescimento, enquanto o PROUNI e o PROUNIP apresentaram oscilações ao longo do período.

### 5.6. Evolução dos concluintes

O número de concluintes apresentou tendência geral de crescimento. Entretanto, foram observadas diferenças entre as modalidades de ensino.

Enquanto o número de concluintes em cursos EAD apresentou tendência de expansão, os cursos presenciais registraram tendência de redução a partir de aproximadamente 2018. Consequentemente, a diferença entre os volumes de concluintes das duas modalidades diminuiu.

### 5.7. Instituições públicas e privadas

A análise das matrículas nas instituições públicas e privadas mostrou desaceleração das taxas de crescimento a partir de aproximadamente 2014, acompanhada por oscilações nos anos posteriores.

Também foi investigada a razão anual entre concluintes e ingressantes. A série apresentou maior estabilidade na rede pública, enquanto a rede privada mostrou redução mais pronunciada ao longo do período.

### 5.8. Ensino presencial e educação a distância

As instituições públicas mantiveram predominância das matrículas presenciais em relação às matrículas EAD.

Nas instituições privadas, observou-se redução das matrículas presenciais a partir de aproximadamente 2015, enquanto as matrículas EAD cresceram continuamente, com aceleração a partir de aproximadamente 2018.

A partir de 2021, o número de matrículas EAD nas instituições privadas superou o número de matrículas presenciais.

Também foi observada uma mudança na composição da oferta de cursos EAD: a participação das instituições privadas passou de aproximadamente 53% em 2009 para 94% em 2024, enquanto a participação das instituições públicas diminuiu de aproximadamente 47% para 6%.

### 5.9. Distribuição regional

A oferta e a demanda por ensino superior apresentaram forte concentração na região Sudeste.

Considerando o total de vagas ofertadas no período, aproximadamente 79,9% estavam concentradas nessa região, enquanto a região Norte representava aproximadamente 2,9%.

Entre os estados, São Paulo apresentou aproximadamente 27% do total de ingressantes no período analisado.

## 6. Visualizações

Os 13 gráficos produzidos durante o projeto estão organizados na pasta `images/` do repositório.

As visualizações complementam o notebook e permitem acompanhar a evolução dos principais indicadores, as diferenças regionais e institucionais e as transformações observadas nas modalidades de ensino.

## 7. Tecnologias e ferramentas

As principais ferramentas utilizadas foram:

- **Python:** linguagem de programação;
- **Pandas:** manipulação, integração, agrupamento e agregação dos dados;
- **NumPy:** operações numéricas;
- **Matplotlib:** construção e personalização de gráficos;
- **Jupyter Notebook:** desenvolvimento e documentação da análise;
- **Git e GitHub:** versionamento e disponibilização do projeto.

## 8. Estrutura do repositório

A organização dos arquivos está apresentada a seguir como uma estrutura de referência:

```text
Projeto_1/
├── README.md
├── Evolução do Ensino Superior Brasileiro (Projeto 1).ipynb
└── images/
    ├── grafico_01.png
    ├── grafico_02.png
    ├── ...
    └── grafico_13.png
```

Os nomes dos arquivos de imagem devem corresponder aos nomes efetivamente utilizados no repositório. Caso os dados preparados sejam incluídos, eles também deverão ser documentados na estrutura do projeto.

## 9. Considerações finais

A análise exploratória dos dados do Censo da Educação Superior entre 2009 e 2024 permitiu identificar mudanças importantes na estrutura do ensino superior brasileiro.

O período foi marcado pelo crescimento do número de ingressantes, matrículas, cursos e vagas, mas a evolução desses indicadores não ocorreu necessariamente na mesma proporção. Destaca-se a expansão da oferta de vagas acompanhada por uma redução da taxa de ocupação em parte do período analisado.

Também foram identificadas mudanças na composição das matrículas e da oferta de cursos, especialmente relacionadas ao crescimento da educação a distância e à maior participação das instituições privadas nessa modalidade.

As diferenças regionais evidenciaram uma forte concentração da oferta e da demanda no Sudeste, enquanto as análises por características dos estudantes mostraram predominância de faixas etárias mais jovens e maior participação feminina nas matrículas.

Além dos resultados sobre o ensino superior, o projeto permitiu aplicar etapas fundamentais de um processo de Ciência de Dados: preparação e limpeza de dados, análise exploratória, construção de indicadores, análise temporal e visualização.

Como continuidade, as análises podem servir de base para investigações mais avançadas, envolvendo modelagem preditiva, séries temporais, análise espacial e técnicas de Machine Learning aplicadas à educação superior.

---

**Autor:** Mauricio Vinhote

**Área:** Ciência de Dados e análise exploratória de dados educacionais

**Período de referência dos dados:** 2009–2024
