# Transfer Learning Project with Python
 - Transferindo conhecimento com rede neural pré treinada de reconhecimento de imagens.
 - Utilizando o modelo Xception pré treinada com o dataset ImageNet.
 - Utilizando o dataset cats_vs_dogs (Kaggle).

# Fluxo de trabalho do transfer learning
1. Instanciando um modelo_base e carregando pesos pré-treinados nele.

    O argumento **_weights="imagenet"_** podemos carregar os pesos pré treinados na ImageNet dataset.

2. Congelando todas as camadas no modelo_base configurando _**modelo_base.trainable = False**_.    
3. Criando um novo modelo sobre a saída de uma (ou várias) camadas do modelo_base.
4. Treinando seu novo modelo em seu novo conjunto de dados.

# Afinando o modelo
Após treinar seu modelo com novos dados, podemos descongelar o modelo_base utilizando **_modelo_base.trainable = True_** e treinar novamente do inicio ao fim com uma baixa taxa de aprendizado.


# Referências e Links importantes
### KERAS - Transfer Learning
https://keras.io/guides/transfer_learning/

### KERAS - Criando novas camadas e modelos por meio de subclasses
https://keras.io/guides/making_new_layers_and_models_via_subclassing/

### KAGGLE - cats_vs_dogs dataset download
https://www.kaggle.com/competitions/dogs-vs-cats/data

[![Cats Vs Dogs](https://media.tenor.com/PFFw6tqLS_wAAAAC/cat-force-catisyourfather.gif "Cats Vs Dogs")](https://tenor.com/view/cat-force-catisyourfather-cat-vs-dog-gif-12806997)
