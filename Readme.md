# AI aplicado a Meteorología

Este repositorio contiene los notebooks y material a desarrollar durante el taller “APRENDIZAJE AUTOMÁTICO E INTELIGENCIA ARTIFICIAL APLICADOS A LA METEOROLOGÍA" organizado por el Servicio Nacional de Meteorología e Hidrología del Perú (SENAMHI).

Los notebooks se han diseñado para ser ejecutados en Google Colab, una plataforma gratuita que permite ejecutar código Python en la nube. Para ejecutar los notebooks, se debe hacer clic en el botón `Open in Colab` que aparece al inicio de cada notebook o en la siguiente lista.

1. **Introducción a la Inteligencia Artificial** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/griverat/Meteo-AI/blob/main/notebooks/1.intro.ipynb)

2. **Deep Learning con redes convolucionales** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/griverat/Meteo-AI/blob/main/notebooks/2.cnn_datos.ipynb)

3. **Regularización en Machine Learning** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/griverat/Meteo-AI/blob/main/notebooks/3.regularization.ipynb)

4. **Redes Neuronales Recurrentes (RNN)** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/griverat/Meteo-AI/blob/main/notebooks/4.rnn_datos.ipynb)

5. **AI para generación de datos 2D** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/griverat/Meteo-AI/blob/main/notebooks/5.gen_ai.ipynb)

## Uso de manera local

Si desea usar los notebooks de manera local, ya sea usando Jupyter Notebook, Juptyer Lab o Visual Studio Code, puede clonar este repositorio usando el siguiente comando (requiere tener instalado git):

```bash
git clone https://github.com/griverat/Meteo-AI.git
cd Meteo-AI
```

o bien, [descargar el repositorio como un archivo ZIP](https://github.com/griverat/Meteo-AI/archive/refs/heads/main.zip) y descomprimirlo en su computadora.

Adicionalmente, debe tener instalado [Miniconda](https://docs.anaconda.com/miniconda/miniconda-install/) o [Miniforge](https://github.com/conda-forge/miniforge?tab=readme-ov-file) (recomendado, seleccionar la descarga en la tabla de Miniforge3 para su sistema operativo) para tener acceso al comando `conda` o `mamba`, los cuales permiten crear y gestionar entornos virtuales de Python.

Una vez se encuentre dentro de la carpeta del repositorio, ejecutar el siguiente comando para instalar las librerías necesarias:

```bash
# en caso de usar mamba
mamba env create -f environment.yml
```
o
```bash
# en caso de usar conda
conda env create -f environment.yml
```

Finalmente, activar el entorno y ejecutar Jupyter Notebook, Jupyter Lab o Visual Studio Code (escoger solo uno):
    
```bash
conda activate meteo-ai

# para abrir jupyter notebook
jupyter notebook

# para abrir jupyter lab
jupyter lab

# para abrir visual studio code
code .
```

Tener en cuenta que el entorno provisto contienen versiones minimas de los paquetes `Tensorflow` y `Pytorch` para poder ejecutar los notebooks usando CPU. Si desea usar GPU, se recomienda seguir las instrucciones de instalación de las respectivas páginas oficiales de [Tensorflow](https://www.tensorflow.org/install) y [Pytorch](https://pytorch.org/get-started/locally/).

Recordar que para usar las versiones de GPU de las librerías, se debe tener una tarjeta gráfica instalada en su equipo (dispositivo físico) que sea compatible con CUDA y cuDNN (usualmente tarjetas gráficas NVIDIA).