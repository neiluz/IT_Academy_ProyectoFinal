[![twitter](https://github.com/neiluz/IT_Academy_ProyectoFinal/blob/main/twitter.png)](https://www.github.com/)  


## IT_Academy_ProyectoFinal
# Descifrando el lenguaje emocional en Twitter: Un análisis predictivo basado en aprendizaje automático
[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)  
[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)

### Descripción:
En la era actual de las redes sociales, Twitter se ha convertido en una de las plataformas más utilizadas en todo el mundo, donde millones de usuarios publican diariamente sus pensamientos, emociones y experiencias. Esta enorme cantidad de datos proporciona una fuente rica de información para analizar las tendencias y patrones de los usuarios. 

La detección de emociones a partir de textos es uno de los desafíos más complejos en el procesamiento del lenguaje natural debido a la naturaleza multiclase del problema y la falta de conjuntos de datos etiquetados. Sin embargo, en este estudio se cuenta con un conjunto de datos ya etiquetado para la detección de emociones en tweets. En este contexto, el objetivo de este estudio es desarrollar un modelo que permita detectar emociones en los tweets con el fin de ayudar en la detección temprana de trastornos emocionales, como la depresión y la ansiedad. Al lograr este objetivo, se puede proporcionar información valiosa para los profesionales de la salud mental y ayudar en la toma de decisiones clínicas tempranas.

Para alcanzar el objetivo, se utilizará la biblioteca Twint de Python para recolectar datos de Twitter y se recopilará información pública de data.world. Posteriormente, se aplicarán técnicas de procesamiento de lenguaje natural para limpiar y pre-procesar los datos. Después, se utilizarán distintos algoritmos de aprendizaje automático para entrenar un modelo capaz de detectar patrones en los datos y predecir el tipo de emoción en los tweets de un usuario de Twitter.

### Objetivos:
#### Objetivo General:
Desarrollar un modelo que permita detectar emociones en los tweets y analizar patrones en el lenguaje utilizado en Twitter para ayudar en la detección temprana de trastornos emocionales, entre otros.

### Ficheros:
* text_emotion: Dataset en que se basó el estudio para la aplicacion los modelos de prediccion. https://data.world/crowdflower/sentiment-analysis-in-text
* test_data: Dataset que se utilizó para probar el modelo final. Se creo a partir de webscrapping de Twitter con la libreria TWINTT. 
emotion_data_clean: El dataset resultó de la limpieza y exploracion del dataset text_emotion.
* dataset1: resultado del preprocesamiento. Este dataset se encuentran las emociones clasificadas del dataset original.
* dataset2: resultado del preprocesamiento. Este dataset se encuentran las emociones  del dataset original fueron transformadas en sentimientos como: Negativo, Positivo y Neutro.
* dataset3: resultado del preprocesamiento. Este dataset se encuentran las emociones  del dataset original fueron transformadas en sentimientos como: Negativo, Positivo y Neutro con el analisis de polaridad de Vader.

### Estructura del repositorio:
* EDA: https://github.com/neiluz/IT_Academy_ProyectoFinal/blob/main/Notebooks/Notebook%202%20-%20EDA.ipynb
* Pre - procesado: https://github.com/neiluz/IT_Academy_ProyectoFinal/blob/main/Notebooks/Notebook%203%20-%20Pre-procesado.ipynb
* Modelo CLF - Label Emociones: https://github.com/neiluz/IT_Academy_ProyectoFinal/blob/main/Notebooks/Notebook%204%20-%20Modelaje%20ML%20-%20Clasificacion%20Base.ipynb
* Modelo CLF - Label Sentimientos: https://github.com/neiluz/IT_Academy_ProyectoFinal/blob/main/Notebooks/Notebook%205%20-%20Modelaje%20ML%20-%20Clasificacion%20Polarity.ipynb
* MODELO CLF - Polaridad Vader: https://github.com/neiluz/IT_Academy_ProyectoFinal/blob/main/Notebooks/Notebook%206%20-%20Modelaje%20ML%20-%20Polarity%20Vader.ipynb
* Modelo BERT - Label Emociones: https://github.com/neiluz/IT_Academy_ProyectoFinal/blob/main/Notebooks/Notebook%207.1%20Modelaje%20DL%20Clasificacion%20Base.ipynb
* Modelo BERT - Label Sentimientos: https://github.com/neiluz/IT_Academy_ProyectoFinal/blob/main/Notebooks/Notebook%207.2a%20Modelaje%20DL%20Polarity%20Vader.ipynb
* Modelo BERT - Label Sentimientos - Balanceado: https://github.com/neiluz/IT_Academy_ProyectoFinal/blob/main/Notebooks/Notebook%207.2b%20Modelo%20Bert%20-%20Polarity%20-Balanceo%20clases.ipynb
* MODELO BERT - Polaridad Vader: https://github.com/neiluz/IT_Academy_ProyectoFinal/blob/main/Notebooks/Notebook%207.3a%20Modelaje%20DL%20Polarity%20Vader.ipynb
* MODELO BERT - Polaridad Vader - Balanceado: https://github.com/neiluz/IT_Academy_ProyectoFinal/blob/main/Notebooks/Notebook%207.3b%20Modelaje%20DL%20Polarity%20Vader%20balanceo.ipynb.ipynb

### Librerias utilizadas:
* Panda
* NLTK
* Tensor 
* Transformer de Bert 
* SKlearn: Algoritmos de clasificacion y metricas de evaluación.
* TWINTT

### Resultados:


### Fuentes utilizadas:
*  https://github.com/twintproject/twint
*  https://data.world/crowdflower/sentiment-analysis-in-text
* https://huggingface.co/docs/transformers/model_doc/bert
* Wong, Y. K., Lee, S. S., & Hung, E. (2017). Emotion Detection in Twitter Using Deep Learning Approaches. In Proceedings of the 2017 International Joint Conference on 
Neural Networks.
