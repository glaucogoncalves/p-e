# Dataset Description - Produção Agrícola e Variáveis Climáticas na Amazônia

## Overview

Este conjunto de dados foi estruturado para estudar a relação entre a produção de insumos de produção agrícola/extrativismo vegetal na Amazônia e variáveis climáticas, hidrológicas e de queimadas .

O estudo deve ser realizado **por Estado (UF)**. O aluno deve selecionar um estado, escolher um insumo agrícola como variável alvo e utilizar as variáveis climáticas desse estado como preditores.

- **Arquivos de Entrada:**
  1. `insumos_{UF}.csv`: Contém a série histórica da produção (Variável Dependente).
  2. `features_{UF}.csv`: Contém as variáveis climáticas e ambientais mensais (Variáveis Preditoras).

- **Total de variáveis:** Varia conforme o estado (devido ao número de estações fluviométricas locais).
- **Variável dependente:** 1 (A ser escolhida pelo aluno dentro do arquivo de produção).
- **Variáveis de identificação:** 2 (`Data/Ano` e `UF`).
- **Variáveis preditoras:** 19 fixas + variáveis hidrológicas específicas por estado.

---

## Estrutura dos Tipos de Produção Agrícola (IBGE)

As colunas nos arquivos de produção agrícola seguem a codificação da Pesquisa da Extração Vegetal e Silvicultura (PEVS) do IBGE. O número inicial indica a categoria do grupo botânico/econômico:

| Grupo (Código) | Categoria | Exemplos |
| :--- | :--- | :--- |
| **1** | **Alimentícios** | 1.1 - Açaí, 1.3 - Castanha-do-pará |
| **2** | **Aromáticos, medicinais, tóxicos e corantes** | 2.1 - Ipecacuanha, 2.3 - Urucum |
| **3** | **Borrachas** | 3.2 - Látex coagulado (Hevea) |
| **4** | **Ceras** | 4.1 - Carnaúba (cera) |
| **5** | **Fibras** | 5.1 - Buriti, 5.3 - Piaçava |
| **6** | **Gomas não elásticas** | 6.1 - Balata, 6.3 - Sorva |
| **8** | **Oleaginosos** | 8.1 - Babaçu, 8.2 - Copaíba |
| **10** | **Tanantes** | 10.1 - Angico |

> **Nota:** No arquivo de produção, as colunas representam as subcategorias (ex: `1.1 - Açaí (fruto)`).

---

## Variáveis de Identificação e Chave

Estas variáveis são usadas para fazer o *merge* (junção) entre o dataset de clima e o de produção.

| Nome da Variável | Descrição | Tipo |
| :--- | :--- | :--- |
| `Data` / `Ano` | Data do registro. No dataset climático é mensal (AAAA-MM), na produção é anual (AAAA). A agregação deve ser feita anualmente para análise. | Data/Tempo |
| `UF` | Sigla da Unidade Federativa (Estado) a que os dados se referem. | Categórica |

---

## Variável Dependente (Alvo)

Localizada nos arquivos `insumos_{UF}.csv`. O aluno deve escolher **uma** coluna deste arquivo para ser o $Y$ (alvo) do estudo (e consequentemente do modelo).

| Nome da Variável | Descrição | Tipo |
| :--- | :--- | :--- |
| `[Código] - [Nome do Insumo]` | Quantidade produzida (em toneladas ou kg) do insumo selecionado naquele ano para o estado. (Ex: `1.1 - Açaí (fruto)`). | Numérica |

---

## Variáveis Preditoras

Localizadas nos arquivos `features_{UF}.csv`. Estas variáveis representam as condições ambientais agregadas para o estado inteiro.

### Dados de Queimadas (INPE)

| Nome da Variável | Descrição | Tipo |
| :--- | :--- | :--- |
| `Total_Focos` | Contagem total de focos de calor detectados por satélite no estado no mês. | Numérica (Discreta) |
| `Qtd_Municipios_Com_Fogo` | Quantidade de municípios distintos que registraram pelo menos um foco de calor no mês. | Numérica (Discreta) |
| `Media_Focos_Mun_Com_Fogo` | Média de focos de calor considerando apenas os municípios que tiveram fogo. | Numérica |
| `FRP_Medio` | *Fire Radiative Power* (Potência Radiativa do Fogo) média. Medida de intensidade do fogo (em MW). | Numérica |
| `FRP_Maximo` | Valor máximo de FRP registrado no mês (indica o incêndio mais intenso). | Numérica |
| `Risco_Fogo_Medio` | Média do índice de risco de fogo calculado (varia de 0 a 1 ou escala específica do INPE). | Numérica |
| `Dias_Secos_Medio` | Média de dias consecutivos sem chuva nos locais monitorados. | Numérica |

### Dados Climáticos e Atmosféricos

| Nome da Variável | Descrição | Tipo |
| :--- | :--- | :--- |
| `Precipitacao_Media` | Precipitação (chuva) média acumulada no estado (mm). | Numérica |
| `Precipitacao_Media_Local_Fogo` | Precipitação média estimada especificamente nas coordenadas onde ocorreram focos de fogo. | Numérica |
| `Temp_Max_Media` | Média das temperaturas máximas diárias (°C). | Numérica |
| `Temp_Min_Media` | Média das temperaturas mínimas diárias (°C). | Numérica |
| `Umidade_Relativa_Media` | Média da umidade relativa do ar (%). | Numérica |
| `VPD_Medio` | *Vapor Pressure Deficit* (Déficit de Pressão de Vapor). Mede a diferença entre a umidade real do ar e o máximo que ele poderia conter (saturação). | Numérica |
| `Evapotranspiracao_Media` | Quantidade média de água transferida do solo/plantas para a atmosfera (mm). | Numérica |
| `Radiacao_Solar_Media` | Radiação solar incidente média. | Numérica |
| `Velocidade_Vento_Media` | Velocidade média do vento (m/s). | Numérica |

### Dados Hidrológicos (Fluviométricos)

Estas colunas variam de nome conforme o estado, pois referem-se a estações de medição de rios locais (ANA).

| Nome da Variável | Descrição | Tipo |
| :--- | :--- | :--- |
| `NOME_RIO_CODIGO` | Nível médio ou vazão do rio registrado na estação específica (Ex: `RIO_BRANCO_13600002`). | Numérica |