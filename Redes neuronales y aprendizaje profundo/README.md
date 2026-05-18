# 📘 Curso 1: Redes Neuronales y Aprendizaje Profundo

Este curso es el pilar fundamental de la especialización de Deep Learning. Su principal objetivo es profundizar en la matemática, lógica y álgebra lineal detrás de las redes neuronales artificiales, construyendo los algoritmos paso a paso desde cero, utilizando únicamente **Python y NumPy** (sin recurrir a frameworks como TensorFlow o PyTorch).

---

## 🛠️ Contenido de los Módulos y Trabajos Prácticos

### 📅 Semana 2: Introducción a Redes Neuronales y Vectorización

*   **Lab 1:** [Conceptos Básicos de Python con NumPy](./Semana%202%20-%20Introduccion%20a%20Redes%20Neuronales/W2A1/Python_Basics_with_Numpy.ipynb)
    *   **Objetivo:** Dominar el uso de **NumPy** y la **vectorización**. Aprendemos a erradicar los bucles `for` (que ralentizan drásticamente los entrenamientos) mediante operaciones matriciales eficientes.
    *   **Claves:** Implementación de la función `sigmoid` y su derivada, redimensionamiento de matrices (`reshape`), normalización de filas, la función `softmax` y funciones de pérdida avanzadas (L1 y L2).
*   **Lab 2:** [Regresión Logística con Mentalidad de Red Neuronal](./Semana%202%20-%20Introduccion%20a%20Redes%20Neuronales/W2A2/Logistic_Regression_with_a_Neural_Network_mindset.ipynb)
    *   **Objetivo:** Construir un clasificador de imágenes real (Gato vs. No Gato) estructurando una Regresión Logística como una red neuronal monocapa.
    *   **Claves:** Inicialización de parámetros ($w$ y $b$), diseño de la propagación hacia adelante (Forward propagation para calcular el coste) y hacia atrás (Backward propagation para calcular gradientes), optimización con Descenso de Gradiente y ajuste empírico de la tasa de aprendizaje ($\alpha$).

---

### 📅 Semana 3: Redes Neuronales Superficiales (Una Capa Oculta)

*   **Lab 1:** [Clasificación de Datos Planares con una Capa Oculta](./Semana%203%20-%20Redes%20Neuronales%20Superficiales/W3A1/Planar_data_classification_with_one_hidden_layer%20(1).ipynb)
    *   **Objetivo:** Comprender la necesidad de la no linealidad en el aprendizaje profundo mediante la construcción de una red neuronal de dos capas para clasificar un conjunto de datos en forma de flor ("Planar Dataset") que la regresión logística lineal no puede separar.
    *   **Claves:** Uso de la función de activación `tanh` en la capa oculta y `sigmoid` en la de salida; cálculo y actualización manual de gradientes complejos; y análisis del impacto de variar el número de neuronas ocultas (tamaño de la capa oculta) en la frontera de decisión.

---

### 📅 Semana 4: Redes Neuronales Profundas (Múltiples Capas)

*   **Lab 1:** [Construyendo una Red Neuronal Profunda Paso a Paso](./Semana%204%20-%20Redes%20Neuronales%20Profundas/W4A1/Building_your_Deep_Neural_Network_Step_by_Step.ipynb)
    *   **Objetivo:** Desarrollar la infraestructura de una Red Neuronal Profunda genérica con $L$ capas totalmente personalizable y modular.
    *   **Claves:** Inicialización de parámetros para $L$ capas utilizando pesos no nulos; diseño de módulos de Forward Propagation lineal y lineal-activación (ReLU y Sigmoide); almacenamiento en caché de valores intermedios (caches) para optimizar la Backpropagation; e implementación de la actualización modular de parámetros.
*   **Lab 2:** [Red Neuronal Profunda - Aplicación](./Semana%204%20-%20Redes%20Neuronales%20Profundas/W4A2/Deep%20Neural%20Network%20-%20Application.ipynb)
    *   **Objetivo:** Aplicar la infraestructura desarrollada en el laboratorio anterior al problema de clasificación de gatos y contrastar empíricamente la efectividad de las arquitecturas profundas.
    *   **Claves:** Entrenamiento y comparación detallada de un modelo de 2 capas frente a uno profundo de 4 capas ($L$-capas), evidenciando cómo la jerarquía de representación de características incrementa significativamente la precisión y generalización del modelo.

---

## 💡 Aprendizajes Clave del Curso

1.  **Vectorización y Eficiencia:** El impacto masivo de la paralelización con NumPy para calcular activaciones y gradientes de millones de registros simultáneamente.
2.  **Backpropagation Matemática:** El entendimiento riguroso de cómo la regla de la cadena del cálculo se traduce en actualizaciones de parámetros paso a paso ($dW^{[l]}$, $db^{[l]}$).
3.  **Broadcasting y Dimensiones:** La rigurosidad de mantener la consistencia dimensional ($W$ de tamaño $(n^{[l]}, n^{[l-1]})$, $b$ de tamaño $(n^{[l]}, 1)$), una habilidad crítica para depurar cualquier arquitectura neuronal profunda.
