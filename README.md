# CP1_Front_and_Mobile

# Aprimoramento de Modelos de Classificação para o Case Ifood (Checkpoint #1)

Este repositório contém o desenvolvimento e os resultados do primeiro checkpoint para a disciplina de [Nome da Disciplina], com foco no aprimoramento de modelos de classificação para o dataset do Case Ifood, conforme apresentado em aula.

O objetivo principal deste trabalho foi explorar diferentes algoritmos de classificação e otimizar seus hiperparâmetros, utilizando a biblioteca PyCaret, com a métrica AUC (Area Under the ROC Curve) como principal referência de desempenho. Buscamos alcançar valores de AUC superiores aos obtidos nos notebooks de aula para o conjunto de teste (representado em nosso código como `df_valid`).

A abordagem adotada envolveu a experimentação com diversos modelos, incluindo:

* **Random Forest (`rf`):** Criamos e otimizamos um modelo Random Forest como ponto de partida e referência.
* **Análise Discriminante Linear (`lda`):** Exploramos o modelo LDA, ajustando seus hiperparâmetros com uma validação cruzada robusta e foco na otimização do AUC.
* **Regressão Ridge (`ridge`):** Investigamos o desempenho da Regressão Ridge em um contexto de classificação, otimizando-a para a métrica de interesse.
* **LightGBM (`lightgbm`):** Testamos e otimizamos o modelo LightGBM, conhecido por sua eficiência e capacidade de alcançar alto desempenho em tarefas de classificação.
* **XGBoost (`xgboost`):** De forma similar, o modelo XGBoost foi incluído na experimentação, passando por um processo de otimização de hiperparâmetros direcionado ao AUC.

Os códigos presentes neste repositório demonstram o processo de criação, otimização (tuning) e avaliação desses modelos utilizando as funcionalidades do PyCaret. Os outputs das etapas de treinamento e otimização, incluindo os valores de AUC obtidos durante a validação cruzada, estão devidamente comentados no notebook.

A análise comparativa dos resultados obtidos indica que [**Aqui você deverá inserir uma breve conclusão sobre qual modelo ou modelos se destacaram em relação ao Random Forest em termos de AUC durante a validação e/ou avaliação no conjunto `df_valid`. Mencione se algum modelo consistentemente superou o Random Forest.**].

Este trabalho representa a primeira etapa na busca por um modelo de classificação aprimorado para o Case Ifood, com foco na otimização da capacidade de discriminação entre as classes, medida pelo AUC.

**Integrantes do Grupo:**

* Pablo Menezes Barreto
* Matheus Hungaro Fidelis
