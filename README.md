# Desafio de Previsão de Gastos em Saúde
<img src="https://auxomedical.com/wp-content/uploads/2020/12/levo-health-why-is-healthcare-marketing-important-1-1200x801-1-1110x624.jpg" alt="Gastos Saúde" width="500" />

# Visão Geral
Nesse projeto, voltado para estudo, vamos sugerir soluções para um desafio de previsão que tem como objetivo prever gastos em cuidados em saúde a partir de características sociodemográficas de um grupo de pacientes. O desafio original pode ser encontrado no link [FreeCodeCamp](https://www.freecodecamp.org/learn/machine-learning-with-python/machine-learning-with-python-projects/linear-regression-health-costs-calculator)

# Problema e Solução
Além da importancia de projetar gastos na área da saúde a capacidade de prever gastos também pode abordar outro ponto muito importante para o tema, a identificação de quais fatores podem influenciar nesse resultado, poís além de entender a influencia de cada característica nos gastos podemos também evidenciar quais características ou hábitos podem ser alterados ou trabalhados para diminuir esses gastos.

Esse conhecimento pode direcionar melhor as decisões e conscientizar pacientes sobre hábitos nocivos a sua própria saúde, fazendo a tomada de decisão em saúde de uma melhor forma. Além disso campanhas de conscientização podem ser elaboradas com maior eficácia por parte de instituições e órgãos públicos de saúde.

Para esse desafio foi proposto o uso de modelo de regressão linear para encontrar um modelo que consiga prever os gastos com Erro Absoluto Médio (Mean Absolute Erros - MAE) abaixo de $3500.

Também vamos tentar responder as seguintes perguntas:<br>
<br>
1.Hábitos saudáveis influenciam nos gastos em saúde?<br>
2.Quais hábitos poderiam ser mudados para diminuir gastos e promover melhor saúde?<br>
<br>

# Processo
A solução básica seguirá as seguintes etapas:<br>
1.Investigação inicial do conjunto de dados<br>
2.Análise descritiva<br>
3.Pré-processamento dos dados<br>
4.Construção do modelo<br>
5.Métricas do modelo<br>

Iremos também adicionar algumas etapas nesse estudos utilizando:
- [Auto EDA](https://github.com/Bruno-Donato/desafio_gastos_saude/blob/main/eda_autom.ipynb)
- [Seleção de variáveis com Boruta](https://github.com/Bruno-Donato/desafio_gastos_saude/blob/main/selecao_variaveis.ipynb)
- [Modelos mais complexos e robustos, e construção de rede neural com Keras/TensorFlow](https://github.com/Bruno-Donato/desafio_gastos_saude/blob/main/previsao_gastos_saude.ipynb)
- [Explicando modelos complexos com LIME e SHAP](https://github.com/Bruno-Donato/desafio_gastos_saude/blob/main/explicando_modelos_complexos.ipynb)
- [Previsão e otimização utilizando PyCaret (AutoML)](https://github.com/Bruno-Donato/desafio_gastos_saude/blob/main/pycaret_teste.ipynb)

# Resultados
- As variáveis IMC, idade e tabagismo contribuem de maneira relevante para a performance do modelo de regressão
- Modelo de regressão linear básico não foi capaz de prever os gastos com MAE abaixo do valor estipulado no desafio
- O modelo de regresão com transformação polinomial teve uma performance aceitável para o desafio
- Modelos mais complexos e robustos obtiveram resultados com valores significativamente abaixo do valor estipulado

# Conclusão
Características como tabagismo, idade e IMC parecem ser fatores importantes para prever gastos em saúde, e utilizando um modelo de regressão linear com função polinomial de grau II podemos prever os gastos em saúde com MAE abaixo de $3500 estipulado pelo desafio. Podemos prever com menor MAE utilizando modelos mais complexos e robustos, porém a princípio devemos priorizar modelos mais simples, pois além de serem menos custosos computacionalmente eles também tem uma característica muito importante para a tomada de decisão que é a explicabilidade, o que torna os insights gerados pelos dados muito mais fáceis de serem compreendidos e serem transformados em ações.
