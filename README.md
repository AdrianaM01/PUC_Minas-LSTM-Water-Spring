# PUC_Minas-LSTM-Water-Spring

## A preservação do “ouro azul”

No início de dezembro de 2020 a Acea Group, um dos líderes de distribuição de água, gás e energia da Itália, publicou em uma das maiores comunidades de data science, o Kaggle, uma competição para encontrar meios eficientes de prever a disponibilidade de água dos recursos hídricos administrados por ela.

De acordo com a Acea Group (2020), há uma grande necessidade de prever a disponibilidade do nível de água dos recursos hídricos (nascentes, rios, lagos ou aquíferos) para que seja possível garantir o consumo diário e, principalmente, preservar esses recursos naturais.

De toda água disponível no planeta, apenas 2,5% corresponde a água doce. No entanto, aproximadamente 68,7% do total de água doce encontra-se em locais de difícil acesso como a Antártica ou picos gelados e 30,3% em subsolos, rios, pântanos etc. Portanto, menos de 1% restante é água doce de fácil acesso para o ser humano (RIBEIRO, 2008).

Dessa forma, somando esse cenário aos problemas ambientais que se agravam ao longo dos anos, torna-se cada vez mais necessária a preocupação na preservação do “ouro azul”, principalmente pelas companhias distribuidoras de água que estão diretamente ligadas ao gerenciamento do uso desses recursos.]

## Prevendo a vazão de nascentes 

A Acea Group disponibilizou no site Kaggle, diversos datasets relacionados aos seus principais recursos hídricos (nascentes, rios, lagos e aquíferos) (KAGGLE, 2020). Para o estudo proposto, serão utilizados os dados das nascentes de Amiata.

Amiata refere-se ao Monte Amiata, um antigo vulcão extinto que fica na região de Toscana, Itália, possuindo 1.738 metros de altura e bastante caracterizado por suas nascentes que formam rios e lagos na região (DISCOVER TUSCANY, 2015?).

Cada recurso hídrico possui um alvo diferente para predição. Para as nascentes, o objetivo é prever a vazão da nascente em um período futuro. O estudo da vazão de uma nascente apoia na caracterização do seu regime hidrológico, que pode sofrer influência do índice pluviométrico, localização e também por ações do homem. (ARAÚJO FILHO, et al., 2011 apud SIMEDO; MARTINS; LOPES, 2015)

Dessa forma, cada nascente possui um dataset único e com atributos distintos que podem influenciar o resultado da vazão de forma distinta. Para o estudo proposto, o algoritmo terá como objetivo prever a vazão do próximo mês. Para o treinamento do modelo, serão avaliados todos os dados históricos disponibilizados pela Acea Group. Portanto, dados desde 2000.

## Redes Neurais Recorrentes — LSTM

O estudo proposto tem como objetivo prever como será a vazão das nascentes de Amiata no mês seguinte com base nos dados históricos. Para isso, decidiu-se desenvolver um modelo de rede neural recorrente LSTM (Long short-term memory) que deverá considerar multivariáveis para prever uma saída única. Isso significa que será considerado histórico dos atributos de Rainfall, Temperature e Depth to Groundwater para prever a vazão da nascente, o Flow Rate.

A definição desse modelo foi feita com base no estudo compartilhado por Bielinskas (2020), no qual o autor utilizou LSTM e múltiplas variáveis para predição de valores de ações.

## Referências

ACEA GROUP. **Acea Smart Water Analytics**. Kaggle, 10 dez. 2020. Disponível em: https://www.kaggle.com/c/acea-water-prediction. Acesso em: 28 dez. 2020.

RIBEIRO, W. C. **Geografia Política da Água**. São Paulo: Editora Annablume, 2008.

KAGGLE. **Acea Smart Water Analytics Data**. Kaggle, 10 dez. 2020. Disponível em: https://www.kaggle.com/c/acea-water-prediction/data. Acesso em: 28 dez. 2020.

DISCOVER TUSCANY. **Monte Amiata dominates over the Val d'Orcia**. Website Discovery Tuscany, [2015?]. Disponível em: https://www.discovertuscany.com/what-to-do-in-tuscany/monte-amiata.html. Acesso em: 31 jan 2021.

SIMEDO, M. B. L.; MARTINS, A. L. M.; LOPES, M. C. **O Monitoramento Da Vazão Como Ferramenta Para O Plano De Gestão Ambiental Em Microbacias Hidrográficas**. Periódico Eletrônico Fórum Ambiental da Alta Paulista, [S.l.], v. 11, n. 6, dez. 2015.

**Multivariate Time Series Prediction with LSTM and Multiple features (Predict Google Stock Price)**. Tutorial feito por Vytautas Bielinskas. [S. l.: s. n.], 2020. 1 vídeo (20 min). Disponível em: https://www.youtube.com/watch?v=gSYiKKoREFI&. Acesso em: 10 jan 2010.
