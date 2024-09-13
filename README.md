# Detecção de Fraude em Transações com Cartão de Crédito

## Descrição do Projeto
Este projeto visa detectar fraudes em transações com cartão de crédito utilizando algoritmos de machine learning. O conjunto de dados contém 284.807 transações realizadas ao longo de dois dias, das quais 492 são fraudes. Dada a natureza desbalanceada do dataset, a métrica AUPRC (Area Under the Precision-Recall Curve) foi escolhida para avaliar o desempenho dos modelos, por ser mais apropriada do que a acurácia em situações de desbalanceamento severo.

## Modelos Utilizados
Foram implementados e comparados os seguintes modelos de classificação:
<ul>
  <li><b>Random Forest</b></li>
  <li><b>XGBoost</b></li>
  <li><b>Regressão Logística</b></li>
  <li><b>K-Nearest Neighbors (KNN)</b></li>
  <li><b>Árvore de Decisão</b></li>
</ul>
  
## Avaliação e Resultados
Os modelos foram avaliados utilizando a métrica AUPRC. Após a comparação, o XGBoost apresentou o melhor desempenho, com uma AUPRC de 0,775, superando os outros modelos e sendo a escolha mais adequada para este problema de detecção de fraude.

## Métricas de Desempenho dos Modelos:
| Modelo              | AUPRC  | Precisão  | Recall    | F1-Score  | Acurácia   |
|---------------------|--------|-----------|-----------|-----------|------------|
| Random Forest        | 0.7607 | 0.9402    | 0.8088    | 0.8696    | 0.9996     |
| XGBoost              | 0.7754 | 0.9412    | 0.8235    | 0.8784    | 0.9996     |
| Regressão Logística  | 0.3991 | 0.8333    | 0.4779    | 0.6075    | 0.9990     |
| KNN                  | 0.7022 | 0.9358    | 0.7500    | 0.8327    | 0.9995     |
| Árvore de Decisão    | 0.7607 | 0.9402    | 0.8088    | 0.8696    | 0.9996     |

## Tecnologias Utilizadas
<ul>
  <li><b>Python</b></li>
  <li><b>NumPy</b></li>
  <li><b>Pandas</b></li>
  <li><b>Scikit-learn</b></li>
</ul>

## Conclusão
Este projeto demonstrou a importância de testar diferentes algoritmos de machine learning para encontrar a melhor solução. O XGBoost se destacou por sua performance em comparação com Random Forest, Regressão Logística, KNN e Árvore de Decisão.
