# Variáveis do conjunto de dados

`MSSubClass` Identifica o tipo de moradia envolvida na venda.	

        20	1-STORY 1946 & NEWER ALL STYLES
        30	1-STORY 1945 & OLDER
        40	1-STORY W/FINISHED ATTIC ALL AGES
        45	1-1/2 STORY - UNFINISHED ALL AGES
        50	1-1/2 STORY FINISHED ALL AGES
        60	2-STORY 1946 & NEWER
        70	2-STORY 1945 & OLDER
        75	2-1/2 STORY ALL AGES
        80	SPLIT OR MULTI-LEVEL
        85	SPLIT FOYER
        90	DUPLEX - ALL STYLES AND AGES
       120	1-STORY PUD (Planned Unit Development) - 1946 & NEWER
       150	1-1/2 STORY PUD - ALL AGES
       160	2-STORY PUD - 1946 & NEWER
       180	PUD - MULTILEVEL - INCL SPLIT LEV/FOYER
       190	2 FAMILY CONVERSION - ALL STYLES AND AGES

`MSZoning`: Identifica a classificação geral de zoneamento da venda.
		
       A	Agricultura
       C	Comercial
       FV	Residencial Vila Flutuante
       I	Industrial
       RH	Residencial Alta Densidade
       RL	Residencial Baixa Densidade
       RP	Residencial Baixa Densidade Parque
       RM	Residencial Média Densidade
	
`LotFrontage`: Pés lineares de rua conectados à propriedade.

`LotArea`: Tamanho do lote em pés quadrados

`Street`: Tipo de acesso rodoviário à propriedade

       Grvl	Cascalho	
       Pave	Pavimentada
       	
`Alley`: Tipo de acesso à propriedade

       Grvl	Cascalho
       Pave	Pavimentada
       NA 	Sem acesso
		
`LotShape`: Forma geral da propriedade

       Reg	Regular	
       IR1	Ligeiramente irregular
       IR2	Moderadamente irregular
       IR3	Irregular
       
`LandContour`: Planicidade do imóvel

       Lvl	Quase plano/nivelado	
       Bnk	Bancado - Aumento rápido e significativo do nível da rua para o edifício
       HLS	Encosta - Declive significativo de um lado para o outro
       Low	Depressão
		
`Utilities`: Tipo de utilidades disponíveis
		
       AllPub	Todos os serviços públicos (E,G,W,& S)	
       NoSewr	Eletricidade, Gás e Água (Fossa Séptica)
       NoSeWa	Somente eletricidade e gás
       ELO	Somente eletricidade	
	
`LotConfig`: Configuração do lote

       Inside	Dentro do lote
       Corner	Lote de esquina
       CulDSac	Beco sem saída
       FR2	Fachada em 2 lados da propriedade
       FR3	Fachada em 3 lados da propriedade
	
`LandSlope`: Declive da propriedade
		
       Gtl	Declive suave
       Mod	Declive moderado	
       Sev	Declive severo
	
`Neighborhood`: Locais físicos dentro dos limites da cidade de Ames

       Blmngtn	Bloomington Heights
       Blueste	Bluestem
       BrDale	Briardale
       BrkSide	Brookside
       ClearCr	Clear Creek
       CollgCr	College Creek
       Crawfor	Crawford
       Edwards	Edwards
       Gilbert	Gilbert
       IDOTRR	Iowa DOT and Rail Road
       MeadowV	Meadow Village
       Mitchel	Mitchell
       Names	North Ames
       NoRidge	Northridge
       NPkVill	Northpark Villa
       NridgHt	Northridge Heights
       NWAmes	Northwest Ames
       OldTown	Old Town
       SWISU	South & West of Iowa State University
       Sawyer	Sawyer
       SawyerW	Sawyer West
       Somerst	Somerset
       StoneBr	Stone Brook
       Timber	Timberland
       Veenker	Veenker
			
`Condition1`: Proximidade de várias condições
	
       Artery	Adjacente à uma via arterial (via de trânsito principal)
       Feedr	Adjacente à rua de alimentação (via secundária, geralmente conectada a ruas arteriais)	
       Norm	Normal	
       RRNn	A 200' da Ferrovia Norte-Sul
       RRAn	Adjacente à Ferrovia Norte-Sul
       PosN	Característica positiva próxima ao local: parque, greenbelt, etc.
       PosA	Adjacente a uma característica positiva externa
       RRNe	A 200' da Ferrovia Leste-Oeste
       RRAe	Adjacente à Ferrovia Leste-Oeste
	
`Condition2`: Proximidade de várias condições (se mais de uma estiver presente)
		
       Artery	Adjacente à rua arterial (via de trânsito principal)
       Feedr	Adjacente à rua de alimentação (via secundária, geralmente conectada a ruas arteriais)	
       Norm	Normal	
       RRNn	A 200' da Ferrovia Norte-Sul
       RRAn	Adjacente à Ferrovia Norte-Sul
       PosN	Característica positiva próxima ao local: parque, greenbelt, etc.
       PosA	Adjacente a uma característica positiva externa
       RRNe	A 200' da Ferrovia Leste-Oeste
       RRAe	Adjacente à Ferrovia Leste-Oeste
	
`BldgType`: Tipo de moradia
		
       1Fam	Moradia unifamiliar isolada	
       2FmCon	Conversão para duas famílias; originalmente construída como moradia unifamiliar
       Duplx	Duplex
       TwnhsE	Unidade final do sobrado
       TwnhsI	Moradia geminada dentro da unidade
	
`HouseStyle`: Estilo de moradia
	
       1Story	Um andar
       1.5Fin	Um andar e meio: 2º andar concluído
       1.5Unf	Um andar e meio: 2º nível inacabado
       2Story	Dois andares
       2.5Fin	Dois andares e meio: 2º andar concluído
       2.5Unf	Dois andares e meio: 2º andar inacabado
       SFoyer	Hall de entrada dividido
       SLvl	Split Level
	
`OverallQual`: Avalia o material geral e o acabamento da casa

       10	Muito excelente
       9	Excelente
       8	Muito Bom
       7	Bom
       6	Acima da média
       5	Média
       4	Abaixo da média
       3	Razoável
       2	Pobre
       1	Muito Pobre
	
`OverallCond`: Avalia o estado geral da casa

       10	Muito excelente
       9	Excelente
       8	Muito Bom
       7	Bom
       6	Acima da média
       5	Média
       4	Abaixo da média
       3	Razoável
       2	Pobre
       1	Muito Pobre
		
`YearBuilt`: Data de construção original

`YearRemodAdd`: Data da reforma (a mesma da construção, se não houver reforma ou acréscimos)

`RoofStyle`: Tipo de telhado

       Flat	Plano
       Gable	Telhado de duas águas (dois planos inclinados que se encontram em um ponto central, formando uma estrutura triangular).
       Gambrel	Telhado em estilo de celeiro ("barn roof") com dois planos inclinados em cada lado, sendo o inferior mais inclinado que o superior.
       Hip	Telhado em estilo "quatro águas", onde todos os lados do telhado são inclinados para baixo em direção às paredes.
       Mansard	Telhado em estilo Mansarda, caracterizado por dois planos inclinados em cada lado, sendo o inferior mais inclinado que o superior (comum em construções de estilo francês).
       Shed	Telhado de uma única água, com apenas uma inclinação.
		
`RoofMatl`: Material do telhado

       ClyTile	Argila ou Telha
       CompShg	Telha composta padrão
       Membran	Membrana
       Metal	Metal
       Roll	Telha em rolo
       Tar&Grv	Cascalho e Piche
       WdShake	Telha de madeira
       WdShngl	Telhas de madeira (semelhantes a WdShake, mas geralmente mais finas e uniformes)
		
`Exterior1st`: Revestimento externo da casa

       AsbShng	Telhas de amianto
       AsphShn	Telhas de asfalto
       BrkComm	Tijolo comum
       BrkFace	Tijolo decorativo
       CBlock	Cinder Bloco de concreto
       CemntBd	Painel de cimento
       HdBoard	Hard Board (placa de fibra prensada, geralmente usada como revestimento econômico)
       ImStucc	Estuque de imitação
       MetalSd	Revestimento de metal
       Other	Outros
       Plywood	Compensado
       PreCast	Pré-Moldado	
       Stone	PEdra
       Stucco	Estuque
       VinylSd	Revestimento de vinil
       Wd Sdng	Revestimento de madeira
       WdShing	Telhas de madeira
	
`Exterior2nd`: Revestimento externo da casa (se houver mais de um material)

       AsbShng	Telhas de amianto
       AsphShn	Telhas de asfalto
       BrkComm	Tijolo comum
       BrkFace	Tijolo decorativo
       CBlock	Cinder Bloco de concreto
       CemntBd	Painel de cimento
       HdBoard	Hard Board (placa de fibra prensada, geralmente usada como revestimento econômico)
       ImStucc	Estuque de imitação
       MetalSd	Revestimento de metal
       Other	Outros
       Plywood	Compensado
       PreCast	Pré-Moldado	
       Stone	Pedra
       Stucco	Estuque
       VinylSd	Revestimento de vinil
       Wd Sdng	Revestimento de madeira
       WdShing	Telhas de madeira
	
`MasVnrType`: Tipo de revestimento de alvenaria

       BrkCmn	Tijolo comum
       BrkFace	Tijolo decorativo
       CBlock	Cinder Bloco de cimento
       None	Nenhum
       Stone	Pedra
	
`MasVnrArea`: Área de revestimento de alvenaria em pés quadrados

`ExterQual`: Avalia a qualidade do material no exterior 
		
       Ex	Excelente
       Gd	Bom
       TA	Médio/Típico
       Fa	Razoável
       Po	Pobre
		
`ExterCond`: Avalia a condição atual do material no exterior
		
       Ex	Excelente
       Gd	Bom
       TA	Médio/Típico
       Fa	Razoável
       Po	Pobre
		
`Foundation`: Tipo de fundação
		
       BrkTil	Tijolo e Azulejo
       CBlock	Bloco de concreto
       PConc	Concreto derramado	
       Slab	Laje
       Stone	Pedra
       Wood	Madeira
		
`BsmtQual`: Avalia a altura do porão

       Ex	Excelente (100+ polegadas / mais de 2,54 metros)	
       Gd	Bom (90-99 polegadas / cerca de 2,28 a 2,52 metros)
       TA	Típico (80-89 polegadas / cerca de 2,03 a 2,26 metros)
       Fa	Razoável (70-79 polegadas / cerca de 1,78 a 2,01 metros)
       Po	Pobre (<70 polegadas / menos de 1,78 metros)
       NA	Sem porão
		
`BsmtCond`: Avalia o estado geral do porão

       Ex	Excelente
       Gd	Bom
       TA	Típico - umidade leve permitida
       Fa	Razoável - umidade ou algumas rachaduras ou sedimentação
       Po	Pobre - rachaduras severas, sedimentação ou umidade
       NA	Sem porão
	
`BsmtExposure`: Refere-se a muros de saída ou de nível de jardim

       Gd	Boa Exposição
       Av	Média de Exposição Média (níveis divididos ou foyers geralmente)
       Mn	Exposição Mínima
       No	Sem Exposição
       NA	Sem porão
	
`BsmtFinType1`: Classificação da área final do porão

       GLQ	Bom alojamento
       ALQ	Alojamento médio
       BLQ	Alojamento abaixo da média	
       Rec	Sala de recreação média
       LwQ	Sala de recreação média
       Unf	Inacabado
       NA	Sem porão
		
`BsmtFinSF1`: Tipo 1 pés quadrados acabados

`BsmtFinType2`: Classificação da área final do porão (se houver vários tipos)

       GLQ	Bom alojamento
       ALQ	Alojamento médio
       BLQ	Alojamento abaixo da média	
       Rec	Sala de recreação média
       LwQ	Sala de recreação média
       Unf	Inacabado
       NA	Sem porão

`BsmtFinSF2`: Tipo 2 pés quadrados acabados

`BsmtUnfSF`: Pés quadrados de área de porão inacabada

`TotalBsmtSF`: Total de pés quadrados de área do porão

`Heating`: Tipo de aquecimento
		
       Floor	Aquecedor embutido no piso
       GasA	Aquecedor a gás com ar quente forçado
       GasW	Aquecimento a gás com água quente ou vapor
       Grav	Aquecedor por gravidade ( Um sistema mais antigo que utiliza a gravidade para mover o ar quente para os ambientes sem ventiladores)	
       OthW	Aquecimento com água quente ou vapor, exceto gás
       Wall	Aquecedor de parede
		
`HeatingQC`: Qualidade e condição do aquecimento

       Ex	Excelente
       Gd	Bom
       TA	Médio/Típico
       Fa	Razoável
       Po	Pobre
		
`CentralAir`: Ar condicionado central

       N	Não
       Y	Sim
		
`Electrical`: Sistema elétrico

       SBrkr	Disjuntores padrão e fiação Romex
       FuseA	Caixa de fusíveis com mais de 60 AMP e toda a fiação Romex - Qualidade média	
       FuseF	Caixa de fusíveis de 60 AMP e principalmente fiação Romex - Qualidade razoável
       FuseP	Caixa de fusíveis de 60 AMP e principalmente fiação tipo "knob & tube" - Ruim
       Mix	Misto
		
`1stFlrSF`: Área do primeiro andar em pés quadrados
 
2ndFlrSF: Área do segundo andar em pés quadrados

LowQualFinSF: Área acabada de baixa qualidade em pés quadrados - todos os andares

GrLivArea: Área habitável acima do solo em pés quadrados

BsmtFullBath: Banheiros completos no porão

BsmtHalfBath: Lavabo no porão

FullBath: Banheiros completos acima do nível do solo

HalfBath: Lavabo acima do nível do solo

Bedroom: Quartos acima do nível do solo - não inclui quartos no porão

`KitchenAbvGr`: Cozinha acima do nível do solo

KitchenQual: Qualidade da Cozinha

       Ex	Excelente
       Gd	Bom
       TA	Médio/Típico
       Fa	Razoável
       Po	Pobre
       	
TotRmsAbvGrd: Total de cômodos acima do nível do solo (não inclui banheiros)

Functional: Funcionalidade geral da casa (assuma que é típico, a menos que deduções sejam garantidas)

       Typ	Funcionalidade típica
       Min1	Pequenas deduções nível 1
       Min2	Pequenas deduções nível 2
       Mod	Deduções moderadas
       Maj1	Grandes deduções nível 1
       Maj2	Grandes deduções nível 2
       Sev	Severamente danificado
       Sal	Somente para recuperação
		
Fireplaces: Número de lareiras

FireplaceQu: Qualidade da larerira

       Ex	Excelente - Lareira de alvenaria excepcional
       Gd	Bom - Lareira de alvenaria no andar principal
       TA	Média - Lareira pré-fabricada na área principal ou de alvenaria no porão
       Fa	Razoável - Lareira pré-fabricada no porão
       Po	Pobre - Fogão a lenha tipo "Ben Franklin"
       NA	Sem lareira
		
GarageType: Localização da garagem
		
       2Types	Mais de um tipo de garagem
       Attchd	Anexada à casa
       Basment	Garagem no porão
       BuiltIn	Integrada (Parte da casa, normalmente com cômodos acima da garagem)
       CarPort	Caramanchão
       Detchd	Separada da casa
       NA	Sem garagem
		
GarageYrBlt: Ano de construção da garagem
		
GarageFinish: Acabamento interno da garagem

       Fin	Acabada
       RFn	Acabamento simples	
       Unf	Inacabada
       NA	Sem garagem
		
GarageCars: Tamanho da garagem em capacidade de carros

GarageArea: Tamanho da garagem em pés quadrados

GarageQual: Qualidade da garagem

       Ex	Excelente
       Gd	Bom
       TA	Típico/Média
       Fa	Razoável
       Po	Pobre
       NA	Sem garagem
		
GarageCond: Condições da garagem

       Ex	Excelente
       Gd	Bom
       TA	Típico/Média
       Fa	Razoável
       Po	Pobre
       NA	Sem garagem
		
PavedDrive: Entrada pavimentada

       Y	Pavimentada 
       P	Pavimentação parcial
       N	Terra ou cascalho
		
WoodDeckSF: Área do deck de madeira em pés quadrados

OpenPorchSF: Área da varanda aberta em pés quadrados

EnclosedPorch: Área da varanda fechada em pés quadrados

3SsnPorch: Área da varanda para três estações em pés quadrados

ScreenPorch: Área da varanda telada em pés quadrados

PoolArea: Área da piscina em pés quadrados

PoolQC: Qualidade da piscina
		
       Ex	Excelente
       Gd	Bom
       TA	Média/Típico
       Fa	Razoável
       NA	Sem piscina
		
Fence: Qualidade da cerca

       GdPrv	Boa privacidade
       MnPrv	Privacidade mínima
       GdWo	Boa madeira
       MnWw	Madeira/arame mínimo
       NA	Sem cerca
	
MiscFeature: Característica adicional não coberta em outras categorias
		
       Elev	Elevador
       Gar2	Segunda garagem (se não descrita na seção garagem)
       Othr	Outros
       Shed	Galpão ou depósito (com mais de 100 pés quadrados)
       TenC	Quadra de tênis
       NA	Nenhum
		
MiscVal: $ Valor de características adicionais

MoSold: Mês da venda (MM)

YrSold: Ano da venda (YYYY)

SaleType: Tipo de venda
		
       WD 	Escritura de garantia - Convencional
       CWD	Escritura de garantia - Pagamento à vista
       VWD	Escritura de garantia - Financiamento VA (Venda financiada pelo programa de crédito para veteranos)
       New	Casa recém-construída e vendida
       COD	Escritura judicial ou venda por inventário
       Con	Contrato com 15% de entrada, termos regulares
       ConLw	Contrato com baixa entrada e baixa taxa de juros
       ConLI	Contrato com baixa taxa de juros
       ConLD	Contrato com baixa entrada
       Oth	Outro
		
SaleCondition: Condição da venda

       Normal	Venda normal
       Abnorml	Venda anormal -  Venda resultante de trocas, execução de hipotecas, ou venda a preços abaixo do mercado
       AdjLand	Compra de terreno adjacente
       Alloca	Alocação - Venda de duas propriedades interligadas, normalmente um condomínio e uma unidade de garagem	
       Family	Venda entre membros da família
       Partial	Casa não estava concluída na última avaliação (associada com Novas Casas)
