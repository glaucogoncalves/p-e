# Exame B: Insumos Agrícolas 2025.2

Este exame será conduzido no formato de uma análise de dados crítica, aplicando conceitos de probabilidade e estatística na prática. O objetivo principal é analisar um conjunto de dados real de insumos agrícolas na Amazônia, de modo que os alunos avaliem os impactos das mudanças climáticas na produção agrícola e reflitam criticamente sobre as relações entre clima, práticas produtivas e sustentabilidade na região. 

O exame deverá ser realizado **obrigatoriamente em duplas**. As equipes deverão explorar, analisar e modelar os dados com foco em respostas relevantes para cadeias produtivas amazônicas, considerando fatores ambientais, socioeconômicos e climáticos.

## Sumário

* [Conjunto de dados](#conjunto-de-dados)
* [Etapas da Avaliação](#etapas-da-avaliação)
* [Formato de Submissão](#formato-de-submissão)
* [Avaliação](#avaliação)
* [Sugestões de Formatação e Organização](#sugestões-de-formatação-e-organização)

## Conjunto de dados

O conjunto de dados é separado em arquivos .csv (Comma-Separated-Values), cada um sendo referente aos dados de um estado da região Amazônica brasileira: 

    - RR: Roraima

    - RO: Rondônia

    - PA: Pará

    - AP: Amapá

    - AM: Amazonas

    - AC: Acre

Os estudantes receberão esse conjunto de arquivos contendo variáveis relacionadas à produção, características ambientais e atributos físico-químicos associados a PFNM e outros insumos agrícolas amazônicos.

**Os alunos deverão obrigatoriamente escolher um único estado dentre os disponíveis e uma única cultura alimentícia específica para trabalhar durante todo o exame. Essa escolha deverá ser mantida ao longo de todas as etapas da avaliação, não sendo permitidas alterações.**

**Não será permitido que duas duplas escolham a mesma combinação de estado e cultura alimentícia. Cada dupla deverá trabalhar com uma combinação exclusiva.**


Exemplos de variáveis que o compõem:

- Volume anual de produção por estado

- Temperatura média mensal

- Déficit de pressão de vapor (VPD)

- Precipitação média mensal

- Ocorrência de queimadas


As descrições detalhadas de cada atributo estão disponíveis no arquivo `data_description.md`, que acompanha a avaliação. Recomendamos fortemente a leitura para entender o contexto e as variáveis disponíveis.

## Etapas da Avaliação

O exame será dividido em três etapas, com entregas sucessivas via SIGAA. Cada etapa aborda um componente específico do processo de análise de dados e modelagem preditiva.

### Etapa 1: Análise Unidimensional e Multidimensional

Na primeira etapa, os alunos terão a tarefa de explorar, no mínimo, um subconjunto de variáveis de modo a compreender melhor o conjunto de dados e identificar possíveis problemas (como valores ausentes ou *outliers*). 

Análise unidimensional: No primeiro momento, os alunos deverão tratar as variáveis de forma isolada, realizando análises exploratórias de modo a se familiarizarem com o conjunto de dados e extraírem informações iniciais.

* **Possíveis análises unidimensionais:**
  * Calcular estatísticas descritivas para variáveis numéricas.
  * Criar tabelas de frequência para variáveis categóricas, identificando as categorias mais frequentes e aquelas menos representadas.
  * Gerar gráficos como histogramas e *boxplots* para investigar distribuições e possíveis outliers.
  * Relatar valores ausentes nas variáveis e sugerir estratégias para tratá-los.

Análise multidimensional: No segundo momento, os alunos deverão explorar as relações entre variáveis, com especial atenção às relações entre a variável alvo "prod_ton" e as outras variáveis do conjunto de dados. Essa etapa é crucial para identificar quais variáveis serão mais importantes nas etapas à frente.

* **Possíveis análises multidimensionais:**
  * Gerar gráficos de dispersão para explorar as relações entre `prod_tun` e variáveis contínuas.
  * Criar boxplots ou violin plots para investigar como `prod_tun` varia entre categorias.
  * Calcular e interpretar uma matriz de correlação para as variáveis numéricas.
  * Relatar os padrões encontrados, destacando variáveis potencialmente relevantes para a modelagem.

* **Entrega:**
  * Um notebook contendo as análises, gráficos e explicações claras de cada etapa.
  * O notebook deve estar em um zip como explicado em [Formato de Submissão](#formato-de-submissão)

### Etapa 2: Testes de Hipótese

A dupla deverá propor no mínimo cinco hipóteses relacionadas a impactos ambientais, climáticos ou socioeconômicos sobre a produtividade dos insumos.

Possíveis análises podem incluir: verificar se a ocorrência de eventos climáticos extremos impacta a média de produção; avaliar a relação linear entre queimadas e produção; associar faixas de precipitação (chuva) com categorias de sucesso da safra (Baixa/Média/Alta); verificar a tendência temporal da produção ou a influência da temperatura.

Para a avaliação ser bem-sucedida, sugere-se que estruturem os testes seguindo este roteiro:

    1. Formulação: Definir H0​ e H1​ claramente, justificando a escolha do teste perante o contexto do conjunto de dados e do problema.

    2. Seleção do Teste: Justificar por que escolheram aquele teste (ex: "Usamos Spearman porque os dados não são normais").

    3. Execução: Rodar o teste no Python.

    4. Conclusão: Apresentar resultados numéricos, em saída de código e em texto quando citados. Além disso, a conclusão do teste deve ser redigida em texto de forma clara e discorrendo um significado para o resultado no contexto do problema. Por exemplo: Não dizer apenas "rejeito H0", mas sim "Com 95% de confiança, há evidências de que queimadas reduzem a produção de açaí, sugerindo que..."

* **Entrega:**
  * Um notebook explicando as hipóteses levantadas, os testes realizados (com a devida checagem das suposições) e a interpretação conclusiva sobre cada hipótese.
  * O notebook deve estar em um zip como explicado em [Formato de Submissão](#formato-de-submissão)


### Etapa 3: Modelagem Preditiva

Na última etapa, os alunos deverão construir um modelo de regressão linear múltipla para prever a produção, ou seja, a variável dependente é `prod_ton` e as demais podem ser usadas (todas ou apenas parte delas) como variáveis independentes.

Os alunos devem:

1. Utilizar o conjunto do respectivo estado (como ```PA.csv```) para treinar e validar seus modelos. Deve-se separar um subconjunto dos dados para validação, sem que esse subconjunto seja observado pelo modelo durante o treinamento.

2. Fazer previsões sobre o conjunto de validação e salvar o resultado em um arquivo. Deve-se incluir esse arquivo .csv na submissão final junto ao notebook. 

Essa organização permite que o desempenho dos modelos seja avaliado de forma justa e objetiva sobre um conjunto de dados durante o desenvolvimento.

Salienta-se que é necessário justificar cada etapa da construção do modelo, comentando desde a escolha das features até o resultados do modelo final.

* **Tarefas obrigatórias:**
  * Ajustar um modelo de **regressão linear** utilizando o conjunto de dados. Convém realizar testes mudando as variáveis independentes usadas no modelo e realizar possíveis transformações.
  * Realizar a análise dos resíduos do modelo final.

* **Entrega:**
  * Um notebook contendo:
    * O modelo final com explicações sobre as decisões tomadas
    * Análise dos resíduos
    * As previsões do modelo sobre o conjunto de validação, acompanhadas da discussão dos resultados
  * Os arquivos devem estar em um zip como explicado em [Formato de Submissão](#formato-de-submissão)

---

## Formato de Submissão

Sua submissão será um arquivo ZIP contendo os arquivos abaixo listados. O notebook deve ser salvo com o nome no formato `ExameB_<ETX>_<Estudante1>_<Estudante2>.ipynb`. Em `<ETX>` você deve preencher o código da etapa que está enviando, enquanto que em `<Estudante1>` e `<Estudante2>`, você deve indicar os nomes completos dos estudantes que fazem a dupla. A regra é similar para o nome do arquivo zip.

```text
  ExameB_<ETX>_<Estudante1>_<Estudante2>.zip
  ├── <dataset_estado>.csv
  └── ExameB_<ETX>_<Estudante1>_<Estudante2>.ipynb
```

**Atenção**: você pode criar seu notebook usando o Google Colab se desejar, mas deve exportá-lo no formato requerido antes do envio. Não serão aceitos o envio por link de compartilhamento.

## Avaliação

Cada entrega será avaliada com base nos seguintes critérios:

1. **Qualidade Técnica [4,5 pts]:** Este critério avalia a robustez metodológica e o rigor estatístico da sua solução. Espera-se que o código esteja correto e que as técnicas aplicadas sejam adequadas à natureza estatística de cada variável (o que difere do simples tipo de dado computacional). A pontuação depende da validação das premissas teóricas de cada teste ou modelo escolhido (como verificação de normalidade, homocedasticidade, etc.) e do tratamento fundamentado de dados ausentes e discrepantes (outliers). Não basta rodar uma função; é necessário demonstrar que a técnica escolhida é matematicamente válida para aquele cenário.

2. **Clareza [4,5 pts]:** Este critério avalia a capacidade de comunicação e o data storytelling. O notebook deve funcionar como um relatório técnico fluido e autoexplicativo, onde cada etapa de código é precedida por uma justificativa e sucedida por uma interpretação crítica. Gráficos devem ser legíveis e acompanhados de análise textual (em células de texto/markdown) que traduza os números e p-valores em conclusões de negócio ou científicas. A ausência de discussão sobre os resultados ou a falta de organização lógica do raciocínio penalizarão a nota, mesmo que o código esteja funcional.

3. **Criatividade [1,0 pts]:** Este critério avalia a originalidade e a profundidade analítica. Valoriza-se a proatividade em ir além do roteiro básico: isso inclui a engenharia de atributos (criação ou transformação inteligente de variáveis para capturar novos padrões), a formulação de hipóteses de que fujam do óbvio e a exploração de relações complexas entre variáveis. Soluções que demonstrem curiosidade investigativa, insights não triviais ou o uso correto de técnicas complementares (que vão além das mostradas em sala) para enriquecer a análise serão recompensadas.

Para as Etapas de 1 a 2 serão geradas notas de 0 a 10 e serão lançadas como as atividades ET01 , ET02 em nossa planilha. A etapa de modelagem será lançada como Exame B. Isto significa que esta atividade terá maior peso na nota.

### Pontuação Adicional

Ao final da Etapa 3, as equipes serão convidadas a apresentar seus trabalhos. Nessa apresentação, os avaliadores poderão atribuir **até 1,0 ponto extra** às equipes que demonstrarem clareza na comunicação, qualidade dos insights e boa justificativa das análises realizadas.

## Sugestões de Formatação e Organização

## 2.1 Estrutura do Notebook

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

### 2.4 Justificativas Textuais

* Para cada tratamento de dados (outliers, imputação, codificação), inserir uma célula Markdown intitulada **Justificativa** com fundamentação teórica ou empírica.

* Para testes estatísticos:

  * Formular claramente as hipóteses nula (H₀) e alternativa (H₁).
  * Definir o **nível de significância** (por exemplo, α = 0,05).
  * Escolher e justificar o teste estatístico adequado (ex.: correlação de Pearson, Spearman, teste t, ANOVA).
  * Apresentar os **valores das estatísticas** calculadas e o **p-value**.
  * Concluir se rejeita ou não H₀, com base no p-valor.
  * Incluir uma **tabela resumida** com os principais resultados.

---

**Exemplo**: Hipótese 1 – Relação entre `A` e `B`

**Hipóteses formuladas:**

* H₀: Não há correlação significativa entre `A` e `B`.
* H₁: Existe correlação significativa entre `A` e `B`.

**Teste aplicado:** Correlação de Pearson  
**Nível de significância:** α = 0,05

**Resultados:**

| Estatística | Valor |
|-------------|-------|
| Correlação (r) | *preencher* |
| p-value        | *preencher* |

**Conclusão:** Escreva aqui se rejeita ou não H₀, e o que isso implica.

### 2.4 Reprodutibilidade

* **Random seed fixo** em todas operações aleatórias (`random_state=2025`).
* **Versões de pacotes**: no bloco inicial, exibir:

```python
  import pandas as pd, numpy as np, sklearn
  print(pd.__version__, np.__version__, sklearn.__version__)
```

---

*Boa sorte e mãos à obra!*
