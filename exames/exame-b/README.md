# Exame B: Competição de Previsão de Preços de Casas

Este exame foi planejado para ser conduzido no formato de uma **competição**, oferecendo a oportunidade de aplicar conceitos aprendidos em sala de aula de maneira prática, colaborativa e desafiadora. O objetivo principal é desenvolver um modelo de **regressão linear** para prever os preços de venda de casas na cidade de Ames, Iowa, utilizando um conjunto de dados real.

Os alunos trabalharão em **duplas** e serão desafiados a explorar os dados, realizar análises detalhadas e construir um modelo preditivo que será avaliado com base em sua capacidade de generalização.

---

## Datasets
O conjunto de dados fornecido contém informações detalhadas sobre as casas, como o tamanho do lote, o número de quartos, a idade da construção, entre outras características. Ele está dividido em dois arquivos:

1. **`train.csv`:** Este é o arquivo que será disponibilizado para os alunos. Ele contém os dados de treino, incluindo a variável alvo `SalePrice` (preço de venda das casas).
2. **`test.csv`:** Este arquivo será mantido **oculto pela organização** e será utilizado exclusivamente para avaliar o desempenho dos modelos submetidos na última etapa da competição.

Para mais detalhes a cerca das váriaveis acesse o arquivo **`data_description.txt`**

---

## Como Funcionará
O exame será dividido em **quatro etapas**, com entregas realizadas após as aulas correspondentes. Cada etapa aborda um componente específico do processo de análise de dados e modelagem preditiva.

### Etapa 1: Análise Unidimensional
Na primeira etapa, os alunos terão a tarefa de explorar cada variável de forma isolada. O objetivo é compreender melhor o conjunto de dados, identificar possíveis problemas (como valores ausentes ou outliers) e levantar hipóteses iniciais sobre os padrões presentes.

- **Tarefas:**
  - Calcular estatísticas descritivas para variáveis numéricas, como média, mediana, desvio padrão e assimetria.
  - Criar tabelas de frequência para variáveis categóricas, identificando as categorias mais frequentes e aquelas menos representadas.
  - Gerar gráficos como histogramas e boxplots para investigar distribuições e possíveis outliers.
  - Relatar valores ausentes nas variáveis e sugerir estratégias para tratá-los.

- **Entrega:**
  - Um notebook contendo as análises, gráficos e explicações claras de cada etapa.

- **Prazo:** 
  - A entrega deve ser realizada **1 semana após a aula sobre análise 1D**.

---

### Etapa 2: Análise Bidimensional
Na segunda etapa, os alunos deverão explorar as relações entre variáveis, com especial atenção às correlações entre `SalePrice` e as outras variáveis do dataset. Essa etapa é crucial para identificar quais variáveis podem ser mais importantes para a modelagem.

- **Tarefas:**
  - Gerar gráficos de dispersão para explorar as relações entre `SalePrice` e variáveis contínuas, como `GrLivArea` (área útil) ou `TotalBsmtSF` (área total do porão).
  - Criar boxplots ou violin plots para investigar como `SalePrice` varia entre categorias (ex.: `Neighborhood` ou `MSZoning`).
  - Calcular e interpretar uma matriz de correlação para as variáveis numéricas.
  - Relatar os padrões encontrados, destacando variáveis potencialmente relevantes para a modelagem.

- **Entrega:**
  - Um notebook contendo os gráficos, análises e interpretações das relações observadas.

- **Prazo:**
  - A entrega deve ser realizada **1 semana após a aula sobre análise 2D**.

---

### Etapa 3: Engenharia de Atributos
Na terceira etapa, os alunos terão a oportunidade de melhorar os dados disponíveis. Criar atributos novos e tratar valores ausentes será fundamental para aumentar o desempenho do modelo preditivo.

- **Tarefas:**
  - Criar novos atributos relevantes, como:
    - **`HouseAge`:** Idade da casa no ano de venda (calculada como `YrSold - YearBuilt`).
    - **`TotalPorchSF`:** Soma das áreas de todas as varandas.
    - **`Bathrooms`:** Soma dos banheiros completos e metade dos banheiros.
  - Tratar valores ausentes de maneira lógica, como imputar a mediana em variáveis numéricas ou substituir valores nulos por "None" em variáveis categóricas.
  - Explicar o motivo de cada transformação ou atributo criado.

- **Entrega:**
  - Um notebook com os novos atributos criados e o tratamento de valores ausentes, incluindo explicações detalhadas.

- **Prazo:**
  - A entrega deve ser realizada **1 semana após a aula sobre engenharia de atributos**.

---

### Etapa 4: Modelagem Preditiva
Na última etapa, os alunos deverão construir um modelo de regressão linear para prever os preços de venda das casas. A avaliação será baseada no desempenho do modelo no dataset oculto (`test.csv`).

- **Tarefas:**
  - Dividir o conjunto de treino (`train.csv`) em três partes:
    - **Treino:** Para ajustar o modelo (aproximadamente 70% dos dados).
    - **Validação:** Para ajustar os hiperparâmetros e avaliar o desempenho preliminar do modelo (aproximadamente 20% dos dados).
    - **Teste:** Para simular a generalização do modelo antes de submetê-lo (aproximadamente 10% dos dados).  
    *Nota: A divisão pode ser feita de forma manual ou utilizando técnicas como `train_test_split` do scikit-learn.*

  - Ajustar o modelo de **regressão linear** utilizando a parte de treino do conjunto de dados.
  - Avaliar o modelo no conjunto de **validação**, utilizando o **RMSE** (Root Mean Squared Error).
  - Comparar o desempenho no conjunto de **teste** e discutir possíveis problemas de overfitting ou underfitting.

- **Competição:**
  - A organização irá testar os modelos submetidos no arquivo oculto `test.csv` e calcular o RMSE.
  - As equipes com os menores RMSE receberão **bônus** de pontuação:
    - **1º lugar:** +2 pontos extras.
    - **2º e 3º lugares:** +1 ponto extra.

- **Entrega:**
  - Um notebook contendo:
    - A divisão dos dados.
    - O modelo ajustado.
    - O cálculo do RMSE nos conjuntos de validação e teste.
    - Gráficos e análises que expliquem os resultados obtidos (ex.: gráficos de dispersão dos erros).

- **Prazo:**
  - A entrega deve ser realizada **1 semana após a aula sobre regressão linear**.

---

## Avaliação
Cada etapa será avaliada com base nos seguintes critérios:

1. **Qualidade Técnica:** O código está correto e segue as técnicas aprendidas em aula?
2. **Clareza:** O notebook está organizado, com explicações claras e gráficos bem apresentados?
3. **Criatividade:** Há originalidade na abordagem, com insights ou soluções criativas?

### Pontuação Adicional:
Na etapa de modelagem, as equipes com os melhores desempenhos no dataset oculto serão recompensadas:
- **1º lugar:** +2 pontos extras.
- **2º e 3º lugares:** +1 ponto extra.

---

## Entrega e Submissão
- Os notebooks devem ser enviados via **Google Colab** (compartilhando o link) ou no repositório do GitHub da equipe.
- Entregas atrasadas poderão ter penalidades definidas pela organização.

---

## Conclusão
Este exame/competição foi estruturado para transformar a avaliação em uma experiência prática e desafiadora (e quem sabe divertida), que simula situações reais enfrentadas por cientistas de dados. Mantenha o espírito de colaboração e criatividade, e aproveite esta oportunidade para aprender e crescer!

Boa sorte, e que vença a melhor análise!