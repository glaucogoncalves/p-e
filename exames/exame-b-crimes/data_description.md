# Dataset Description

## Overview
- **Total de variáveis:** 147  
- **Variáveis preditivas:** 125  
- **Variáveis não-preditivas:** 4  
- **Variáveis alvo potenciais:** 18  

---

## Variáveis 
| Nome da Variável     | Descrição                                                                          | Tipo        |
|----------------------|------------------------------------------------------------------------------------|-------------|
| `communityname`      | Nome da comunidade (apenas informativo)                                            | String      |
| `countyCode`         | Código numérico do condado (muitos valores faltantes)                              | Numérico    |
| `communityCode`      | Código numérico da comunidade (muitos valores faltantes)                           | Numérico    |
| `fold`               | Número do *fold* para validação cruzada 10-fold (uso em testes pareados)           | Inteiro     |

---
### Dados Demográficos Básicos
| Nome da Variável     | Descrição                                                                          | Tipo        |
|----------------------|------------------------------------------------------------------------------------|-------------|
| `state`              | Sigla do estado (EUA)                                                              | Nominal     |
| `population`         | População total                                                                    | Inteiro     |
| `householdsize`      | Média de pessoas por domicílio                                                    | Decimal     |
| `racepctblack`       | % população afro-americana                                                         | Decimal     |
| `racePctWhite`       | % população branca                                                                 | Decimal     |
| `racePctAsian`       | % população de origem asiática                                                     | Decimal     |
| `racePctHisp`        | % população de origem hispânica                                                    | Decimal     |
| `agePct12t21`        | % população entre 12-21 anos                                                       | Decimal     |
| `agePct12t29`        | % população entre 12-29 anos                                                       | Decimal     |
| `agePct16t24`        | % população entre 16-24 anos                                                       | Decimal     |
| `agePct65up`         | % população com 65+ anos                                                           | Decimal     |
| `numbUrban`          | População em áreas urbanas                                                         | Inteiro     |
| `pctUrban`           | % população em áreas urbanas                                                       | Decimal     |

### Renda e Economia
| Nome da Variável     | Descrição                                                                          | Tipo        |
|----------------------|------------------------------------------------------------------------------------|-------------|
| `medIncome`          | Renda familiar mediana                                                             | Inteiro     |
| `pctWWage`           | % domicílios com renda de salário (1989)                                           | Decimal     |
| `pctWFarmSelf`       | % domicílios com renda agropecuária/autônoma (1989)                                | Decimal     |
| `pctWInvInc`         | % domicílios com renda de investimentos (1989)                                     | Decimal     |
| `pctWSocSec`         | % domicílios com previdência social (1989)                                         | Decimal     |
| `pctWPubAsst`        | % domicílios com assistência pública (1989)                                        | Decimal     |
| `pctWRetire`         | % domicílios com renda de aposentadoria (1989)                                     | Decimal     |
| `medFamInc`          | Renda familiar mediana (apenas famílias)                                           | Inteiro     |
| `perCapInc`          | Renda *per capita*                                                                 | Decimal     |
| `whitePerCap`        | Renda *per capita* (brancos)                                                       | Decimal     |
| `blackPerCap`        | Renda *per capita* (afro-americanos)                                               | Decimal     |
| `indianPerCap`       | Renda *per capita* (nativos americanos)                                            | Decimal     |
| `AsianPerCap`        | Renda *per capita* (asiáticos)                                                     | Decimal     |
| `OtherPerCap`        | Renda *per capita* (outras etnias)                                                 | Decimal     |
| `HispPerCap`         | Renda *per capita* (hispânicos)                                                    | Decimal     |
| `NumUnderPov`        | Pessoas abaixo da linha da pobreza                                                 | Inteiro     |
| `PctPopUnderPov`     | % população abaixo da linha da pobreza                                             | Decimal     |

### Educação e Emprego
| Nome da Variável     | Descrição                                                                          | Tipo        |
|----------------------|------------------------------------------------------------------------------------|-------------|
| `PctLess9thGrade`    | % população (25+ anos) com menos de 9 anos de estudo                               | Decimal     |
| `PctNotHSGrad`       | % população (25+ anos) sem ensino médio completo                                   | Decimal     |
| `PctBSorMore`        | % população (25+ anos) com ensino superior completo                                | Decimal     |
| `PctUnemployed`      | % população (16+ anos) desempregada                                                | Decimal     |
| `PctEmploy`          | % população (16+ anos) empregada                                                   | Decimal     |
| `PctEmplManu`        | % empregados na indústria                                                          | Decimal     |
| `PctEmplProfServ`    | % empregados em serviços profissionais                                             | Decimal     |
| `PctOccupManu`       | % população (16+ anos) em ocupações industriais                                    | Decimal     |
| `PctOccupMgmtProf`   | % população (16+ anos) em cargos gerenciais/profissionais                          | Decimal     |

### Estrutura Familiar
| Nome da Variável         | Descrição                                                                  | Tipo        |
|--------------------------|----------------------------------------------------------------------------|-------------|
| `MalePctDivorce`         | % homens divorciados                                                       | Decimal     |
| `MalePctNevMarr`         | % homens nunca casados                                                     | Decimal     |
| `FemalePctDiv`           | % mulheres divorciadas                                                     | Decimal     |
| `TotalPctDiv`            | % população divorciada                                                     | Decimal     |
| `PersPerFam`             | Média de pessoas por família                                               | Decimal     |
| `PctFam2Par`             | % famílias com dois pais (com filhos)                                      | Decimal     |
| `PctKids2Par`            | % crianças em famílias com dois pais                                       | Decimal     |
| `PctYoungKids2Par`       | % crianças (≤4 anos) em famílias com dois pais                             | Decimal     |
| `PctTeen2Par`            | % adolescentes (12-17 anos) em famílias com dois pais                      | Decimal     |
| `PctWorkMomYoungKids`    | % mães (com filhos ≤6 anos) no mercado de trabalho                         | Decimal     |
| `PctWorkMom`             | % mães (com filhos <18 anos) no mercado de trabalho                        | Decimal     |
| `NumKidsBornNeverMar`    | Crianças nascidas de mães solteiras                                        | Inteiro     |
| `PctKidsBornNeverMar`    | % crianças nascidas de mães solteiras                                      | Decimal     |

### Imigração e Habitação
| Nome da Variável         | Descrição                                                                  | Tipo        |
|--------------------------|----------------------------------------------------------------------------|-------------|
| `NumImmig`               | Pessoas nascidas no exterior                                               | Inteiro     |
| `PctImmigRecent`         | % imigrantes chegados nos últimos 3 anos                                   | Decimal     |
| `PctImmigRec5`           | % imigrantes chegados nos últimos 5 anos                                   | Decimal     |
| `PctImmigRec8`           | % imigrantes chegados nos últimos 8 anos                                   | Decimal     |
| `PctImmigRec10`          | % imigrantes chegados nos últimos 10 anos                                  | Decimal     |
| `PctRecentImmig`         | % população imigrante recente (≤3 anos)                                    | Decimal     |
| `PctRecImmig5`           | % população imigrante (≤5 anos)                                            | Decimal     |
| `PctRecImmig8`           | % população imigrante (≤8 anos)                                            | Decimal     |
| `PctRecImmig10`          | % população imigrante (≤10 anos)                                           | Decimal     |
| `PctSpeakEnglOnly`       | % população que fala apenas inglês                                         | Decimal     |
| `PctNotSpeakEnglWell`    | % população com dificuldade em inglês                                      | Decimal     |
| `PctLargHouseFam`        | % famílias em domicílios grandes (6+ pessoas)                             | Decimal     |
| `PctLargHouseOccup`      | % domicílios ocupados grandes (6+ pessoas)                                | Decimal     |
| `PersPerOccupHous`       | Média de pessoas por domicílio ocupado                                     | Decimal     |
| `PersPerOwnOccHous`      | Média de pessoas em domicílios próprios                                    | Decimal     |
| `PersPerRentOccHous`     | Média de pessoas em domicílios alugados                                    | Decimal     |
| `PctPersOwnOccup`        | % população em domicílios próprios                                         | Decimal     |
| `PctPersDenseHous`       | % população em moradias superlotadas (>1 pessoa/cômodo)                    | Decimal     |
| `PctHousLess3BR`         | % domicílios com < 3 quartos                                                | Decimal     |
| `MedNumBR`               | Número mediano de quartos                                                  | Decimal     |
| `HousVacant`             | Domicílios vagos                                                           | Inteiro     |
| `PctHousOccup`           | % domicílios ocupados                                                      | Decimal     |
| `PctHousOwnOcc`          | % domicílios próprios ocupados                                             | Decimal     |
| `PctVacantBoarded`       | % domicílios vagos com entradas vedadas                                    | Decimal     |
| `PctVacMore6Mos`         | % domicílios vagos >6 meses                                                | Decimal     |
| `MedYrHousBuilt`         | Ano mediano de construção dos imóveis                                      | Inteiro     |
| `PctHousNoPhone`         | % domicílios sem telefone (1990)                                           | Decimal     |
| `PctWOFullPlumb`         | % domicílios sem instalações sanitárias completas                          | Decimal     |
| `OwnOccLowQuart`         | 1º quartil do valor de imóveis próprios                                    | Decimal     |
| `OwnOccMedVal`           | Valor mediano de imóveis próprios                                          | Decimal     |
| `OwnOccHiQuart`          | 3º quartil do valor de imóveis próprios                                    | Decimal     |
| `OwnOccQrange`           | Diferença interquartil de valores de imóveis próprios                       | Decimal     |
| `RentLowQ`               | 1º quartil do aluguel                                                      | Decimal     |
| `RentMedian`             | Mediana do aluguel                                                         | Decimal     |
| `RentHighQ`              | 3º quartil do aluguel                                                      | Decimal     |
| `RentQrange`             | Diferença interquartil de aluguéis                                         | Decimal     |
| `MedRent`                | Aluguel mediano bruto (inclui utilities)                                   | Decimal     |
| `MedRentPctHousInc`      | Aluguel bruto como % da renda familiar                                     | Decimal     |
| `MedOwnCostPctInc`       | Custo do imóvel próprio como % da renda (com hipoteca)                     | Decimal     |
| `MedOwnCostPctIncNoMtg`  | Custo do imóvel próprio como % da renda (sem hipoteca)                     | Decimal     |
| `NumInShelters`          | Pessoas em abrigos para sem-teto                                           | Inteiro     |
| `NumStreet`              | Pessoas em situação de rua                                                 | Inteiro     |

### Mobilidade e Origem
| Nome da Variável     | Descrição                                                                  | Tipo        |
|----------------------|----------------------------------------------------------------------------|-------------|
| `PctForeignBorn`     | % população nascida no exterior                                            | Decimal     |
| `PctBornSameState`   | % população nascida no estado atual                                        | Decimal     |
| `PctSameHouse85`     | % população na mesma residência (vs. 1985)                                 | Decimal     |
| `PctSameCity85`      | % população na mesma cidade (vs. 1985)                                     | Decimal     |
| `PctSameState85`     | % população no mesmo estado (vs. 1985)                                     | Decimal     |

### Policiamento
| Nome da Variável         | Descrição                                                                  | Tipo        |
|--------------------------|----------------------------------------------------------------------------|-------------|
| `LemasSwornFT`           | Policiais em tempo integral                                                | Inteiro     |
| `LemasSwFTPerPop`        | Policiais/100k habitantes                                                  | Decimal     |
| `LemasSwFTFieldOps`      | Policiais em operações de campo                                            | Inteiro     |
| `LemasSwFTFieldPerPop`   | Policiais em campo/100k habitantes                                         | Decimal     |
| `LemasTotalReq`          | Total de solicitações policiais                                            | Inteiro     |
| `LemasTotReqPerPop`      | Solicitações policiais/100k habitantes                                     | Decimal     |
| `PolicReqPerOffic`       | Solicitações por policial                                                  | Decimal     |
| `PolicPerPop`            | Policiais/100k habitantes                                                  | Decimal     |
| `RacialMatchCommPol`     | Similaridade racial entre comunidade e polícia                             | Decimal     |
| `PctPolicWhite`          | % policiais brancos                                                        | Decimal     |
| `PctPolicBlack`          | % policiais afro-americanos                                                | Decimal     |
| `PctPolicHisp`           | % policiais hispânicos                                                     | Decimal     |
| `PctPolicAsian`          | % policiais asiáticos                                                      | Decimal     |
| `PctPolicMinor`          | % policiais de minorias                                                    | Decimal     |
| `OfficAssgnDrugUnits`    | Policiais em unidades anti-drogas                                          | Inteiro     |
| `NumKindsDrugsSeiz`      | Tipos de drogas apreendidas                                                | Inteiro     |
| `PolicAveOTWorked`       | Média de horas extras policiais                                            | Decimal     |
| `LandArea`               | Área territorial (mi²)                                                     | Decimal     |
| `PopDens`                | Densidade populacional (pessoas/mi²)                                       | Decimal     |
| `PctUsePubTrans`         | % população que usa transporte público                                     | Decimal     |
| `PolicCars`              | Viaturas policiais                                                         | Inteiro     |
| `PolicOperBudg`          | Orçamento operacional da polícia                                           | Inteiro     |
| `LemasPctPolicOnPatr`    | % policiais em patrulha                                                    | Decimal     |
| `LemasGangUnitDeploy`    | Unidade anti-gangues implantada (0=Não, 10=Sim, 5=Parcial)                 | Inteiro     |
| `LemasPctOfficDrugUn`    | % policiais em unidades anti-drogas                                        | Decimal     |
| `PolicBudgPerPop`        | Orçamento policial per capita                                              | Decimal     |
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
| `violentPerPop`    | **Atributo alvo principal:** Crimes violentos/100k habitantes              | Decimal     |
| `nonViolPerPop`          | Crimes não-violentos/100k habitantes                                       | Decimal     |

---

