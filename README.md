# Nuestras caras
Este repositorio contiene el código desarrollado por el **Grupo 4** para el trabajo final de la materia *Data Mining*, correspondiente a la *Maestría en Ciencia de Datos de la Universidad Austral*.

El objetivo del trabajo fue comprender el funcionamiento de las redes neuronales, así como los principales desafíos asociados a su entrenamiento y evaluación. La tarea elegida fue la detección y clasificación de rostros de los alumnos de esta materia.
Cabe destacar que este trabajo no busca replicar el estado del arte en visión computacional, sino que se desarrolla con fines exclusivamente educativos.

## Objetivo
Clasificar imágenes de rostros pertenecientes a los integrantes del grupo. El modelo entrenado debe ser capaz de identificar correctamente a las personas conocidas y rechazar (clasificar como intruso) imágenes de personas no vistas durante el entrenamiento.

## Estuctura proyecto

El desarrollo del trabajo se dividió en tres etapas principales:

**1. Preprocesamiento de imágenes**
Lectura de imágenes desde carpetas organizadas por persona. Detección automática de rostros utilizando un modelo DNN preentrenado. Recorte de la región del rostro con margen configurable. Conversión a escala de grises y redimensionado a 80x80 píxeles.

**2. Entrenamiento de la red (Grid Search)**
Red neuronal multicapa construida desde cero. Reducción de dimensionalidad mediante Isomap, con tuning de sus hiperparámetros. Búsqueda por grid de los mejores hiperparámetros de la red (Cantidad de capas, neuronas ocultas, función de activación, learning rate, epoch límite, umbral de error, semillas aleatorias). Análisis exploratorio de métricas, modelos y predicciones.

**3. Producción y evaluación final** 
Entrenamiento final con todos los datos disponibles usando la mejor combinación encontrada. Evaluación con imágenes nuevas y no vistas para simular una situación de producción. Definición de un umbral de confianza para decidir si una imagen pertenece a una persona conocida o debe ser clasificada como "intruso".
Visualización de la clasificación.

Autores: 
- Arenas, Cristian
- Banegas, Jorgelina
- Marín, Natalia
