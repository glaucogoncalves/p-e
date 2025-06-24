# Dataset Description

## Overview
- **Total de variáveis:** 147  
- **Variáveis preditivas:** 125  
- **Variáveis não-preditivas:** 4  
- **Variáveis alvo potenciais:** 18  

---

## Variáveis Não-Preditivas (4)
| Nome da Variável     | Descrição                                                                          | Tipo        |
|----------------------|------------------------------------------------------------------------------------|-------------|
| `communityname`      | Nome da comunidade (apenas informativo)                                            | String      |
| `countyCode`         | Código numérico do condado (muitos valores faltantes)                              | Numérico    |
| `communityCode`      | Código numérico da comunidade (muitos valores faltantes)                           | Numérico    |
| `fold`               | Número do *fold* para validação cruzada 10-fold (uso em testes pareados)           | Inteiro     |

---

## Variáveis Preditivas (125)
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

---

## Variáveis Alvo Potenciais (18)
| Nome da Variável         | Descrição                                                                  | Tipo        |
|--------------------------|----------------------------------------------------------------------------|-------------|
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

## Estatísticas Resumidas


## Estatísticas Resumidas Completas

| Variável                 | Mínimo      | Máximo         | Média         | Desvio Padrão  | Correlação c/ ViolPerPop | Mediana    | Moda       | Missing |
|--------------------------|-------------|----------------|---------------|----------------|--------------------------|------------|------------|---------|
| pop                      | 10005       | 7322564        | 53117.9842    | 204620.2529    | 0.212353809             | 22792      | 12361      | 0       |
| perHoush                 | 1.6         | 5.28           | 2.707327314   | 0.334119654    | -0.020110177            | 2.66       | 2.6        | 0       |
| pctBlack                 | 0           | 96.67          | 9.33510158    | 14.2471563     | 0.628367756             | 2.87       | 0.24       | 0       |
| pctWhite                 | 2.68        | 99.63          | 83.97981941   | 16.41908022    | -0.676848823            | 90.35      | 98.04      | 0       |
| pctAsian                 | 0.03        | 57.46          | 2.67020316    | 4.473843444    | 0.031949477             | 1.23       | 0.41       | 0       |
| pctHisp                  | 0.12        | 95.29          | 7.950176072   | 14.58983204    | 0.253596415             | 2.18       | 0.78       | 0       |
| pct12-21                 | 4.58        | 54.4           | 14.44583747   | 4.518622844    | 0.023535103             | 13.62      | 13.62      | 0       |
| pct12-29                 | 9.38        | 70.51          | 27.64483973   | 6.181517075    | 0.105908765             | 26.78      | 26.78      | 0       |
| pct16-24                 | 4.64        | 63.62          | 13.97514221   | 5.970746729    | 0.045251915             | 12.54      | 11.61      | 0       |
| pct65up                  | 1.66        | 52.77          | 11.83639278   | 4.777565216    | 0.055637064             | 11.73      | 11.06      | 0       |
| persUrban                | 0           | 7322564        | 47734.72009   | 205606.6933    | 0.21384036              | 18041      | 0          | 0       |
| pctUrban                 | 0           | 100            | 70.46530926   | 44.08027532    | 0.086294263             | 100        | 100        | 0       |
| medIncome                | 8866        | 123625         | 33984.69616   | 13424.68001    | -0.397407452            | 31441      | 27095      | 0       |
| pctWwage                 | 31.68       | 96.76          | 78.31275847   | 7.950672435    | -0.289829747            | 78.61      | 85.12      | 0       |
| pctWfarm                 | 0           | 6.53           | 0.881841986   | 0.689005635    | -0.148357317            | 0.69       | 0.54       | 0       |
| pctWdiv                  | 5.81        | 89.04          | 43.75093454   | 12.78792465    | -0.557786505            | 42.88      | 41.65      | 0       |
| pctWsocsec               | 4.81        | 76.39          | 26.40941761   | 8.295604161    | 0.107881101             | 26.59      | 21.51      | 0       |
| pctPubAsst               | 0.18        | 44.82          | 6.801444695   | 4.700334848    | 0.563107116             | 5.61       | 2.27       | 0       |
| pctRetire                | 3.46        | 45.51          | 15.96900226   | 4.622553011    | -0.098964807            | 15.65      | 13.14      | 0       |
| medFamIncome             | 10447       | 139008         | 39857.05508   | 14251.20603    | -0.411864109            | 36678      | 30546      | 0       |
| perCapInc                | 5237        | 63302          | 15603.5246    | 6281.558523    | -0.315255977            | 14101      | 11252      | 0       |
| whitePerCap              | 5472        | 68850          | 16567.69842   | 6346.840251    | -0.185898177            | 15073      | 12735      | 0       |
| blackPerCap              | 0           | 212120         | 11541.74944   | 9232.102062    | -0.209243037            | 9777       | 0          | 0       |
| NAperCap                 | 0           | 480000         | 12229.19142   | 14853.83618    | -0.060250637            | 9895       | 0          | 0       |
| asianPerCap              | 0           | 106165         | 14227.98962   | 9881.266395    | -0.128086386            | 12250      | 0          | 0       |
| otherPerCap              | 0           | 137000         | 9442.765131   | 7926.466713    | -0.103288444            | 8186       | 0          | 1       |
| hispPerCap               | 0           | 54648          | 11018.99819   | 5884.063446    | -0.219349786            | 9721       | 0          | 0       |
| persPoverty              | 78          | 1384994        | 7590.853273   | 39361.46001    | 0.240253072             | 2142       | 470        | 0       |
| pctPoverty               | 0.64        | 58             | 11.62053725   | 8.600352277    | 0.505349223             | 9.33       | 3.26       | 0       |
| pctLowEdu                | 0.2         | 49.89          | 9.186645598   | 6.66670296     | 0.371421768             | 7.74       | 5.78       | 0       |
| pctNotHSgrad             | 1.46        | 73.66          | 22.30511964   | 10.98951654    | 0.46759552              | 21.38      | 11.27      | 0       |
| pctCollGrad              | 1.63        | 79.18          | 23.05687585   | 12.68721342    | -0.299897539            | 19.65      | 14.2       | 0       |
| pctUnemploy              | 1.32        | 31.23          | 6.045241535   | 2.89561824     | 0.483440771             | 5.45       | 4.36       | 0       |
| pctEmploy                | 24.82       | 84.67          | 62.02161174   | 8.31204498     | -0.31764382             | 62.44      | 62.6       | 0       |
| pctEmployMfg             | 2.05        | 50.03          | 18.22890745   | 8.099280979    | -0.04712343             | 17.3       | 25.38      | 0       |
| pctEmployProfServ        | 8.69        | 62.67          | 24.53229797   | 6.659470242    | -0.064554813            | 23.39      | 21.52      | 0       |
| pctOccupManu             | 1.37        | 44.27          | 13.81916479   | 6.430263859    | 0.283898507             | 13.15      | 16.52      | 0       |
| pctOccupMgmt             | 6.48        | 64.97          | 28.2092009    | 9.326123364    | -0.324430512            | 26.24      | 28.31      | 0       |
| pctMaleDivorc            | 2.13        | 20.08          | 9.12758465    | 2.802747328    | 0.510455756             | 9.15       | 10.82      | 0       |
| pctMaleNevMar            | 12.06       | 76.6           | 30.68351693   | 8.127990901    | 0.271229742             | 29         | 26.78      | 0       |
| pctFemDivorc             | 3.35        | 23.92          | 12.32530023   | 3.262612867    | 0.537302801             | 12.52      | 14.36      | 0       |
| pctAllDivorc             | 2.83        | 22.23          | 10.81251467   | 3.000883481    | 0.536548564             | 10.9       | 11.77      | 0       |
| persPerFam               | 2.29        | 4.64           | 3.129697517   | 0.240742507    | 0.149955382             | 3.1        | 3.13       | 0       |
| pct2Par                  | 22.97       | 93.6           | 74.05912867   | 10.52595184    | -0.698640874            | 75.03      | 72.16      | 0       |
| pctKids2Par              | 18.3        | 92.58          | 71.22725508   | 12.04504833    | -0.728058986            | 72.53      | 63.25      | 0       |
| pctKids-4w2Par           | 8.7         | 100            | 81.86542212   | 12.26373565    | -0.658436367            | 83.99      | 100        | 0       |
| pct12-17w2Par            | 20.2        | 97.34          | 75.52178781   | 10.36526212    | -0.655627787            | 76.92      | 77.49      | 0       |
| pctWorkMom-6             | 24.42       | 87.97          | 60.54264108   | 8.008936744    | -0.02162507             | 60.71      | 63.48      | 0       |
| pctWorkMom-18            | 41.95       | 89.37          | 68.85479458   | 6.679959744    | -0.146173218            | 69.23      | 65.64      | 0       |
| kidsBornNevrMarr         | 0           | 527557         | 2141.418962   | 14692.58284    | 0.240337327             | 352        | 139        | 0       |
| pctKidsBornNevrMarr      | 0           | 27.35          | 3.115498871   | 3.127681493    | 0.738089083             | 2.04       | 0.97       | 0       |
| numForeignBorn           | 20          | 2082931        | 6277.273589   | 55419.65383    | 0.144585649             | 1024       | 147        | 0       |
| pctFgnImmig-3            | 0           | 64.29          | 13.525693     | 9.780097693    | 0.156688654             | 12.26      | 0          | 0       |
| pctFgnImmig-5            | 0           | 76.16          | 20.42128668   | 12.41035515    | 0.201445794             | 19.08      | 0          | 0       |
| pctFgnImmig-8            | 0           | 80.81          | 27.54418059   | 14.36881288    | 0.236607959             | 26.72      | 0          | 0       |
| pctFgnImmig-10           | 0           | 88             | 34.73392777   | 16.32732237    | 0.281536984             | 34.79      | 0          | 0       |
| pctImmig-3               | 0           | 13.71          | 1.099124153   | 1.595766262    | 0.215616823             | 0.5        | 0          | 0       |
| pctImmig-5               | 0           | 19.93          | 1.697462754   | 2.46105956     | 0.232900674             | 0.75       | 0          | 0       |
| pctImmig-8               | 0           | 25.34          | 2.307503386   | 3.286647928    | 0.23889175              | 1.04       | 0          | 0       |
| pctImmig-10              | 0           | 32.63          | 2.943760722   | 4.246468259    | 0.250865298             | 1.31       | 0          | 0       |
| pctSpeakOnlyEng          | 6.15        | 98.98          | 87.07499323   | 14.07608745    | -0.219031839            | 92.18      | 93.57      | 0       |
| pctNotSpeakEng           | 0           | 38.33          | 2.405792325   | 4.210367661    | 0.27243614              | 0.92       | 0.44       | 0       |
| pctLargHousFam           | 0.96        | 34.87          | 5.38661851    | 3.794309411    | 0.341601121             | 4.28       | 3.71       | 0       |
| pctLargHous              | 0.44        | 30.87          | 3.91578781    | 3.175770454    | 0.257215583             | 3.05       | 2.98       | 0       |
| persPerOccupHous         | 1.58        | 4.52           | 2.615841986   | 0.315646341    | -0.017700909            | 2.57       | 2.44       | 0       |
| persPerOwnOccup          | 1.61        | 4.48           | 2.74048307    | 0.297420849    | -0.099169625            | 2.71       | 2.65       | 0       |
| persPerRenterOccup       | 1.55        | 4.73           | 2.367137698   | 0.391805778    | 0.240564095             | 2.29       | 2.17       | 0       |
| pctPersOwnOccup          | 13.93       | 97.24          | 66.36945372   | 14.18258845    | -0.507329566            | 65.91      | 63.79      | 0       |
| pctPopDenseHous          | 0.05        | 59.49          | 4.132437923   | 5.599131346    | 0.395855647             | 2.34       | 1.31       | 0       |
| pctSmallHousUnits        | 3.06        | 95.34          | 45.40534086   | 13.77834736    | 0.454469731             | 46.39      | 53.15      | 0       |
| medNumBedrm              | 1           | 4              | 2.640632054   | 0.512686001    | -0.347149961            | 3          | 3          | 0       |
| houseVacant              | 36          | 172768         | 1748.368849   | 6503.866478    | 0.289690649             | 558        | 246        | 0       |
| pctHousOccup             | 37.47       | 99             | 92.93397291   | 5.04073584     | -0.256836226            | 94.21      | 95.38      | 0       |
| pctHousOwnerOccup        | 16.86       | 96.49          | 63.36829797   | 13.9700567     | -0.45535904             | 62.83      | 56.17      | 0       |
| pctVacantBoarded         | 0           | 39.89          | 2.778523702   | 3.592396207    | 0.479910148             | 1.66       | 0          | 0       |
| pctVacant6up             | 3.12        | 82.13          | 34.77388713   | 13.91146771    | 0.030768767             | 34.1       | 37.5       | 0       |
| medYrHousBuilt           | 1939        | 1987           | 1962.623476   | 11.16655501    | -0.111201128            | 1964       | 1939       | 0       |
| pctHousWOphone           | 0           | 23.88          | 4.289823928   | 4.088174777    | 0.473717673             | 2.85       | 0          | 0       |
| pctHousWOplumb           | 0           | 5.33           | 0.425273138   | 0.426188232    | 0.311226836             | 0.32       | 0          | 0       |
| ownHousLowQ              | 14999       | 500001         | 88695.80226   | 66670.78153    | -0.194912005            | 65500      | 34000      | 0       |
| ownHousMed               | 19500       | 500001         | 113097.5233   | 81906.36228    | -0.17822542             | 82800      | 500001     | 0       |
| ownHousUperQ             | 28200       | 500001         | 145318.2578   | 99030.91382    | -0.166029142            | 106700     | 500001     | 0       |
| ownHousQrange            | 0           | 331000         | 56622.45553   | 39106.49804    | -0.086578248            | 43400      | 28100      | 0       |
| rentLowQ                 | 99          | 1001           | 329.9665914   | 144.1384609    | -0.245708342            | 307        | 252        | 0       |
| rentMed                  | 120         | 1001           | 428.537246    | 170.7066437    | -0.232797807            | 397        | 316        | 0       |
| rentUpperQ               | 182         | 1001           | 527.2528217   | 199.29078      | -0.223893683            | 486        | 1001       | 0       |
| rentQrange               | 0           | 803            | 197.2862302   | 85.20568803    | -0.110281171            | 171        | 139        | 0       |
| medGrossRent             | 192         | 1001           | 501.4663657   | 169.2717347    | -0.231754244            | 467        | 1001       | 0       |
| medRentpctHousInc        | 14.9        | 35.1           | 26.29810384   | 2.979297132    | 0.315536838             | 26.1       | 24.7       | 0       |
| medOwnCostpct            | 14          | 32.7           | 20.99015801   | 2.987621666    | 0.061058949             | 21         | 22.6       | 0       |
| medOwnCostPctWO          | 10.1        | 23.4           | 13.01020316   | 1.419678674    | 0.063296009             | 12.8       | 11.8       | 0       |
| persEmergShelt           | 0           | 23383          | 66.95349887   | 564.253149     | 0.19494198              | 0          | 0          | 0       |
| persHomeless             | 0           | 10447          | 17.8234763    | 245.4525529    | 0.136446046             | 0          | 0          | 0       |
| pctForeignBorn           | 0.18        | 60.4           | 7.340302483   | 8.418475989    | 0.193229615             | 4.31       | 2.97       | 0       |
| pctBornStateResid        | 6.75        | 93.14          | 61.5396298    | 16.75006116    | -0.070943862            | 64.49      | 74.45      | 0       |
| pctSameHouse-5           | 11.83       | 78.56          | 51.53859594   | 10.51792598    | -0.14008735             | 52.17      | 54.85      | 0       |
| pctSameCounty-5          | 27.95       | 96.59          | 77.41107901   | 10.87818569    | 0.082634597             | 79.49      | 81.47      | 0       |
| pctSameState-5           | 32.83       | 99.9           | 88.11186456   | 7.287836465    | -0.006663834            | 90.03      | 92.69      | 0       |
| numPolice                | 65          | 25655          | 499.1982507   | 1681.472251    | 0.194219827             | 173        | 100        | 1872    |
| policePerPop             | 29.4        | 3437.23        | 246.4909621   | 273.7991617    | 0.073197363             | 196.01     | #N/A       | 1872    |
| policeField              | 14          | 22496          | 432.5597668   | 1493.708385    | 0.186477279             | 152        | 94         | 1872    |
| policeFieldPerPop        | 19.21       | 3290.62        | 210.8447813   | 235.4788145    | 0.065928304             | 170.27     | 183.22     | 1872    |
| policeCalls              | 2100        | 8328470        | 252404.9883   | 689449.7817    | 0.230023206             | 90000      | 50000      | 1872    |
| policCallPerPop          | 2704.8      | 1926281.5      | 120651.7189   | 148211.3422    | 0.14854896              | 91034.6    | #N/A       | 1872    |
| policCallPerOffic        | 20.8        | 2162.5         | 523.658309    | 307.8390067    | 0.145798061             | 443.2      | 422.6      | 1872    |
| policePerPop2            | 29.4        | 3437.2         | 246.493586    | 273.7984086    | 0.073203166             | 196        | 171.5      | 1872    |
| racialMatch              | 42.15       | 100            | 85.4996793    | 10.94131216    | -0.469374164            | 87.93      | 100        | 1872    |
| pctPolicWhite            | 1.6         | 100            | 82.5158309    | 15.33261214    | -0.392584252            | 86.18      | 100        | 1872    |
| pctPolicBlack            | 0           | 67.31          | 9.263294461   | 11.02142376    | 0.513568853             | 5          | 0          | 1872    |
| pctPolicHisp             | 0           | 98.4           | 5.459766764   | 10.60453332    | 0.056080974             | 2.04       | 0          | 1872    |
| pctPolicAsian            | 0           | 18.57          | 0.681282799   | 1.706344058    | 0.072778715             | 0          | 0          | 1872    |
| pctPolicMinority         | 0           | 98.4           | 15.2422449    | 14.82675626    | 0.416418453             | 11.37      | 0          | 1872    |
| officDrugUnits           | 0           | 1773           | 26.28862974   | 100.8219209    | 0.166934688             | 12         | 6          | 1872    |
| numDiffDrugsSeiz         | 1           | 15             | 8.816326531   | 2.836390802    | 0.115940631             | 9          | 9          | 1872    |
| policAveOT               | 0           | 634.7          | 119.1142857  | 92.49518559    | 0.010162351             | 98.7       | 0          | 1872    |
| landArea                 | 0.9         | 3569.8         | 27.41995485   | 109.8226001    | 0.075697852             | 13.7       | 4.9        | 0       |
| popDensity               | 10          | 44229.9        | 2783.835034   | 2828.993341    | 0.256966815             | 2027.3     | 3217.7     | 0       |
| pctUsePubTrans           | 0           | 54.33          | 3.041124153   | 4.91291686     | 0.190478991             | 1.22       | 0          | 0       |
| policCarsAvail           | 20          | 3187           | 185.4781341  | 318.5428335    | 0.313164478             | 86         | 55         | 1872    |
| policOperBudget          | 2380215     | 1617293056     | 32176019.34  | 110456627.5    | 0.195267289             | 11164110   | 8000000    | 1872    |
| pctPolicPatrol           | 10.85       | 99.94          | 87.13093294   | 10.34961235    | -0.093114808            | 89.58      | 93.07      | 1872    |
| gangUnit                 | 0           | 10             | 4.285714286   | 4.064537838    | 0.109156269             | 5          | 0          | 1872    |
| pctOfficDrugUnit         | 0           | 48.44          | 0.980162528   | 2.877127691    | 0.318474028             | 0          | 0          | 0       |
| policBudgetPerPop        | 15260.4     | 2422367        | 153577.8712  | 203040.8861    | 0.056100531             | 114582     | #N/A       | 1872    |
| murders                  | 0           | 1946           | 7.764785553  | 58.16646847    | 0.248259306             | 1          | 0          | 0       |
| murdPerPop               | 0           | 91.09          | 5.859295711   | 9.156828742    | 0.671541352             | 2.17       | 0          | 0       |
| rapes                    | 0           | 2818           | 28.04633782   | 105.6161353    | 0.336087881             | 7          | 0          | 208     |
| rapesPerPop              | 0           | 401.35         | 36.25848032   | 34.23974957    | 0.581533276             | 26.92      | 0          | 208     |
| robberies                | 0           | 86001          | 237.9521229  | 2250.720788    | 0.208547391             | 19         | 1          | 1       |
| robbbPerPop              | 0           | 2264.13        | 162.6125971  | 234.4866243    | 0.828574083             | 74.8       | 0          | 1       |
| assaults                 | 0           | 62778          | 326.5281562  | 1987.947941    | 0.301016534             | 56         | 12         | 13      |
| assaultPerPop            | 0           | 4932.5         | 378.0046049  | 438.2385994    | 0.945565838             | 226.525    | 0          | 13      |
| burglaries               | 2           | 99207          | 761.2368897  | 3111.702756    | 0.316504514             | 205        | 79         | 3       |
| burglPerPop              | 16.92       | 11881.02       | 1033.430203  | 763.3544416    | 0.698552626             | 822.715    | 728.93     | 3       |
| larcenies                | 10          | 235132         | 2137.629295  | 7600.573464    | 0.2950221               | 747        | 547        | 3       |
| larcPerPop               | 77.86       | 25910.55       | 3372.97915   | 1901.316145    | 0.509410495             | 3079.51    | 4631.1     | 3       |
| autoTheft                | 1           | 112464         | 516.6925859  | 3258.164244    | 0.244925811             | 75         | 16         | 3       |
| autoTheftPerPop          | 6.55        | 4968.59        | 473.9656284  | 504.6660256    | 0.636484339             | 302.355    | 213.62     | 3       |
| arsons                   | 0           | 5119           | 30.90772128  | 180.1252481    | 0.232824758             | 5          | 0          | 91      |
| arsonsPerPop             | 0           | 436.37         | 32.15368173  | 39.24090028    | 0.416718515             | 21.08      | 0          | 91      |
| violentPerPop            | 0           | 4877.06        | 589.0789218  | 614.7845182    | 1                      | 374.06     | 223.06     | 221     |
| nonViolPerPop            | 116.79      | 27119.76       | 4908.241804  | 2739.708901    | 0.675374243             | 4425.45    | 4295.96    | 97      |

## Distribuição da Variável Alvo Principal (`violentPerPop`)

### Frequência por Faixa
| Faixa de Valores       | Frequência |
|------------------------|------------|
| 0                      | 1          |
| 1 - 100                | 285        |
| 100 - 200              | 306        |
| 200 - 300              | 265        |
| 300 - 400              | 185        |
| 400 - 500              | 151        |
| 500 - 600              | 131        |
| 600 - 700              | 100        |
| 700 - 800              | 77         |
| 800 - 900              | 72         |
| 900 - 1000             | 61         |
| 1000 - 1100            | 38         |
| 1100 - 1200            | 33         |
| 1200 - 1300            | 50         |
| 1300 - 1400            | 35         |
| 1400 - 1500            | 30         |
| 1500 - 1600            | 28         |
| 1600 - 1700            | 28         |
| 1700 - 1800            | 14         |
| 1800 - 1900            | 12         |
| 1900 - 2000            | 14         |
| > 2000                 | 78         |

### Características Chave:
- **Assimetria positiva:** 75% dos valores abaixo de 800 crimes/100k hab
- **Outliers:** 78 comunidades (>2000) com extrema violência
- **Pico modal:** Faixa 100-200 crimes/100k hab (306 ocorrências)
- **Distribuição:** Não-normal com cauda pesada à direita

---

## Considerações para Modelagem
1. **Tratamento de Missing Values:**
   - Variáveis policiais: 1,872 registros faltantes (≈12% do dataset)
   - `arsons`: 91 valores ausentes
2. **Transformações Necessárias:**
   - Normalização de variáveis escalares (ex: renda, população)
   - Codificação one-hot para estado (nominal)
3. **Alvo:**
   - `ViolentCrimesPerPop` mostra distribuição exponencial
   - Sugere-se transformação logarítmica para modelagem