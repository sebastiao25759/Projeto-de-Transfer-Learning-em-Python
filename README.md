Aqui está uma descrição para o seu projeto no GitHub:

---

# Classificação de Gatos e Cachorros com Transfer Learning

Este projeto utiliza **Transfer Learning** para classificar imagens de gatos e cachorros em um modelo de aprendizado profundo. O modelo foi desenvolvido usando o **MobileNetV2**, um modelo pré-treinado, e adaptado para a tarefa de classificação binária entre as duas classes: gato e cachorro.

## Funcionalidades
- **Pré-processamento de Dados**: Utiliza o `ImageDataGenerator` para carregar e aumentar o conjunto de dados de imagens de gatos e cachorros.
- **Modelo Base**: A base do modelo é o **MobileNetV2**, que foi treinado previamente com a base de dados ImageNet. Este modelo é congelado e apenas camadas adicionais são treinadas.
- **Camadas Adicionais**: Camadas densas foram adicionadas para personalizar o modelo para a classificação binária de gatos e cachorros.
- **Avaliação**: O modelo é treinado e avaliado usando conjuntos de dados de treino e validação, sendo capaz de classificar imagens de novas amostras (gatos ou cachorros).

## Estrutura do Código
1. **Preparação dos Dados**: O código prepara os dados para o treinamento, incluindo aumento de dados (data augmentation) e normalização das imagens.
2. **Transfer Learning**: Utiliza o MobileNetV2 como modelo base e adiciona camadas de rede neural totalmente conectadas para classificação binária.
3. **Treinamento do Modelo**: O modelo é compilado e treinado usando a função de perda `binary_crossentropy` e a métrica de `accuracy`.
4. **Classificação de Imagens**: O modelo treinado pode ser utilizado para classificar imagens de gatos e cachorros, mostrando o resultado da previsão.

## Requisitos
- **Python 3.x**
- **TensorFlow 2.x**
- **Keras**
- **NumPy**
- **Matplotlib**

## Como Usar
1. Substitua o caminho do diretório do conjunto de dados (`data_dir`) com o diretório onde estão as imagens de treino e validação.
2. Substitua o caminho da imagem de teste (`image_path`) para testar o modelo com uma imagem nova.

### Exemplo de Teste
```python
image_path = "path_to_test_image"
predict_image(image_path)
```

Este projeto é ideal para quem deseja aprender sobre **Transfer Learning** e como implementar modelos de classificação de imagens usando redes neurais profundas.

### Comando para clonar o diretorio
```
git clone https://github.com/sebastiao25759/Projeto-de-Transfer-Learning-em-Python.git
```
