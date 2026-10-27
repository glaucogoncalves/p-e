# Dataset Description - Demanda de Bicicletas Compartilhadas em Seul

## Overview

Este conjunto de dados reúne a quantidade de bicicletas alugadas **a cada hora** no sistema público de bicicletas compartilhadas de Seul (Coreia do Sul), junto com as condições meteorológicas registradas no mesmo horário e informações sobre o calendário (estação do ano, feriados e funcionamento do sistema).

O objetivo do estudo é entender como o clima e o calendário se relacionam com a demanda por bicicletas e construir um modelo capaz de prever o número de bicicletas alugadas em uma determinada hora (`Rented_Bike_Count`).

- **Arquivo de Entrada:**
  1. `bike_sharing.csv`: Contém os registros horários, com as variáveis preditoras e a variável dependente.

- **Período coberto:** 01/12/2017 a 30/11/2018.
- **Total de observações:** 7.008 registros horários.
- **Total de variáveis:** 14.
- **Variável dependente:** 1 (`Rented_Bike_Count`).
- **Variáveis de identificação/tempo:** 2 (`Date` e `Hour`).
- **Variáveis preditoras:** 11 (8 numéricas + 3 categóricas), além de `Date` e `Hour`.

> **Fonte:** Seoul Bike Sharing Demand, UCI Machine Learning Repository (licença CC BY 4.0). Os nomes das colunas foram padronizados para facilitar o uso em Python; as unidades de medida estão indicadas nas tabelas abaixo.

---

## Variáveis de Tempo

| Nome da Variável | Descrição | Tipo |
| :--- | :--- | :--- |
| `Date` | Data do registro, no formato `DD/MM/AAAA`. | Data |
| `Hour` | Hora do dia a que o registro se refere (0 a 23). | Numérica (Discreta) |

> **Nota:** Cada linha corresponde a uma hora de um dia. A coluna `Date` não deve ser usada diretamente no modelo, mas pode servir de base para criar novas variáveis.

---

## Variável Dependente (Alvo)

| Nome da Variável | Descrição | Tipo |
| :--- | :--- | :--- |
| `Rented_Bike_Count` | Quantidade de bicicletas alugadas naquela hora. Varia de 0 a 3.556, com média de 704,97 e mediana de 504,5. | Numérica (Discreta) |

---

## Variáveis Preditoras

### Dados Meteorológicos

| Nome da Variável | Descrição | Unidade | Tipo |
| :--- | :--- | :--- | :--- |
| `Temperature` | Temperatura do ar. Varia de -17,8 a 39,4 (média 12,91). | °C | Numérica |
| `Humidity` | Umidade relativa do ar. Varia de 0 a 98 (média 58,27). | % | Numérica |
| `Wind_Speed` | Velocidade do vento. Varia de 0 a 7,4 (média 1,73). | m/s | Numérica |
| `Visibility` | Visibilidade horizontal. Varia de 27 a 2.000 (média 1.434,96). | unidades de 10 m | Numérica |
| `Dew_Point_Temperature` | Temperatura do ponto de orvalho, ou seja, a temperatura em que o vapor d'água do ar começa a condensar. Varia de -30,6 a 26,8 (média 4,12). | °C | Numérica |
| `Solar_Radiation` | Radiação solar incidente. Varia de 0 a 3,52 (média 0,57). | MJ/m² | Numérica |
| `Rainfall` | Volume de chuva na hora. Varia de 0 a 29,5 (média 0,14). | mm | Numérica |
| `Snowfall` | Volume de neve na hora. Varia de 0 a 8,8 (média 0,08). | cm | Numérica |

### Dados de Calendário

| Nome da Variável | Descrição | Tipo |
| :--- | :--- | :--- |
| `Seasons` | Estação do ano. Possui 4 categorias: `Spring` (1.766), `Summer` (1.767), `Autumn` (1.747) e `Winter` (1.728). | Categórica |
| `Holiday` | Indica se o dia é feriado. Possui 2 categorias: `No Holiday` (6.660) e `Holiday` (348). | Categórica (Binária) |
| `Functioning_Day` | Indica se o sistema de bicicletas estava em funcionamento naquele dia. Possui 2 categorias: `Yes` (6.774) e `No` (234). | Categórica (Binária) |

---

## Observações para a Modelagem

- As variáveis categóricas precisarão ser **codificadas** (ex.: *one-hot encoding* / variáveis *dummy*) para uso na regressão linear. Lembre-se de deixar uma categoria de referência para evitar multicolinearidade perfeita.
- O arquivo de teste cego (`TesteRegressao.csv`) terá exatamente as mesmas colunas de `bike_sharing.csv`, exceto `Rented_Bike_Count`. Qualquer variável criada a partir das colunas originais deve ser recriada também no teste.
