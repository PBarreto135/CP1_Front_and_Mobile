# CP1_Front_and_Mobile

# Aprimoramento de Modelos de Classificação para o Case Ifood (Checkpoint #1)

Este repositório contém o desenvolvimento e os resultados do primeiro checkpoint para a disciplina de Front and Mobile, com foco no aprimoramento de modelos de classificação para o dataset do Case Ifood, conforme apresentado em aula.

O objetivo principal deste trabalho foi explorar diferentes algoritmos de classificação e otimizar seus hiperparâmetros, utilizando a biblioteca PyCaret, com a métrica AUC (Area Under the ROC Curve) como principal referência de desempenho. Buscamos alcançar valores de AUC superiores aos obtidos nos notebooks de aula para o conjunto de teste (representado em nosso código como `df_valid`).

A abordagem adotada envolveu a experimentação com diversos modelos, incluindo:

* **Random Forest Classifier:** Modelo base para comparação.
* **Linear Discriminant Analysis:** Um modelo linear testado para avaliar seu desempenho.
* **Ridge Classifier:** Outro modelo linear explorado no contexto da classificação.
* **Light Gradient Boosting Machine:** Um algoritmo de boosting conhecido por sua eficiência e performance.
* **Extreme Gradient Boosting:** Outro algoritmo de boosting poderoso amplamente utilizado.

A tabela abaixo resume o desempenho dos modelos avaliados no conjunto de validação (os valores para o Random Forest são antes da otimização, para fornecer um ponto de referência inicial):

| Modelo                         | Accuracy | AUC    | Recall | Precision | F1     | Kappa  | MCC    |
| :----------------------------- | :------- | :----- | :----- | :-------- | :----- | :----- | :----- |
| Random Forest Classifier       | 0.8636   | 0.8270 | 0.1429 | 0.4000    | 0.2105 | 0.1538 | 0.1786 |
| Linear Discriminant Analysis | 0.7455   | 0.8181 | 0.7857 | 0.3056    | 0.4400 | 0.3143 | 0.3731 |
| Ridge Classifier               | 0.7455   | 0.7626 | 0.7857 | 0.3056    | 0.4400 | 0.3143 | 0.3731 |
| Light Gradient Boosting Machine| 0.8364   | 0.8144 | 0.3571 | 0.3571    | 0.3571 | 0.2634 | 0.2634 |
| Extreme Gradient Boosting      | 0.8000   | 0.8263 | 0.8571 | 0.3750    | 0.5217 | 0.4188 | 0.4761 |

A análise comparativa dos resultados obtidos indica que, embora o Random Forest apresente uma alta acurácia, outros modelos como o **Linear Discriminant Analysis** e o **Extreme Gradient Boosting** demonstraram valores de AUC comparáveis ou ligeiramente inferiores ao Random Forest inicial, mas com um Recall significativamente maior. O **Ridge Classifier** apresentou um AUC inferior aos demais. O **Light Gradient Boosting Machine** mostrou um AUC também ligeiramente inferior ao Random Forest inicial neste estágio. A otimização dos hiperparâmetros (tuning), conforme demonstrado nos códigos, buscou melhorar o AUC desses modelos, e os resultados finais dessa otimização devem ser considerados para uma conclusão definitiva sobre qual modelo se destaca.

Este trabalho representa a primeira etapa na busca por um modelo de classificação aprimorado para o Case Ifood, com foco na otimização da capacidade de discriminação entre as classes, medida pelo AUC.
**Integrantes do Grupo:**

* **Nome:** Pablo Menezes Barreto **RM:** 556389
* **Nome:** Matheus Hungaro Fidelis **RM:** 555677
