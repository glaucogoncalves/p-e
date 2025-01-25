# Exame B: Competição de Previsão de Preços de Casas

Este exame foi planejado para ser conduzido no formato de uma **competição**, oferecendo a oportunidade de aplicar conceitos aprendidos em sala de aula de maneira prática. O objetivo principal é analisar um conjunto de dados real de preços de casas na cidade de Ames, Iowa, e projetar um modelo para prever preços nesta região.

Os alunos trabalharão em **duplas** e serão desafiados a explorar os dados, realizar testes de hipótese e construir um modelo preditivo.

---

## Conjunto de dados

O conjunto de dados fornecido (arquivo **`houses.csv`**) contém informações detalhadas sobre as casas, como o área do terreno, número de quartos, a idade da construção, entre outras características. Para detalhes acerca das váriaveis acesse o arquivo [**`data_description.md`**](data_description.md).

---

## Instruções do exame

O exame será dividido em **quatro etapas**, com **entregas sucessivas em datas disponibilizadas no SIGAA**. Cada etapa aborda um componente específico do processo de análise de dados e modelagem preditiva.

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
  - Gerar gráficos de dispersão para explorar as relações entre `SalePrice` e variáveis contínuas.
  - Criar boxplots ou violin plots para investigar como `SalePrice` varia entre categorias (ex.: `Neighborhood` ou `MSZoning`).
  - Calcular e interpretar uma matriz de correlação para as variáveis numéricas.
  - Relatar os padrões encontrados, destacando variáveis potencialmente relevantes para a modelagem.

- **Entrega:**
  - Um notebook contendo os gráficos, análises e interpretações das relações observadas.

### Etapa 3: Testes de Hipótese

Na terceira etapa, os alunos elaborarão hipóteses (no mínimo três) e farão testes estatísticos usando os dados disponíveis.

- **Possíveis análises:**
  - O preço das casas aumenta com o aumento do tamanho das casas?
  - O tipo do bairro onde a casa está localizada tem relação sobre os serviços públicos disponíveis?
  - O estado da casa tem relação com o ano em que foi construída?

- **Entrega:**
  - Um notebook explicando as hipóteses levantadas, os testes realizados (com a devida checagem das suposições) e a interpretação conclusiva sobre cada hipótese.

### Etapa 4: Modelagem Preditiva

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

1. **Qualidade Técnica:** O código está correto e segue as técnicas aprendidas em aula?
2. **Clareza:** O notebook está organizado, com explicações claras e gráficos bem apresentados?
3. **Criatividade:** Há originalidade na abordagem, com insights ou soluções criativas?

**Pontuação Adicional**

Na etapa de modelagem, a organização irá testar os modelos submetidos em um conjunto de dados oculto. As equipes com os melhores desempenhos em termos de $R^2$ sobre os dados ocultos serão recompensadas:

- **1º lugar:** 2 pontos extras no Exame B.
- **2º e 3º lugares:** 1 ponto extra no Exame B.

---

## Entrega e Submissão

- Os notebooks devem ser criados no **Google Colab** e o link de compartilhamento deve ser enviado via SIGAA.
- Entregas atrasadas não serão consideradas.

---

## Conclusão

Este exame/competição foi estruturado para transformar a avaliação em uma experiência prática, que simula situações reais enfrentadas por cientistas de dados. Mantenha o espírito de colaboração e criatividade, e aproveite esta oportunidade para aprender e crescer!

Boa sorte, e que vença a melhor análise!