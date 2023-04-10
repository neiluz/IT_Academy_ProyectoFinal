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
* out : resultados de aplicar la pipeline con Vader al fichero test_data

### Estructura del repositorio:
* EDA
* Pre - procesado
* Modelo CLF - Label Emociones
* Modelo CLF - Label Sentimientos
* MODELO CLF - Polaridad Vader
* Modelo BERT - Label Emociones
* Modelo BERT - Label Sentimientos
* Modelo BERT - Label Sentimientos - Balanceado
* MODELO BERT - Polaridad Vader
* MODELO BERT - Polaridad Vader - Balanceado

### Librerias utilizadas:
* Panda
* NLTK
* Tensor 
* Transformer de Bert 
* SKlearn: Algoritmos de clasificacion y metricas de evaluación.
* TWINTT

### Resultados:
En el presente estudio, se compararon dos modelos de análisis de sentimientos: SGDClassifier y BERT, aplicados a diferentes conjuntos de datos etiquetados con diferentes niveles de granularidad. La Tabla  muestra una comparación de las métricas de rendimiento de ambos modelos. 

[![libro](https://github.com/neiluz/IT_Academy_ProyectoFinal/blob/main/Libro1-htm.jpg)](https://www.github.com/) 

Los resultados indican que el modelo BERT supera al SGDClassifier en todos los conjuntos de datos analizados en términos de métricas de rendimiento de clasificación de sentimientos. En particular, el modelo BERT mostró un mejor rendimiento en el conjunto de datos etiquetados con sentimientos, alcanzando valores de f1, precisión y recall superiores al 60%. Además, los resultados sugieren que el balanceo de los datos puede ser una estrategia efectiva para mejorar el rendimiento del modelo en la clasificación de sentimientos con polaridad de Vader. Sin embargo, el modelo BERT todavía tiene dificultades en la detección de ciertas emociones, como "anger" y "boredom", lo que indica que se necesitan más investigaciones para mejorar el rendimiento del modelo en estas áreas.

### Fuentes utilizadas:
*  https://github.com/twintproject/twint
*  https://data.world/crowdflower/sentiment-analysis-in-text
* https://huggingface.co/docs/transformers/model_doc/bert
* Wong, Y. K., Lee, S. S., & Hung, E. (2017). Emotion Detection in Twitter Using Deep Learning Approaches. In Proceedings of the 2017 International Joint Conference on 
Neural Networks.
