# Exame B – Previsão de Preços de Passagens Aéreas

Neste exame, a avaliação acontece em formato de **competição**: em vez de uma prova tradicional, as duplas vão trabalhar com um problema real de ciência de dados, do início ao fim. O desafio é investigar um conjunto de dados com preços de passagens aéreas de voos domésticos na Índia e, a partir dele, desenvolver um modelo capaz de estimar quanto custa uma passagem com base nas características do voo.

O trabalho será feito em **duplas**, e passa por três momentos: exploração dos dados, validação de hipóteses com estatística inferencial e construção de um modelo de regressão.

---

## Sobre os dados

Os dados estão no arquivo **`flights.csv`**, que reúne 40 mil registros de voos entre as seis maiores cidades indianas. Para cada voo há informações como companhia aérea, cidades de origem e destino, horários de partida e chegada, quantidade de escalas, classe do bilhete, duração da viagem e quantos dias faltavam para o voo no momento da consulta.

A descrição completa de cada coluna, com categorias e faixas de valores, está em [**`data_description.md`**](data_description.md). Recomenda-se ler esse arquivo antes de começar.

---

## Etapas do trabalho

O exame está organizado em **três etapas**, cada uma com sua própria entrega. Os prazos serão divulgados no SIGAA.

### Etapa 1: Exploração dos Dados

O ponto de partida é conhecer bem o dataset. Nesta etapa, a dupla deve examinar cada variável individualmente e, em seguida, observar como elas se relacionam, com foco principal em entender **o que faz o `price` subir ou cair**. Problemas como colunas sem utilidade, categorias raras ou valores extremos também devem ser identificados aqui, já que influenciam diretamente as decisões das etapas seguintes.

- **Sugestões do que investigar:**
  - Medidas resumo (média, mediana, desvio padrão, assimetria) para as variáveis numéricas.
  - Tabelas de frequência para as variáveis categóricas, apontando categorias dominantes e pouco representadas.
  - Histogramas e *boxplots* para visualizar o formato das distribuições e localizar possíveis *outliers*.
  - Verificação da qualidade dos dados (valores ausentes, duplicados, colunas sem utilidade para a análise), com proposta de tratamento.
  - Gráficos de dispersão entre `price` e as variáveis contínuas.
  - *Boxplots* ou *violin plots* para comparar a distribuição de `price` entre as categorias de uma variável.
  - Matriz de correlação entre as variáveis numéricas, com interpretação dos resultados.
  - Um fechamento destacando quais variáveis parecem mais promissoras para o modelo.

- **O que entregar:**
  - Notebook com as análises, gráficos e comentários explicando cada passo e o que foi observado.


### Etapa 2: Testes de Hipótese

Com o conhecimento adquirido na exploração, a dupla deve propor **pelo menos três hipóteses** sobre os dados e verificá-las usando testes estatísticos adequados.

- **Alguns exemplos de perguntas:**
  - Comprar com mais antecedência deixa a passagem mais barata?
  - Existe diferença no preço médio entre as companhias aéreas?
  - Voos diretos custam menos do que voos com escala?
  - A quantidade de escalas depende da companhia aérea?
  - O horário de partida interfere no valor da passagem?

- **O que entregar:**
  - Notebook apresentando cada hipótese, o teste escolhido, a verificação das suposições do teste e a conclusão obtida.

### Etapa 3: Construção do Modelo

Por fim, a dupla deve desenvolver um modelo de **regressão linear múltipla** que estime o preço da passagem. A variável resposta é `price`; como variáveis explicativas, podem ser usadas todas as demais colunas ou apenas as que a dupla julgar relevantes.

- **O que fazer:**
  - Ajustar o modelo de **regressão linear**, testando diferentes combinações de variáveis e possíveis transformações (por exemplo, logaritmo do preço, interações entre variáveis e codificação das categóricas).
  - Analisar os resíduos do modelo escolhido.
  - Avaliar a significância das variáveis por meio de ANOVA.

- **O que entregar:**
  - Notebook com:
    - O modelo final e a justificativa das escolhas feitas ao longo do processo
    - A análise dos resíduos

---

## Critérios de Avaliação

As três entregas serão corrigidas segundo os mesmos critérios:

1. **Qualidade Técnica** [4 pts]: o código funciona corretamente e aplica as técnicas vistas em aula?
2. **Clareza** [4 pts]: o notebook é bem organizado, com textos explicativos e gráficos fáceis de interpretar?
3. **Criatividade** [2 pts]: a dupla trouxe ideias próprias, abordagens diferentes ou análises que vão além do básico?

### Apresentações

Além dos notebooks, haverá apresentações em sala:

- Após a **Etapa 1 (ET01)**, metade das duplas, escolhida por sorteio, apresentará seus resultados.
- Após a **Etapa 2 (ET02)**, as duplas restantes apresentarão os resultados dessa etapa.
- A nota dessas apresentações entra como uma das atividades da disciplina (APR).

> Cada apresentação terá 10 minutos no total: 7 minutos de exposição e 3 minutos de perguntas. Um integrante, sorteado na hora, faz a apresentação, e o outro fica responsável por responder às perguntas do professor e dos colegas.


## Arguição Final (Nota do Exame B)

Depois da entrega da **Etapa 3 (ET03)**, cada aluno passará por uma arguição **individual** com o professor, em data e horário a serem definidos. A nota obtida nessa arguição será a nota do Exame B.

Como vai funcionar:

* **Quantidade de perguntas:** cada aluno responderá a **2 perguntas**.
* **Valor:** cada pergunta vale **5 pontos**.
* **Tempo:** 6 minutos por aluno.
* **Conteúdo:** fundamentos teóricos de regressão linear e o notebook entregue pela dupla na Etapa 3.



## Bônus da Competição

As duplas que quiserem disputar pontos extras devem incluir, ao final do notebook da Etapa 3, uma função que use o modelo já treinado para:

1. Ler um arquivo de teste cego chamado `TesteRegressao.csv`;
2. Gerar as previsões de `price` para cada linha;
3. Salvar um novo CSV contendo **somente** os valores previstos, com o nome no formato `NOME_ALUNO1-NOME_ALUNO2.csv`.

> **Como testar antes de entregar:** o repositório traz o arquivo `exemplo.csv`, com as 5 primeiras linhas do teste oficial. Ele tem as mesmas colunas do dataset original, exceto `price`. Basta renomeá-lo para `TesteRegressao.csv` no Colab e rodar a função para confirmar que o arquivo de saída é gerado sem erros.

> **Cuidado:** se o modelo foi treinado com o preço transformado (por exemplo, `log(price)`), as previsões precisam ser convertidas de volta para rúpias antes de serem salvas.

O desempenho será medido pelo $R^2$ calculado sobre os dados de teste ocultos:

- **1º lugar:** +2 pontos no Exame B.
- **2º e 3º lugares:** +1 ponto no Exame B.

---

## Regras de Entrega

- Todos os notebooks devem ser desenvolvidos em Python no Google Colab e enviados pelo SIGAA.
- Não serão aceitas entregas fora do prazo.

---

## Considerações Finais

A ideia deste exame é aproximar a avaliação do que acontece no dia a dia de quem trabalha com dados: entender o problema, explorar, testar ideias e construir um modelo defensável. Aproveitem para trocar ideias com o colega de dupla, experimentar abordagens diferentes e, principalmente, aprender com o processo.

---

## Orientações de Formatação e Organização

### Organização do Notebook

* **Resumo inicial e seções:** comece o notebook com um pequeno resumo dos objetivos e do que foi feito. Cada seção deve ter um cabeçalho no padrão `## Seção X – Nome da Seção`.

* **Hierarquia de títulos:** use os níveis de título do Markdown para deixar o notebook fácil de navegar, com `##` para as partes principais e `###` para os subtópicos. Por exemplo:

  * `## Etapa 1 – Análise Exploratória`
  * `### 1.1 Distribuição dos Preços`

* **Comentário no início de cada célula:** toda célula de código deve abrir com um comentário curto dizendo o que ela faz. Siga o padrão PEP8 (nomes descritivos, indentação correta e linhas de até 100 caracteres).

```python
  # Objetivo: Descrição sucinta
```

### Uso de Funções

* **Modularização:** organize o código em funções que representem as etapas do fluxo de trabalho (carregar dados, tratar, visualizar, modelar etc.). Não existe uma quantidade mínima, mas as funções devem evitar repetição de código e deixar claro o papel de cada parte da análise. Exemplo:

```python
def carregar_dados(caminho):
    """Lê o arquivo CSV e devolve um DataFrame."""
    # ...
    return df
```

* **Docstrings:** toda função deve ter uma docstring curta explicando o que faz, quais parâmetros recebe e o que retorna.

### Acompanhamento do Dataset

Depois de cada transformação importante nos dados, mostre como o dataset ficou antes e depois. Por exemplo:

```python
  print("Shape:", df.shape)
  print("Missing por coluna:\n", df.isna().sum())
  print("Estatísticas básicas:\n", df.describe().T)
```

### Justificativas

* Sempre que fizer algum tratamento nos dados (remoção de outliers, codificação, transformações), adicione uma célula Markdown com o título **Justificativa**, explicando o motivo da escolha com base teórica ou nos próprios dados.

* Nos testes estatísticos, cada hipótese deve conter:

  * As hipóteses nula (H₀) e alternativa (H₁) bem definidas.
  * O **nível de significância** adotado (ex.: α = 0,05).
  * O teste escolhido e o porquê da escolha (ex.: Pearson, Spearman, teste t, ANOVA, qui-quadrado).
  * O **valor da estatística** do teste e o **p-valor**.
  * A decisão de rejeitar ou não H₀ com base no p-valor.
  * Uma **tabela resumo** com os resultados.

---

**Modelo de apresentação**: Hipótese 1 – Antecedência da compra (`days_left`) e preço (`price`)

**Hipóteses:**

* H₀: Não existe correlação significativa entre `days_left` e `price`.
* H₁: Existe correlação significativa entre `days_left` e `price`.

**Teste utilizado:** Correlação de Spearman
**Nível de significância:** α = 0,05

**Resultados:**

| Estatística | Valor |
|-------------|-------|
| Correlação (ρ) | *preencher* |
| p-valor        | *preencher* |

**Conclusão:** Indique se H₀ foi rejeitada ou não e o que isso significa na prática.

### Reprodutibilidade

* Use **semente aleatória fixa** em todas as operações que envolvem aleatoriedade (`random_state=2025`).
* Mostre as **versões das bibliotecas** logo no início do notebook:

```python
  import pandas as pd, numpy as np, sklearn
  print(pd.__version__, np.__version__, sklearn.__version__)
```

---

Bom trabalho a todos, e que vença o melhor modelo!
