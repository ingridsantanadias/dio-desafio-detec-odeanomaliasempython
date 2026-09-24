# Detecção de Fraude em Cartão de Crédito 

Projeto de Machine Learning para identificar transações fraudulentas em uma base altamente desbalanceada.

##  O Problema
Apenas **0,17%** das transações da base são fraudes. Por isso, a **acurácia não serve**: um modelo que diz "não é fraude" para tudo acertaria 99,8% das vezes, mas falharia em todas as fraudes. O foco aqui foi maximizar o **Recall** (capturar o máximo de fraudes possíveis).

##  O que foi feito
1. **Preparação:** Limpeza, transformação logarítmica no valor (`Amount`) e divisão estratificada dos dados.
2. **Modelagem:** Teste com Regressão Logística (Baseline), Random Forest e XGBoost, usando pesos balanceados para lidar com a raridade das fraudes.
3. **Avaliação:** Uso de Curva Precision-Recall e ajuste de limiar (*threshold*) para encontrar o ponto ideal de detecção.
4. **Explicabilidade:** Uso do SHAP para entender quais variáveis mais pesaram nas decisões do modelo.

##  Como executar
Abra o notebook no Google Colab, carregue o dataset e execute as células do início ao fim.
