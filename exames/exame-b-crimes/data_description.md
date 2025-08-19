# Dataset Description

## Overview

- **Total de variáveis:** 147
- **Variável dependente:** 1
- **Variáveis de identificação:** 4
- **Variáveis preditoras:** 142

---

## Variáveis de identificação

| Nome da Variável     | Descrição                                                                          | Tipo        |
|----------------------|------------------------------------------------------------------------------------|-------------|
| `communityname`      | Nome da comunidade (apenas informativo)                                            | Categórica      |
| `countyCode`         | Código numérico do condado (muitos valores faltantes)                              | Ordinal    |
| `communityCode`      | Código numérico da comunidade (muitos valores faltantes)                           | Ordinal    |
| `fold`               | Número do *fold* para validação cruzada 10-fold (uso em testes pareados)           | Numérica     |

## Variável dependente

| Nome da Variável     | Descrição                                                                          | Tipo        |
|----------------------|------------------------------------------------------------------------------------|-------------|
| `violentPerPop`    | Crimes violentos/100k habitantes              | Numérica     |

## Variáveis preditoras

### Dados Demográficos Básicos

| Nome da Variável     | Descrição                                                                          | Tipo        |
|----------------------|------------------------------------------------------------------------------------|-------------|
| `state`              | Sigla do estado (EUA)                                                              | Categórica     |
| `pop`         | População total                                                                    | Numérica     |
| `perHoush`      | Média de pessoas por domicílio                                                    | Numérica     |
| `pctblack`       | % população afro-americana                                                         | Numérica     |
| `pctWhite`       | % população branca                                                                 | Numérica     |
| `pctAsian`       | % população de origem asiática                                                     | Numérica     |
| `pctHisp`        | % população de origem hispânica                                                    | Numérica     |
| `pct12-21`        | % população entre 12-21 anos                                                       | Numérica     |
| `pct12-29`        | % população entre 12-29 anos                                                       | Numérica     |
| pct16-24`        | % população entre 16-24 anos                                                       | Numérica     |
| `pct65up`         | % população com 65+ anos                                                           | Numérica     |
| `persUrban`          | População em áreas urbanas                                                         | Numérica     |
| `pctUrban`           | % população em áreas urbanas                                                       | Numérica     |

### Renda e Economia

| Nome da Variável     | Descrição                                                                          | Tipo        |
|----------------------|------------------------------------------------------------------------------------|-------------|
| `medIncome`          | Renda familiar mediana                                                             | Numérica     |
| `pctWwage`           | % domicílios com renda de salário (1989)                                           | Numérica     |
| `pctWfarm`       | % domicílios com renda agropecuária/autônoma (1989)                                | Numérica     |
| `pctWdiv`         | % domicílios com renda de investimentos (1989)                                     | Numérica     |
| `pctWsocsec`         | % domicílios com previdência social (1989)                                         | Numérica     |
| `pctWPubAsst`        | % domicílios com assistência pública (1989)                                        | Numérica     |
| `pctWRetire`         | % domicílios com renda de aposentadoria (1989)                                     | Numérica     |
| `medFamIncome`          | Renda familiar mediana (apenas famílias)                                           | Numérica     |
| `perCapInc`          | Renda *per capita*                                                                 | Numérica     |
| `whitePerCap`        | Renda *per capita* (brancos)                                                       | Numérica     |
| `blackPerCap`        | Renda *per capita* (afro-americanos)                                               | Numérica     |
| `NAPerCap`       | Renda *per capita* (nativos americanos)                                            | Numérica     |
| `AsianPerCap`        | Renda *per capita* (asiáticos)                                                     | Numérica     |
| `otherPerCap`        | Renda *per capita* (outras etnias)                                                 | Numérica     |
| `hispPerCap`         | Renda *per capita* (hispânicos)                                                    | Numérica     |
| `persPoverty`        | Pessoas abaixo da linha da pobreza                                                 | Numérica     |
| `pctPoverty`     | % população abaixo da linha da pobreza                                             | Numérica     |

### Educação e Emprego

| Nome da Variável     | Descrição                                                                          | Tipo        |
|----------------------|------------------------------------------------------------------------------------|-------------|
| `pctLowEdu`    | % população (25+ anos) com menos de 9 anos de estudo                               | Numérica     |
| `pctNotHSgrad`       | % população (25+ anos) sem ensino médio completo                                   | Numérica     |
| `pctCollGrad`        | % população (25+ anos) com ensino superior completo                                | Numérica     |
| `pctUnemploy`      | % população (16+ anos) desempregada                                                | Numérica     |
| `pctEmploy`          | % população (16+ anos) empregada                                                   | Numérica     |
| `pctEmployMfg`        | % empregados na indústria                                                          | Numérica     |
| `pctEmployProfServ`    | % empregados em serviços profissionais                                             | Numérica     |
| `pctOccupManu`       | % população (16+ anos) em ocupações industriais                                    | Numérica     |
| `pctOccupMgmt`   | % população (16+ anos) em cargos gerenciais/profissionais                          | Numérica     |

### Estrutura Familiar

| Nome da Variável         | Descrição                                                                  | Tipo        |
|--------------------------|----------------------------------------------------------------------------|-------------|
| `pctMaleDivorc`         | % homens divorciados                                                       | Numérica     |
| `pctMaleNevMar`         | % homens nunca casados                                                     | Numérica     |
| `pctFemDivorc`           | % mulheres divorciadas                                                     | Numérica     |
| `pctAllDivorc`            | % população divorciada                                                     | Numérica     |
| `persPerFam`             | Média de pessoas por família                                               | Numérica     |
| `pct2Par`             | % famílias com dois pais (com filhos)                                      | Numérica     |
| `pctKids2Par`            | % crianças em famílias com dois pais                                       | Numérica     |
| `pctKids-4w2Par`       | % crianças (≤4 anos) em famílias com dois pais                             | Numérica     |
| `pct12-17w2Par`            | % adolescentes (12-17 anos) em famílias com dois pais                      | Numérica     |
| `pctWorkMom-6`    | % mães (com filhos ≤6 anos) no mercado de trabalho                         | Numérica     |
| `pctWorkMom-18`             | % mães (com filhos <18 anos) no mercado de trabalho                        | Numérica     |
| `kidsBornNevrMarr`    | Crianças nascidas de mães solteiras                                        | Numérica     |
| `pctKidsBornNevrMarr`    | % crianças nascidas de mães solteiras                                      | Numérica     |

### Imigração e Habitação

| Nome da Variável         | Descrição                                                                  | Tipo        |
|--------------------------|----------------------------------------------------------------------------|-------------|
| `numForeignBorn`               | Pessoas nascidas no exterior                                               | Numérica     |
| `pctFgnImmig-3`         | % imigrantes chegados nos últimos 3 anos                                   | Numérica     |
| `pctFgnImmig-5`           | % imigrantes chegados nos últimos 5 anos                                   | Numérica     |
| `pctFgnImmig-8`           | % imigrantes chegados nos últimos 8 anos                                   | Numérica     |
| `pctFgnImmig-10`          | % imigrantes chegados nos últimos 10 anos                                  | Numérica     |
| `pctImmig-3`         | % população imigrante recente (≤3 anos)                                    | Numérica     |
| `pctImmig-5`           | % população imigrante (≤5 anos)                                            | Numérica     |
| `pctImmig-8`           | % população imigrante (≤8 anos)                                            | Numérica     |
| `pctImmig-10`          | % população imigrante (≤10 anos)                                           | Numérica     |
| `pctSpeakOnlyEng`       | % população que fala apenas inglês                                         | Numérica     |
| `pctNotSpeakEng`    | % população com dificuldade em inglês                                      | Numérica     |
| `pctLargHousFam`        | % famílias em domicílios grandes (6+ pessoas)                             | Numérica     |
| `pctLargHous`      | % domicílios ocupados grandes (6+ pessoas)                                | Numérica     |
| `persPerOccupHous`       | Média de pessoas por domicílio ocupado                                     | Numérica     |
| `persPerOwnOccup`      | Média de pessoas em domicílios próprios                                    | Numérica     |
| `persPerRenterOccup`     | Média de pessoas em domicílios alugados                                    | Numérica     |
| `pctPersOwnOccup`        | % população em domicílios próprios                                         | Numérica     |
| `pctPopDenseHous`       | % população em moradias superlotadas (>1 pessoa/cômodo)                    | Numérica     |
| `pctSmallHousUnits`         | % domicílios com < 3 quartos                                                | Numérica     |
| `medNumBedrm`               | Número mediano de quartos                                                  | Numérica     |
| `houseVacant`             | Domicílios vagos                                                           | Numérica     |
| `pctHousOccup`           | % domicílios ocupados                                                      | Numérica     |
| `pctHousOwnerOccup`          | % domicílios próprios ocupados                                             | Numérica     |
| `pctVacantBoarded`       | % domicílios vagos com entradas vedadas                                    | Numérica     |
| `pctVacant6up`         | % domicílios vagos >6 meses                                                | Numérica     |
| `medYrHousBuilt`         | Ano mediano de construção dos imóveis                                      | Numérica     |
| `pctHousWOphone`         | % domicílios sem telefone (1990)                                           | Numérica     |
| `pctHousWOplumb`         | % domicílios sem instalações sanitárias completas                          | Numérica     |
| `ownHousLowQ`         | 1º quartil do valor de imóveis próprios                                    | Numérica     |
| `ownHousMed`           | Valor mediano de imóveis próprios                                          | Numérica     |
| `ownHousUperQ`          | 3º quartil do valor de imóveis próprios                                    | Numérica     |
| `ownHousQrange`           | Diferença interquartil de valores de imóveis próprios                       | Numérica     |
| `rentLowQ`               | 1º quartil do aluguel                                                      | Numérica     |
| `rentMed`             | Mediana do aluguel                                                         | Numérica     |
| `rentUpperQ`              | 3º quartil do aluguel                                                      | Numérica     |
| `rentQrange`             | Diferença interquartil de aluguéis                                         | Numérica     |
| `medGrossRent`                | Aluguel mediano bruto (inclui utilities)                                   | Numérica     |
| `medRentpctHousInc`      | Aluguel bruto como % da renda familiar                                     | Numérica     |
| `medOwnCostpct`       | Custo do imóvel próprio como % da renda (com hipoteca)                     | Numérica     |
| `medOwnCostPctWO`  | Custo do imóvel próprio como % da renda (sem hipoteca)                     | Numérica     |
| `persEmergShelt`          | Pessoas em abrigos para sem-teto                                           | Numérica     |
| `persHomeless`              | Pessoas em situação de rua                                                 | Numérica     |

### Mobilidade e Origem

| Nome da Variável     | Descrição                                                                  | Tipo        |
|----------------------|----------------------------------------------------------------------------|-------------|
| `pctForeignBorn`     | % população nascida no exterior                                            | Numérica     |
| `pctBornStateResid`   | % população nascida no estado atual                                        | Numérica     |
| `pctSameHouse-5`     | % população na mesma residência (vs. 1985)                                 | Numérica     |
| `pctSameCounty-5`      | % população na mesma cidade (vs. 1985)                                     | Numérica     |
| `pctSameState-5`     | % população no mesmo estado (vs. 1985)                                     | Numérica     |

### Policiamento

| Nome da Variável         | Descrição                                                                  | Tipo        |
|--------------------------|----------------------------------------------------------------------------|-------------|
| `numPolice`           | Policiais em tempo integral                                                | Numérica     |
| `policePerPop`        | Policiais/100k habitantes                                                  | Numérica     |
| `policeField`      | Policiais em operações de campo                                            | Numérica     |
| `policeFieldPerPop`   | Policiais em campo/100k habitantes                                         | Numérica     |
| `policeCalls`          | Total de solicitações policiais                                            | Numérica     |
| `policCallPerPop`      | Solicitações policiais/100k habitantes                                     | Numérica     |
| `policCallPerOffic`       | Solicitações por policial                                                  | Numérica     |
| `policePerPop2`            | Policiais/100k habitantes                                                  | Numérica     |
| `racialMatch`     | Similaridade racial entre comunidade e polícia                             | Numérica     |
| `pctPolicWhite`          | % policiais brancos                                                        | Numérica     |
| `pctPolicBlack`          | % policiais afro-americanos                                                | Numérica     |
| `pctPolicHisp`           | % policiais hispânicos                                                     | Numérica     |
| `pctPolicAsian`          | % policiais asiáticos                                                      | Numérica     |
| `pctPolicMinority`          | % policiais de minorias                                                    | Numérica     |
| `officDrugUnits`    | Policiais em unidades anti-drogas                                          | Numérica     |
| `numDiffDrugsSeiz`      | Tipos de drogas apreendidas                                                | Numérica     |
| `policAveOT`       | Média de horas extras policiais                                            | Numérica     |
| `landArea`               | Área territorial (mi²)                                                     | Numérica     |
| `popDensity`                | Densidade populacional (pessoas/mi²)                                       | Numérica     |
| `pctUsePubTrans`         | % população que usa transporte público                                     | Numérica     |
| `policCarsAvail`              | Viaturas policiais                                                         | Numérica     |
| `policOperBudget`          | Orçamento operacional da polícia                                           | Numérica     |
| `pctPolicPatrol`    | % policiais em patrulha                                                    | Numérica     |
| `gangUnit`    | Unidade anti-gangues implantada (0=Não, 10=Sim, 5=Parcial)                 | Numérica     |
| `pctOfficDrugUnit`    | % policiais em unidades anti-drogas                                        | Numérica     |
| `policBudgetPerPop`        | Orçamento policial per capita                                              | Numérica     |
| `murders`                | Número de homicídios (1995)                                                | Numérica     |
| `murdPerPop`             | Homicídios/100k habitantes                                                 | Numérica     |
| `rapes`                  | Número de estupros (1995)                                                  | Numérica     |
| `rapesPerPop`            | Estupros/100k habitantes                                                   | Numérica     |
| `robberies`              | Número de roubos (1995)                                                    | Numérica     |
| `robbbPerPop`            | Roubos/100k habitantes                                                     | Numérica     |
| `assaults`               | Número de agressões (1995)                                                 | Numérica     |
| `assaultPerPop`          | Agressões/100k habitantes                                                  | Numérica     |
| `burglaries`             | Número de arrombamentos (1995)                                             | Numérica     |
| `burglPerPop`            | Arrombamentos/100k habitantes                                              | Numérica     |
| `larcenies`              | Número de furtos (1995)                                                    | Numérica     |
| `larcPerPop`             | Furtos/100k habitantes                                                     | Numérica     |
| `autoTheft`              | Número de furtos de veículos (1995)                                        | Numérica     |
| `autoTheftPerPop`        | Furtos de veículos/100k habitantes                                         | Numérica     |
| `arsons`                 | Número de incêndios criminosos (1995)                                      | Numérica     |
| `arsonsPerPop`           | Incêndios criminosos/100k habitantes                                       | Numérica     |
| `nonViolPerPop`          | Crimes não-violentos/100k habitantes                                       | Numérica     |
| `violentPerPop`          | Crimes violentos/100k habitantes | decimal
