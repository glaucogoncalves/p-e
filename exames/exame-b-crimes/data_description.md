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
| `communityname`      | Nome da comunidade (apenas informativo)                                            | String      |
| `countyCode`         | Código numérico do condado (muitos valores faltantes)                              | Numérico    |
| `communityCode`      | Código numérico da comunidade (muitos valores faltantes)                           | Numérico    |
| `fold`               | Número do *fold* para validação cruzada 10-fold (uso em testes pareados)           | Inteiro     |

## Variável dependente

| Nome da Variável     | Descrição                                                                          | Tipo        |
|----------------------|------------------------------------------------------------------------------------|-------------|
| `violentPerPop`    | Crimes violentos/100k habitantes              | Decimal     |

## Variáveis preditoras

### Dados Demográficos Básicos

| Nome da Variável     | Descrição                                                                          | Tipo        |
|----------------------|------------------------------------------------------------------------------------|-------------|
| `state`              | Sigla do estado (EUA)                                                              | Nominal     |
| `pop`         | População total                                                                    | Inteiro     |
| `perHoush`      | Média de pessoas por domicílio                                                    | Decimal     |
| `pctblack`       | % população afro-americana                                                         | Decimal     |
| `pctWhite`       | % população branca                                                                 | Decimal     |
| `pctAsian`       | % população de origem asiática                                                     | Decimal     |
| `pctHisp`        | % população de origem hispânica                                                    | Decimal     |
| `pct12-21`        | % população entre 12-21 anos                                                       | Decimal     |
| `pct12-29`        | % população entre 12-29 anos                                                       | Decimal     |
| pct16-24`        | % população entre 16-24 anos                                                       | Decimal     |
| `pct65up`         | % população com 65+ anos                                                           | Decimal     |
| `persUrban`          | População em áreas urbanas                                                         | Inteiro     |
| `pctUrban`           | % população em áreas urbanas                                                       | Decimal     |

### Renda e Economia

| Nome da Variável     | Descrição                                                                          | Tipo        |
|----------------------|------------------------------------------------------------------------------------|-------------|
| `medIncome`          | Renda familiar mediana                                                             | Inteiro     |
| `pctWwage`           | % domicílios com renda de salário (1989)                                           | Decimal     |
| `pctWfarm`       | % domicílios com renda agropecuária/autônoma (1989)                                | Decimal     |
| `pctWdiv`         | % domicílios com renda de investimentos (1989)                                     | Decimal     |
| `pctWsocsec`         | % domicílios com previdência social (1989)                                         | Decimal     |
| `pctWPubAsst`        | % domicílios com assistência pública (1989)                                        | Decimal     |
| `pctWRetire`         | % domicílios com renda de aposentadoria (1989)                                     | Decimal     |
| `medFamIncome`          | Renda familiar mediana (apenas famílias)                                           | Inteiro     |
| `perCapInc`          | Renda *per capita*                                                                 | Decimal     |
| `whitePerCap`        | Renda *per capita* (brancos)                                                       | Decimal     |
| `blackPerCap`        | Renda *per capita* (afro-americanos)                                               | Decimal     |
| `NAPerCap`       | Renda *per capita* (nativos americanos)                                            | Decimal     |
| `AsianPerCap`        | Renda *per capita* (asiáticos)                                                     | Decimal     |
| `otherPerCap`        | Renda *per capita* (outras etnias)                                                 | Decimal     |
| `hispPerCap`         | Renda *per capita* (hispânicos)                                                    | Decimal     |
| `persPoverty`        | Pessoas abaixo da linha da pobreza                                                 | Inteiro     |
| `pctPoverty`     | % população abaixo da linha da pobreza                                             | Decimal     |

### Educação e Emprego

| Nome da Variável     | Descrição                                                                          | Tipo        |
|----------------------|------------------------------------------------------------------------------------|-------------|
| `pctLowEdu`    | % população (25+ anos) com menos de 9 anos de estudo                               | Decimal     |
| `pctNotHSgrad`       | % população (25+ anos) sem ensino médio completo                                   | Decimal     |
| `pctCollGrad`        | % população (25+ anos) com ensino superior completo                                | Decimal     |
| `pctUnemploy`      | % população (16+ anos) desempregada                                                | Decimal     |
| `pctEmploy`          | % população (16+ anos) empregada                                                   | Decimal     |
| `pctEmployMfg`        | % empregados na indústria                                                          | Decimal     |
| `pctEmployProfServ`    | % empregados em serviços profissionais                                             | Decimal     |
| `pctOccupManu`       | % população (16+ anos) em ocupações industriais                                    | Decimal     |
| `pctOccupMgmt`   | % população (16+ anos) em cargos gerenciais/profissionais                          | Decimal     |

### Estrutura Familiar

| Nome da Variável         | Descrição                                                                  | Tipo        |
|--------------------------|----------------------------------------------------------------------------|-------------|
| `pctMaleDivorc`         | % homens divorciados                                                       | Decimal     |
| `pctMaleNevMar`         | % homens nunca casados                                                     | Decimal     |
| `pctFemDivorc`           | % mulheres divorciadas                                                     | Decimal     |
| `pctAllDivorc`            | % população divorciada                                                     | Decimal     |
| `persPerFam`             | Média de pessoas por família                                               | Decimal     |
| `pct2Par`             | % famílias com dois pais (com filhos)                                      | Decimal     |
| `pctKids2Par`            | % crianças em famílias com dois pais                                       | Decimal     |
| `pctKids-4w2Par`       | % crianças (≤4 anos) em famílias com dois pais                             | Decimal     |
| `pct12-17w2Par`            | % adolescentes (12-17 anos) em famílias com dois pais                      | Decimal     |
| `pctWorkMom-6`    | % mães (com filhos ≤6 anos) no mercado de trabalho                         | Decimal     |
| `pctWorkMom-18`             | % mães (com filhos <18 anos) no mercado de trabalho                        | Decimal     |
| `kidsBornNevrMarr`    | Crianças nascidas de mães solteiras                                        | Inteiro     |
| `pctKidsBornNevrMarr`    | % crianças nascidas de mães solteiras                                      | Decimal     |

### Imigração e Habitação

| Nome da Variável         | Descrição                                                                  | Tipo        |
|--------------------------|----------------------------------------------------------------------------|-------------|
| `numForeignBorn`               | Pessoas nascidas no exterior                                               | Inteiro     |
| `pctFgnImmig-3`         | % imigrantes chegados nos últimos 3 anos                                   | Decimal     |
| `pctFgnImmig-5`           | % imigrantes chegados nos últimos 5 anos                                   | Decimal     |
| `pctFgnImmig-8`           | % imigrantes chegados nos últimos 8 anos                                   | Decimal     |
| `pctFgnImmig-10`          | % imigrantes chegados nos últimos 10 anos                                  | Decimal     |
| `pctImmig-3`         | % população imigrante recente (≤3 anos)                                    | Decimal     |
| `pctImmig-5`           | % população imigrante (≤5 anos)                                            | Decimal     |
| `pctImmig-8`           | % população imigrante (≤8 anos)                                            | Decimal     |
| `pctImmig-10`          | % população imigrante (≤10 anos)                                           | Decimal     |
| `pctSpeakOnlyEng`       | % população que fala apenas inglês                                         | Decimal     |
| `pctNotSpeakEng`    | % população com dificuldade em inglês                                      | Decimal     |
| `pctLargHousFam`        | % famílias em domicílios grandes (6+ pessoas)                             | Decimal     |
| `pctLargHous`      | % domicílios ocupados grandes (6+ pessoas)                                | Decimal     |
| `persPerOccupHous`       | Média de pessoas por domicílio ocupado                                     | Decimal     |
| `persPerOwnOccup`      | Média de pessoas em domicílios próprios                                    | Decimal     |
| `persPerRenterOccup`     | Média de pessoas em domicílios alugados                                    | Decimal     |
| `pctPersOwnOccup`        | % população em domicílios próprios                                         | Decimal     |
| `pctPopDenseHous`       | % população em moradias superlotadas (>1 pessoa/cômodo)                    | Decimal     |
| `pctSmallHousUnits`         | % domicílios com < 3 quartos                                                | Decimal     |
| `medNumBedrm`               | Número mediano de quartos                                                  | Decimal     |
| `houseVacant`             | Domicílios vagos                                                           | Inteiro     |
| `pctHousOccup`           | % domicílios ocupados                                                      | Decimal     |
| `pctHousOwnerOccup`          | % domicílios próprios ocupados                                             | Decimal     |
| `pctVacantBoarded`       | % domicílios vagos com entradas vedadas                                    | Decimal     |
| `pctVacant6up`         | % domicílios vagos >6 meses                                                | Decimal     |
| `medYrHousBuilt`         | Ano mediano de construção dos imóveis                                      | Inteiro     |
| `pctHousWOphone`         | % domicílios sem telefone (1990)                                           | Decimal     |
| `pctHousWOplumb`         | % domicílios sem instalações sanitárias completas                          | Decimal     |
| `ownHousLowQ`         | 1º quartil do valor de imóveis próprios                                    | Decimal     |
| `ownHousMed`           | Valor mediano de imóveis próprios                                          | Decimal     |
| `ownHousUperQ`          | 3º quartil do valor de imóveis próprios                                    | Decimal     |
| `ownHousQrange`           | Diferença interquartil de valores de imóveis próprios                       | Decimal     |
| `rentLowQ`               | 1º quartil do aluguel                                                      | Decimal     |
| `rentMed`             | Mediana do aluguel                                                         | Decimal     |
| `rentUpperQ`              | 3º quartil do aluguel                                                      | Decimal     |
| `rentQrange`             | Diferença interquartil de aluguéis                                         | Decimal     |
| `medGrossRent`                | Aluguel mediano bruto (inclui utilities)                                   | Decimal     |
| `medRentpctHousInc`      | Aluguel bruto como % da renda familiar                                     | Decimal     |
| `medOwnCostpct`       | Custo do imóvel próprio como % da renda (com hipoteca)                     | Decimal     |
| `medOwnCostPctWO`  | Custo do imóvel próprio como % da renda (sem hipoteca)                     | Decimal     |
| `persEmergShelt`          | Pessoas em abrigos para sem-teto                                           | Inteiro     |
| `persHomeless`              | Pessoas em situação de rua                                                 | Inteiro     |

### Mobilidade e Origem

| Nome da Variável     | Descrição                                                                  | Tipo        |
|----------------------|----------------------------------------------------------------------------|-------------|
| `pctForeignBorn`     | % população nascida no exterior                                            | Decimal     |
| `pctBornStateResid`   | % população nascida no estado atual                                        | Decimal     |
| `pctSameHouse-5`     | % população na mesma residência (vs. 1985)                                 | Decimal     |
| `pctSameCounty-5`      | % população na mesma cidade (vs. 1985)                                     | Decimal     |
| `pctSameState-5`     | % população no mesmo estado (vs. 1985)                                     | Decimal     |

### Policiamento

| Nome da Variável         | Descrição                                                                  | Tipo        |
|--------------------------|----------------------------------------------------------------------------|-------------|
| `numPolice`           | Policiais em tempo integral                                                | Inteiro     |
| `policePerPop`        | Policiais/100k habitantes                                                  | Decimal     |
| `policeField`      | Policiais em operações de campo                                            | Inteiro     |
| `policeFieldPerPop`   | Policiais em campo/100k habitantes                                         | Decimal     |
| `policeCalls`          | Total de solicitações policiais                                            | Inteiro     |
| `policCallPerPop`      | Solicitações policiais/100k habitantes                                     | Decimal     |
| `policCallPerOffic`       | Solicitações por policial                                                  | Decimal     |
| `policePerPop2`            | Policiais/100k habitantes                                                  | Decimal     |
| `racialMatch`     | Similaridade racial entre comunidade e polícia                             | Decimal     |
| `pctPolicWhite`          | % policiais brancos                                                        | Decimal     |
| `pctPolicBlack`          | % policiais afro-americanos                                                | Decimal     |
| `pctPolicHisp`           | % policiais hispânicos                                                     | Decimal     |
| `pctPolicAsian`          | % policiais asiáticos                                                      | Decimal     |
| `pctPolicMinority`          | % policiais de minorias                                                    | Decimal     |
| `officDrugUnits`    | Policiais em unidades anti-drogas                                          | Inteiro     |
| `numDiffDrugsSeiz`      | Tipos de drogas apreendidas                                                | Inteiro     |
| `policAveOT`       | Média de horas extras policiais                                            | Decimal     |
| `landArea`               | Área territorial (mi²)                                                     | Decimal     |
| `popDensity`                | Densidade populacional (pessoas/mi²)                                       | Decimal     |
| `pctUsePubTrans`         | % população que usa transporte público                                     | Decimal     |
| `policCarsAvail`              | Viaturas policiais                                                         | Inteiro     |
| `policOperBudget`          | Orçamento operacional da polícia                                           | Inteiro     |
| `pctPolicPatrol`    | % policiais em patrulha                                                    | Decimal     |
| `gangUnit`    | Unidade anti-gangues implantada (0=Não, 10=Sim, 5=Parcial)                 | Inteiro     |
| `pctOfficDrugUnit`    | % policiais em unidades anti-drogas                                        | Decimal     |
| `policBudgetPerPop`        | Orçamento policial per capita                                              | Decimal     |
| `murders`                | Número de homicídios (1995)                                                | Inteiro     |
| `murdPerPop`             | Homicídios/100k habitantes                                                 | Decimal     |
| `rapes`                  | Número de estupros (1995)                                                  | Inteiro     |
| `rapesPerPop`            | Estupros/100k habitantes                                                   | Decimal     |
| `robberies`              | Número de roubos (1995)                                                    | Inteiro     |
| `robbbPerPop`            | Roubos/100k habitantes                                                     | Decimal     |
| `assaults`               | Número de agressões (1995)                                                 | Inteiro     |
| `assaultPerPop`          | Agressões/100k habitantes                                                  | Decimal     |
| `burglaries`             | Número de arrombamentos (1995)                                             | Inteiro     |
| `burglPerPop`            | Arrombamentos/100k habitantes                                              | Decimal     |
| `larcenies`              | Número de furtos (1995)                                                    | Inteiro     |
| `larcPerPop`             | Furtos/100k habitantes                                                     | Decimal     |
| `autoTheft`              | Número de furtos de veículos (1995)                                        | Inteiro     |
| `autoTheftPerPop`        | Furtos de veículos/100k habitantes                                         | Decimal     |
| `arsons`                 | Número de incêndios criminosos (1995)                                      | Inteiro     |
| `arsonsPerPop`           | Incêndios criminosos/100k habitantes                                       | Decimal     |
| `nonViolPerPop`          | Crimes não-violentos/100k habitantes                                       | Decimal     |
| `violentPerPop`|Crimes violentos/100k habitantes | decimal
