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

- Arquitetura: ``
- Dados: 5 classes celulares, uso focado em *normal vs abnormal*
- Input: imagens em escala de cinza com segmentações
- Performance:
  - Acurácia | para abnormal: ` ` para normal: ` `
  - F1-score | para abnormal: ` ` para normal: ` `
  - Precisão | para abnormal: ` ` para normal: ` `
  - Recall   | para abnormal: ` ` para normal: ` `
  - AUC ROC: 

---

Resultados
 Matriz de Confusão | Curva ROC |Erro de Treinamento e Validação | Acurácia de Treinamento e Validação | Gráfico Precisão e Recall
|--------------------|
'![Confusao]() |'
'![AUC ROC]()  |'
'![Erro_tv]()  |'
'![Ac tv  ]()  |'
'![Prec pr]()  |'
---


##  Dataset

- Fonte: Mendeley Data - Citologia esfoliativa oral <https://data.mendeley.com/datasets/dr7ydy9xbk/2>
- Ou Imagens já pré processadas - <https://drive.google.com/drive/folders/10vCpH-FHLrCuGJeGUv35oHLer2AuQiQR?usp=sharing> para modelos CNN. 
- Formato: imagens 224x224
- Organização: `train`, `val`, `test`

> Devido a direitos de uso, os dados não estão incluídos. Veja o [README na pasta data](./data/README.md) para instruções de acesso.

---

## Como Executar

1. Clone o repositório:
```bash
git clone https://https://github.com/NauaneLopes/Citologia_Oral.git
