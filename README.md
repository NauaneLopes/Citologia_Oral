# Projeto - Identificação Citologia Oral


#  Classificação de Células Citológicas Modelos de Aprendizado de Máquina


Este projeto tem como objetivo identificar células saudáveis (normais) e não saudáveis (anormais) em imagens citológicas por meio de redes neurais convolucionais (CNN). Foi desenvolvido como parte de uma pesquisa aplicada em visão computacional para diagnóstico assistido.

---

## Estrutura do Projeto

- **Preprocessamento** de imagens e segmentações
- **Extração de características morfológicas e texturais**
- ** Treinamento de modelos de árvores (Ex: RandomForest, DecisionTree)
- **Treinamento de modelos CNN** (Ex: EfficientNet, ResNet34)
- **Avaliação estatística** e visual (matriz de confusão, Grad-CAM)
- **Dashboard interativo** (Plotly / Dash)

---

##  Modelo Treinado

- Arquitetura: `ResNet34`
- Dados: 5 classes celulares, uso focado em *normal vs abnormal*
- Input: imagens em escala de cinza com segmentações
- Performance:
  - Acurácia | para abnormal: `97% ` para normal: `91% `
  - F1-score | para abnormal: `97% ` para normal: `92%`
  - Precisão | para abnormal: `97%` para normal: `91%`
  - Recall   | para abnormal: `96%` para normal: `93%`
  - AUC ROC: 0.98

- Foram aplicados outras arquiteturas, como EfficientNet (B2, B3 e B7); ResNet50; VGG16, DecisionTree; RandomForestClassifier; GradientBoosting e XGBostClassifier. Que podem ser visualizados no arquivo [MODELOS_APLICADOS_CNN.ipynb](./MODELOS_APLICADOS_CNN.ipynb) e [Modelos_Árvores.ipynb](./Modelos_Árvores.ipynb). Esses modelos apresentaram resultados similares, para as métricas avaliadas no modelo ResNet34, com valores iguais ou superior a 89% para as classes Normal e Abnormal.

## RESULTADOS

ACURÁCIA: [accuracy.png](./accuracy.png)
LOSS: [loss.png](./loss.png)
MATRIZ DE CONFUSÃO: [mc.png](./mc.png)
CURVA PRECISÃO RECALL: [pr.png](./pr.png)
CURVA ROC: [roc.png](./roc.png)
---

##  Dataset

- Fonte: Mendeley Data - Citologia esfoliativa oral <https://data.mendeley.com/datasets/dr7ydy9xbk/2>
- Ou Imagens já pré processadas - <https://drive.google.com/drive/folders/10vCpH-FHLrCuGJeGUv35oHLer2AuQiQR?usp=sharing> para modelos CNN. 
- Formato: imagens 224x224
- Organização: `train`, `val`, `test`

## Dashboard

Pode ser visualizado nesse arquivo [RELATÓRIO_DASH_RN34.ipynb](./RELATÓRIO_DASH_RN34.ipynb)
> Devido a direitos de uso, os dados não estão incluídos. Veja o [README](./README.md) para instruções de acesso.

---
## Aviso
Os modelos aplicados estão disponíveis na biblioteca keras, foram aplicados conforme apresentado na documentação.
Link Keras: <https://keras.io/api/applications/>
Link PyTorch: <https://docs.pytorch.org/vision/main/models.html>


