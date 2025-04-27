# ProyectoCNN_EnfermedadesPlantas
Clasificación automática de enfermedades en hojas de tomate usando redes neuronales convolucionales (CNNs)

# Proyecto de Clasificación de Enfermedades en Hojas de Tomate usando CNN

## Contexto de aplicación

La industria agrícola se enfrenta a desafíos crecientes relacionados con enfermedades en cultivos, que afectan directamente el rendimiento y la calidad de los productos. El tomate, uno de los cultivos más importantes a nivel mundial, es particularmente vulnerable a enfermedades foliares. La detección temprana y precisa de estas enfermedades puede ser clave para mitigar pérdidas económicas y optimizar procesos de producción. En este contexto, las redes neuronales convolucionales (CNN) ofrecen una solución automatizada, rápida y escalable para la identificación visual de enfermedades en las hojas del tomate.

## Objetivo de machine learning

Desarrollar un modelo de aprendizaje profundo basado en redes neuronales convolucionales (CNN) capaz de **clasificar automáticamente imágenes de hojas de tomate según la enfermedad presente** (o su estado saludable).  
El modelo recibirá como entrada imágenes en color de hojas y deberá predecir una etiqueta correspondiente a una de las posibles clases de enfermedad o al estado saludable.

## Dataset

El conjunto de datos utilizado es el [PlantVillage Tomato Leaf Dataset](https://www.kaggle.com/datasets/arjuntejaswi/plant-village), el cual contiene:

- **Tipo de datos:** Imágenes en formato JPG de hojas de tomate, clasificadas según la enfermedad.
- **Tamaño del dataset:** Aprox. 18,160 imágenes (~2 GB en disco).
- **Número de clases:** 10 clases (9 enfermedades + 1 clase de hoja sana).
- **Distribución de clases:** Relativamente balanceada. Ejemplo:
  - Tomato___Bacterial_spot: 2,123
  - Tomato___Early_blight: 1,997
  - Tomato___Healthy: 1,591
  - Tomato___Late_blight: 1,900
  - ...
  
*Se puede reducir el número de clases o cantidad de datos si se requiere disminuir la carga computacional.*

## Métricas de desempeño

### Métricas de Machine Learning
- **Accuracy (Precisión):** Porcentaje de predicciones correctas.
- **Precision, Recall y F1-score:** Para evaluar el desempeño por clase.
- **Matriz de confusión:** Para visualizar los errores entre clases.

### Métricas de negocio (contexto agrícola)
- **Tasa de detección temprana:** Impacto en la reducción de pérdidas.
- **Reducción de tiempo de diagnóstico humano.**
- **Usabilidad en soluciones móviles o drones para el agro.**

## Referencias y resultados previos

- Mohanty, S. P., Hughes, D. P., & Salathé, M. (2016). *Using deep learning for image-based plant disease detection*. Frontiers in Plant Science.
- En el artículo original, una CNN logró una precisión del 99.35% sobre este mismo dataset.
- Existen múltiples implementaciones en Kaggle y GitHub con modelos como VGG16, ResNet50 o modelos personalizados, que alcanzan resultados competitivos.

---


Enlace documento - https://docs.google.com/document/d/19Bx_iZTc4BACmrJ1LqGadQ_mkKRFByafJpbsg4TD2rM/edit?usp=sharing
