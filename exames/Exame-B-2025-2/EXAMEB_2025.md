# Exame B: Communities & Crime 2025.2

Este exame será conduzido no formato de uma **competição**, aplicando conceitos de probabilidade e estatística na prática. O objetivo principal é analisar um conjunto de dados real de características socioeconômicas e demográficas e prever a taxa de crimes violentos (`violentPerPop`) em comunidades dos EUA.
Alunos trabalham em **duplas** e seguem quatro etapas sequenciais; cada entrega tem prazo divulgado no SIGAA.

---

## Sumário

* [Conjunto de dados](#conjunto-de-dados)
    * [Submissão de resultados](#submissão-dos-resultados)

* [Requisitos Técnicos e Critérios de Formatação](#requisitos-técnicos-e-critérios-de-formatação)
    * [2.1 Estrutura do Notebook](#21-estrutura-do-notebook)
    * [2.2 Comentários e Funções](#22-comentários-e-funções)
    * [2.3 Relatórios de Saúde do Dataset](#23-relatórios-de-saúde-do-dataset)
    * [2.4 Justificativas Textuais](#24-justificativas-textuais)
    * [2.5 Reprodutibilidade](#25-reprodutibilidade)

* [Etapas da Avaliação](#etapas-da-avaliação)
* [Formato de Submissão](#formato-de-submissão)
* [Avaliação](#avaliação)

---

## Conjunto de dados

O exame utiliza uma base real chamada Communities & Crime, que reúne dados socioeconômicos, demográficos e de policiamento de comunidades dos Estados Unidos. O objetivo é prever a taxa de crimes violentos por 100 mil habitantes (violentPerPop) a partir de variáveis como composição racial, renda, estrutura familiar e efetivo policial.

As descrições detalhadas de cada atributo estão disponíveis no arquivo `data_description.md`, que acompanha a avaliação. Recomendamos fortemente a leitura para entender o contexto e as variáveis disponíveis.

A base completa foi dividida em três arquivos:

    - train.csv: 70% dos dados, contendo todas as colunas (inclusive a variável-alvo violentPerPop). Deve ser usado para todas as etapas da análise, inclusive para o treinamento dos modelos.

    - test_features.csv: 30% restantes, contendo apenas as variáveis de entrada (features), sem a coluna-alvo. Esse arquivo será fornecido aos alunos na etapa de modelagem preditiva, e deverá ser usado para gerar as predições.

    - test_labels.csv: valores reais de violentPerPop para os exemplos do conjunto de teste. Será usado apenas pela equipe docente para avaliação interna dos modelos.

### Submissão dos resultados

Na etapa de modelagem (Etapa 4), os alunos devem:

1. Utilizar train.csv para treinar e validar seus modelos.

2. Fazer previsões sobre test_features.csv e salvar o resultado em um arquivo chamado submission.csv, contendo uma única coluna com os valores previstos, com o mesmo número de linhas e na mesma ordem do arquivo de entrada.

3. Incluir esse arquivo .csv na submissão final junto ao notebook.

Essa organização permite que o desempenho dos modelos seja avaliado de forma justa e objetiva sobre um conjunto de dados oculto durante o desenvolvimento.

O conjunto de dados fornecido (arquivo **`train.csv`**) contém informações demográficas detalhadas sobre as comunidades entre outras características suficientes paras as etapas da avaliação.

## Requisitos Técnicos e Critérios de Formatação


## 2.1 Estrutura do Notebook

* **Títulos em Markdown**:

    Títulos em Markdown devem ser usados para estruturar o notebook de forma hierárquica e facilitar a leitura. Utilize níveis como ## para etapas principais e ### para subtópicos, garantindo organização visual e navegabilidade.

  * `## Etapa 1 – Estatísticas Univariadas`
  * `### 1.1 Análise de Distribuições`

* **Comentários de célula**: 

    Cada célula de código deve começar com um comentário breve indicando seu propósito. O código deve seguir o padrão PEP8, com nomes claros, indentação correta e linhas com no máximo 100 caracteres para garantir legibilidade e padronização.

  ```python
  # Objetivo: Descrição sucinta
  ```

### 2.2 Comentários e Funções

* **Modularização**: ao longo do notebook, funções devem ser criadas para representar as etapas do pipeline (ex.: carregamento, tratamento, visualização, modelagem). Não há um número mínimo fixo, mas espera-se que as funções tornem o código reutilizável e organizado, com justificativa clara do seu papel na análise. Um exemplo:

  ```python
  def load_data(path):
      """Carrega o CSV e retorna DataFrame."""
      # ...
      return df
  ```
* **Docstrings**: cada função deve incluir uma breve descrição, listando parâmetros e valores retornados. 

A construção de funções ao longo do notebook é fundamental para a clareza e reutilização do código. Em vez de repetir comandos, os alunos devem encapsular etapas em funções nomeadas e bem documentadas, explicando seu uso dentro do fluxo da análise.

### 2.3 Relatórios de Saúde do Dataset

Ao final de cada processamento signifativo, imprimir informações do dataset antes e depois. Um exemplo:

```python
print("Shape:", df.shape)
print("Missing por coluna:\n", df.isna().sum())
print("Estatísticas básicas:\n", df.describe().T)
```

### 2.3 Justificativas Textuais

* Para cada tratamento de dados (outliers, imputação, codificação), inserir uma célula Markdown intitulada **Justificativa** com fundamentação teórica ou empírica.

* Para testes estatísticos: 

    - Formular claramente as hipóteses nula (H₀) e alternativa (H₁).
    - Definir o **nível de significância** (por exemplo, α = 0,05).
    - Escolher e justificar o teste estatístico adequado (ex.: correlação de Pearson, Spearman, teste t, ANOVA).
    - Apresentar os **valores das estatísticas** calculadas e o **p-value**.
    - Concluir se rejeita ou não H₀, com base no p-valor.
    - Incluir uma **tabela resumida** com os principais resultados.
---

**Exemplo**: Hipótese 1 – Relação entre `racepctblack` e `violentPerPop`

**Hipóteses formuladas:**

- H₀: Não há correlação significativa entre `racepctblack` e `violentPerPop`.
- H₁: Existe correlação significativa entre `racepctblack` e `violentPerPop`.

**Teste aplicado:** Correlação de Pearson  
**Nível de significância:** α = 0,05

**Resultados:**

| Estatística | Valor |
|-------------|-------|
| Correlação (r) | _preencher_ |
| p-value        | _preencher_ |

**Conclusão:** _Escreva aqui se rejeita ou não H₀, e o que isso implica._

### 2.4 Reprodutibilidade

* **Random seed fixo** em todas operações aleatórias (`random_state=2025`).
* **Versões de pacotes**: no bloco inicial, exibir:

  ```python
  import pandas as pd, numpy as np, sklearn
  print(pd.__version__, np.__version__, sklearn.__version__)
  ```
---

* **README e comentários**: Um “executive summary” no início do notebook (Markdown) explicando objetivos, passos e métricas. Lembrando que cada seção do notebook inicia com um cabeçalho do tipo ## Etapa X – Nome da Etapa.

## Etapas da Avaliação

### Etapa 1: Análise Unidimensional

Na primeira etapa, os alunos terão a tarefa de explorar cada variável de forma isolada. O objetivo é compreender melhor o conjunto de dados e identificar possíveis problemas (como valores ausentes ou *outliers*).

- **Possíveis análises:**
  - Calcular estatísticas descritivas para variáveis numéricas, como média, mediana, desvio padrão e assimetria.
  - Criar tabelas de frequência para variáveis categóricas, identificando as categorias mais frequentes e aquelas menos representadas.
  - Gerar gráficos como histogramas e *boxplots* para investigar distribuições e possíveis outliers.
  - Relatar valores ausentes nas variáveis e sugerir estratégias para tratá-los.

- **Entrega:**
  - Um notebook contendo as análises, gráficos e explicações claras de cada etapa.

### Etapa 2: Análise em duas ou mais dimensões

Na segunda etapa, os alunos deverão explorar as relações entre variáveis, com especial atenção às correlações entre `SalePrice` e as outras variáveis do dataset. Essa etapa é crucial para identificar quais variáveis serão mais importantes nas etapas à frente.

- **Possíveis análises:**
  - Gerar gráficos de dispersão para explorar as relações entre `violentPerPop` e variáveis contínuas.
  - Criar boxplots ou violin plots para investigar como `violentPerPop` varia entre categorias.
  - Calcular e interpretar uma matriz de correlação para as variáveis numéricas.
  - Relatar os padrões encontrados, destacando variáveis potencialmente relevantes para a modelagem.

- **Entrega:**
  - Um notebook contendo os gráficos, análises e interpretações das relações observadas.

### Etapa 3: Testes de Hipótese

Na terceira etapa, os alunos elaborarão hipóteses (no mínimo três) e usarão a estatística inferencial para validar as hipóteses usando os dados disponíveis.

- **Possíveis análises:**
  - O preço das casas aumenta com o aumento do tamanho das casas?
  - O tipo do bairro onde a casa está localizada tem relação sobre os serviços públicos disponíveis?
  - O estado da casa tem relação com o ano em que foi construída?

- **Entrega:**
  - Um notebook explicando as hipóteses levantadas, os testes realizados (com a devida checagem das suposições) e a interpretação conclusiva sobre cada hipótese.

### Etapa 4: Modelagem Preditiva

Na última etapa, os alunos deverão construir um modelo de regressão linear múltipla para prever os preços de venda das casas, ou seja, a variável dependente é `violentPerPop` e as demais podem ser usadas (todas ou apenas parte delas) como variáveis independentes.

- **Tarefas:**
  - Ajustar um modelo de **regressão linear** utilizando o conjunto de dados. Convém realizar testes mudando as variáveis independentes usadas no modelo e realizar possíveis transformações.
  - Realizar a análise dos resíduos do modelo final.

- **Entrega:**
  - Um notebook contendo:
    - O modelo final com explicações sobre as decisões tomadas
    - Análise dos resíduos

---

## Avaliação

Cada entrega será avaliada com base nos seguintes critérios:

1. **Qualidade Técnica:** [4 pts] O código está correto e segue as técnicas aprendidas em aula?
2. **Clareza:** [4 pts] O notebook está organizado, com explicações claras e gráficos bem apresentados?
3. **Criatividade:** [2 pts] Há originalidade na abordagem, com insights ou soluções criativas?

Para as Etapas de 1 a 3 serão geradas notas de 0 a 10 e serão lançadas como as atividades ET01, ET02 e ET03 em nossa planilha. A etapa de modelagem será lançada como Exame B. Isto significa que esta atividade terá maior peso na nota.

**Pontuação Adicional**

Nas etapas 2, 3 e 4 um total de 5 duplas serão arbitrariamente convidadas para apresentar suas entregas em sala de aula. As duplas serão recompensadas com 1 ponto extra na respectiva etapa.

Na etapa 4, a organização irá testar os modelos submetidos em um conjunto de dados oculto. As equipes com os melhores desempenhos em termos de $R^2$ sobre os dados ocultos serão recompensadas:

- **1º lugar:** 2 pontos extras no Exame B.
- **2º e 3º lugares:** 1 ponto extra no Exame B.

---

## Formato de Submissão

* **Notebook**: `ExameB_<RA1>_<RA2>.ipynb` (Google Colab compartilhável e arquivo exportado).
* **Conteúdo do ZIP**:

  ```
  ExameB_<E1>_<E2>.zip
  ├── train.csv
  ├── test_features.csv
  ├── submission.csv
  └── ExameB_<RA1>_<RA2>.ipynb
  ```
---

*Boa sorte e mãos à obra!*
