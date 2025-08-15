# Garbage Classification

Classificador de imagens de lixo utilizando transfer learning e um ensemble dos modelos MobileNetV2 e ResNet50.

## Pré-requisitos
- Python 3.8+
- Instalar dependências com `pip install -r requirements.txt`

## Dataset
O notebook utiliza `kagglehub` para baixar automaticamente o conjunto de dados. Defina a variável `DATASET_NAME` no início do notebook com o caminho do dataset no Kaggle.

## Uso
1. Instale as dependências: `pip install -r requirements.txt`
2. Execute o notebook `garbage_classification_annotated.ipynb`.
   - Ajuste `DATASET_NAME` se necessário.
   - O notebook realiza treinamento inicial e ajuste fino.
3. O modelo treinado é salvo como `waste_classifier_ensemble.keras`.

## Características
- Data augmentation para aumentar a diversidade dos dados
- Ensemble entre MobileNetV2 e ResNet50
- Fine-tuning com descongelamento parcial das redes base
- Pesos de classe para lidar com desbalanceamento
