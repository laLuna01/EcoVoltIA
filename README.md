# EcoVoltIA
O projeto visa desenvolver uma solução de Machine Learning capaz de prever a geração de energia em comunidades remotas que dependem de fontes renováveis, como solar e eólica, com base em condições climáticas diárias. Essas comunidades frequentemente enfrentam dificuldades no acesso à energia confiável devido à variabilidade climática e à imprevisibilidade da demanda. A solução proposta busca mitigar esses desafios, fornecendo previsões precisas que permitem um melhor planejamento e gestão dos recursos energéticos disponíveis.

Este projeto tem potencial para ser implementado em soluções reais de monitoramento e gestão de energia, contribuindo para um futuro mais sustentável e seguro para as comunidades que dependem de energia renovável.

## Dados Utilizados
<b>Fonte dos Dados:</b> Os dados meteorológicos foram obtidos da API NASA POWER, que fornece informações climáticas históricas.

<b>Tamanho do Conjunto de Dados:</b> 600 registros de dados diários.

<b>Formato dos Dados:</b> Arquivo CSV com os dados limpos.

### Variáveis Utilizadas:
- <b>Área do Painel Solar (m²):</b> area_painel_m2
- <b>Radiação Solar Média (kWh/m²/dia):</b> radiacao_solar_media_kwh_m2_dia
- <b>Temperatura (°C):</b> temperatura_c
- <b>Cobertura de Nuvens (%):</b> cobertura_nuvens_percentual
- <b>Velocidade do Vento (m/s):</b> velocidade_vento_m_s
- <b>Energia Gerada (kWh/dia):</b> energia_gerada_kwh_dia (Target)

## Bibliotecas Utilizadas
- <b>requests</b> - Para acessar a API e recuperar os dados.
- <b>numpy</b> - Para operações matemáticas.
- <b>pandas</b> - Para manipulação de dados.
- <b>sklearn (Scikit-learn)</b> - Para construção e avaliação do modelo de Machine Learning.
- <b>matplotlib e seaborn</b> - Para visualização de dados.

## Modelo Utilizado
<b>Algoritmo:</b> RandomForestRegressor - Um modelo de aprendizado supervisionado que cria múltiplas árvores de decisão e combina seus resultados para melhorar a precisão da previsão.

<b>Divisão de Dados:</b> 80% dos dados para treino e 20% para teste.

## Resultados Obtidos
### Mean Squared Error (MSE): 44319.32
- Mede a média dos quadrados dos erros, sendo um indicativo da magnitude dos erros na previsão. Um valor mais baixo indica previsões mais precisas.
  
### Erro Médio Absoluto Percentual (MAPE): 10.83%
- Mede a precisão das previsões em termos percentuais. No caso, as previsões do modelo têm, em média, um erro de 10.83% em relação ao valor real.
  
### Precisão Média (Acurácia de Previsão): 89.17%
- O modelo é capaz de prever com uma precisão média de 89.17% os valores de geração de energia com base nas condições climáticas fornecidas.

## Alunos
<b>Luana Sousa Matos:</b> RM552621

<b>Nicolas Martins:</b> RM553478
