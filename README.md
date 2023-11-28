# Projeto de Iniciação Científica Pinus Taeda
Este projeto tem como objetivo monitorar o avanço de Pinus Taeda na região de Ponta Grossa por meio de imagens de sensoriamento remoto, utilizando Machine Learning.

## Requerimentos para utilização dos notebooks
Primeiramente, é recomendável criar um "virtual enviroment" para instalar as bibliotecas necessárias e não ter conflito com suas bibliotecas já instaladas no seu sistema.
### Criando um "virtual enviroment" no vscode
Utilize os comandos abaixo no terminal:
* python -m venv .venv
* source /caminho/para/pasta/.venv/criada/
* pip install -r requirements.txt
## Funcionamento de cada algoritmo
São dois algoritmos:
### convert_dataset
* Utilizar este primeiramente para converter os "shapes" criados no QGIS ou ArcGIS para imagens .tif únicas;
* O "shapefile" deve conter o mesmo formato de mapa dos "rasters";
* Alterar no algoritmo os diretórios para as pastas do seu sistema.
### cnn
* Utilizar posteriormente para criação de diretórios de treino e teste contendo as imagens .tif;
* Pro algoritmo reconhecer as classes, é necessário que existam duas pastas separadas para cada classes dentro do diretório de treino e teste, exemplo: 
- train_folder
    - class_1_folder (e.g., pinus)
        - image1.tif
        - image2.tif
        ...
    - class_2_folder (e.g., non_pinus)
        - image1.tif
        - image2.tif
        ...
- test_folder
    - class_1_folder (e.g., pinus)
        - image1.tif
        - image2.tif
        ...
    - class_2_folder (e.g., non_pinus)
        - image1.tif
        - image2.tif
        ...
* Alterar no algoritmo os diretórios para as pastas do seu sistema;
* Algoritmo CNN ML de rede neural para teste do dataset;
* Alterar no algoritmo os diretórios para as pastas do seu sistema.
