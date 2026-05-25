# Exame B

Este exame foi planejado para ser conduzido no formato de uma **competição**, oferecendo a oportunidade de aplicar conceitos aprendidos em sala de aula de maneira prática. O objetivo principal é analisar um conjunto de dados real de preços de casas na cidade de Ames, Iowa, e projetar um modelo para prever preços nesta região.

Os alunos trabalharão em **duplas** e serão desafiados a explorar os dados, realizar testes de hipótese e construir um modelo preditivo.

---

## Conjunto de dados

O conjunto de dados fornecido (arquivo **`houses.csv`**) contém informações detalhadas sobre as casas, como o área do terreno, número de quartos, a idade da construção, entre outras características. Para detalhes acerca das váriaveis acesse o arquivo [**`data_description.md`**](data_description.md).

---

## Instruções do exame

O exame será dividido em **quatro etapas**, com **entregas sucessivas em datas disponibilizadas no SIGAA**. Cada etapa aborda um componente específico do processo de análise de dados e modelagem preditiva.

### Etapa 1: Análise Unidimensional e em Duas ou Mais Dimensões

Na primeira etapa, os alunos terão a tarefa de explorar cada variável de forma isolada, além de investigar as relações entre elas. O objetivo é compreender melhor o conjunto de dados, identificar possíveis problemas (como valores ausentes ou *outliers*) e, com especial atenção, analisar as correlações entre `SalePrice` e as outras variáveis do dataset. Essa etapa é crucial para identificar quais atributos serão mais importantes nas fases seguintes.

- **Possíveis análises:**
  - Calcular estatísticas descritivas para variáveis numéricas, como média, mediana, desvio padrão e assimetria.
  - Criar tabelas de frequência para variáveis categóricas, identificando as categorias mais frequentes e aquelas menos representadas.
  - Gerar gráficos como histogramas e *boxplots* para investigar distribuições e possíveis outliers.
  - Relatar valores ausentes nas variáveis e sugerir estratégias para tratá-los.
  - Gerar gráficos de dispersão para explorar as relações entre `SalePrice` e variáveis contínuas.
  - Criar boxplots ou violin plots para investigar como `SalePrice` varia entre categorias (ex.: `Neighborhood` ou `MSZoning`).
  - Calcular e interpretar uma matriz de correlação para as variáveis numéricas.
  - Relatar os padrões encontrados, destacando variáveis potencialmente relevantes para a modelagem.

- **Entrega:**
  - Um notebook contendo as análises isoladas e as relações observadas, com gráficos e explicações claras de cada passo.
  

### Etapa 2: Testes de Hipótese

Na terceira etapa, os alunos elaborarão hipóteses (no mínimo três) e usarão a estatística inferencial para validar as hipóteses usando os dados disponíveis.

- **Possíveis análises:**
  - O preço das casas aumenta com o aumento do tamanho das casas?
  - O tipo do bairro onde a casa está localizada tem relação sobre os serviços públicos disponíveis?
  - O estado da casa tem relação com o ano em que foi construída?

- **Entrega:**
  - Um notebook explicando as hipóteses levantadas, os testes realizados (com a devida checagem das suposições) e a interpretação conclusiva sobre cada hipótese.

### Etapa 3: Modelagem Preditiva

Na última etapa, os alunos deverão construir um modelo de regressão linear múltipla para prever os preços de venda das casas, ou seja, a variável dependente é `SalePrice` e as demais podem ser usadas (todas ou apenas parte delas) como variáveis independentes.

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

Além das entregas acima, serão realizadas apresentações da seguinte forma. Ao final da etapa 1, metade das duplas será sorteadas aleatoriamente para apresentar os resultados da Etapa 1 (ET01), em sala de aula, e após a entrega da Etapa 2 (ET02), o restante das duplas deverá apresentar os resultados desta etapa. A nota dessa apresentação será contabilizada como uma das atividades (APR). Após a entrega da Etapa 3 (ET03), **todas** as duplas deverão apresentar seu trabalho final para o professor. A nota desta apresentação será a nota do Exame B.

> As apresentações deverão ser feitas em 10 minutos (7 para apresentação e 3 para perguntas). Um estudante da dupla será sorteado para apresentar e o outro deverá responder às perguntas feitas pelo professor e pela turma.


**Pontuação Adicional**

Na etapa 3, a organização irá testar os modelos submetidos em um conjunto de dados oculto. As equipes com os melhores desempenhos em termos de $R^2$ sobre os dados ocultos serão recompensadas:

- **1º lugar:** 2 pontos extras no Exame B.
- **2º e 3º lugares:** 1 ponto extra no Exame B.

---

## Entrega e Submissão

- Os notebooks devem ser criados no Google Colab em Python e o arquivo deve ser enviado via SIGAA.
- Entregas atrasadas não serão consideradas.

---

## Conclusão

Este exame/competição foi estruturado para transformar a avaliação em uma experiência prática, que simula situações reais enfrentadas por cientistas de dados. Mantenha o espírito de colaboração e criatividade, e aproveite esta oportunidade para aprender e crescer!

---

## Sugestões de Formatação e Organização

### Estrutura do Notebook

* **Resumo e seções**: Adicione um breve resumo no início do seu notebook explicando objetivos e passos realizados. Além disso, cada seção do notebook inicia com um cabeçalho do tipo ## Seção X – Nome da Seção.

* **Títulos em Markdown**:

    Títulos em Markdown devem ser usados para estruturar o notebook de forma hierárquica e facilitar a leitura. Utilize níveis como ## para etapas principais e ### para subtópicos, garantindo organização visual e navegabilidade.

  * `## Etapa 1 – Estatísticas Univariadas`
  * `### 1.1 Análise de Distribuições`

* **Comentários de célula**:

    Cada célula de código deve começar com um comentário breve indicando seu propósito. O código deve seguir o padrão PEP8, com nomes claros, indentação correta e linhas com no máximo 100 caracteres para garantir legibilidade e padronização.

```python
  # Objetivo: Descrição sucinta
```

### Comentários e Funções

* **Modularização**: ao longo do notebook, funções devem ser criadas para representar as etapas do pipeline (ex.: carregamento, tratamento, visualização, modelagem). Não há um número mínimo fixo, mas espera-se que as funções tornem o código reutilizável e organizado, com justificativa clara do seu papel na análise. Um exemplo:

```python
def load_data(path):
    """Carrega o CSV e retorna DataFrame."""
    # ...
    return df
```

* **Docstrings**: cada função deve incluir uma breve descrição, listando parâmetros e valores retornados.

A construção de funções ao longo do notebook é fundamental para a clareza e reutilização do código. Em vez de repetir comandos, os alunos devem encapsular etapas em funções nomeadas e bem documentadas, explicando seu uso dentro do fluxo da análise.

### Relatórios de Saúde do Dataset

Ao final de cada processamento signifativo, imprimir informações do dataset antes e depois. Um exemplo:

```python
  print("Shape:", df.shape)
  print("Missing por coluna:\n", df.isna().sum())
  print("Estatísticas básicas:\n", df.describe().T)
```

### Justificativas Textuais

* Para cada tratamento de dados (outliers, imputação, codificação), inserir uma célula Markdown intitulada **Justificativa** com fundamentação teórica ou empírica.

* Para testes estatísticos:

  * Formular claramente as hipóteses nula (H₀) e alternativa (H₁).
  * Definir o **nível de significância** (por exemplo, α = 0,05).
  * Escolher e justificar o teste estatístico adequado (ex.: correlação de Pearson, Spearman, teste t, ANOVA).
  * Apresentar os **valores das estatísticas** calculadas e o **p-value**.
  * Concluir se rejeita ou não H₀, com base no p-valor.
  * Incluir uma **tabela resumida** com os principais resultados.

---

**Exemplo**: Hipótese 1 – Relação entre `racepctblack` e `violentPerPop`

**Hipóteses formuladas:**

* H₀: Não há correlação significativa entre `racepctblack` e `violentPerPop`.
* H₁: Existe correlação significativa entre `racepctblack` e `violentPerPop`.

**Teste aplicado:** Correlação de Pearson  
**Nível de significância:** α = 0,05

**Resultados:**

| Estatística | Valor |
|-------------|-------|
| Correlação (r) | *preencher* |
| p-value        | *preencher* |

**Conclusão:** Escreva aqui se rejeita ou não H₀, e o que isso implica.

### Reprodutibilidade

* **Random seed fixo** em todas operações aleatórias (`random_state=2025`).
* **Versões de pacotes**: no bloco inicial, exibir:

```python
  import pandas as pd, numpy as np, sklearn
  print(pd.__version__, np.__version__, sklearn.__version__)
```

---

Boa sorte, e que vença a melhor análise!
