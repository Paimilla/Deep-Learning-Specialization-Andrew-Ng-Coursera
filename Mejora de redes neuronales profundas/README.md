# 📙 Curso 2: Mejora de Redes Neuronales Profundas: Ajuste de Hiperparámetros, Regularización y Optimización

Este segundo curso de la especialización está completamente enfocado en los aspectos prácticos y avanzados que determinan el éxito de un modelo profundo en producción. Una vez consolidada la teoría matemática de las redes neuronales, este curso nos capacita para **mejorar su rendimiento, acelerar drásticamente los entrenamientos y evitar el sobreajuste (overfitting)** mediante técnicas industriales de vanguardia, para finalmente dar el salto a frameworks industriales.

---

## 🛠️ Contenido de los Módulos y Trabajos Prácticos

### 📅 Semana 1: Inicialización, Regularización y Verificación de Gradientes

*   **Lab 1:** [Inicialización de Parámetros](./Semana%201%20-%20Inicializacion,%20Regularizacion%20y%20Gradientes/W1A1/Initialization.ipynb)
    *   **Objetivo:** Comprender experimentalmente por qué los valores iniciales de los pesos ($W$) son críticos para la convergencia y estabilidad de una red profunda.
    *   **Claves:** Comparativa empírica entre inicialización con **Ceros** (provoca simetría e inhabilita la diferenciación de neuronas), inicialización **Aleatoria Grande** (induce saturación en funciones de activación y explosión de gradientes) e inicialización de **Xavier / He** (ideal para activaciones ReLU, estabilizando el gradiente).
*   **Lab 2:** [Regularización](./Semana%201%20-%20Inicializacion,%20Regularizacion%20y%20Gradientes/W1A2/Regularization.ipynb)
    *   **Objetivo:** Desarrollar e implementar mecanismos eficaces para combatir el sobreajuste (alta varianza) y asegurar que el modelo generalice de forma óptima en conjuntos de prueba no vistos.
    *   **Claves:** Programación desde cero de **Regularización L2** (penalizando la norma de Frobenius de las matrices de pesos en la función de coste y la retropropagación) y **Dropout** (apagado aleatorio e invertido de neuronas en cada iteración mediante máscaras booleanas).
*   **Lab 3:** [Verificación de Gradientes (Gradient Checking)](./Semana%201%20-%20Inicializacion,%20Regularizacion%20y%20Gradientes/W1A3/Gradient_Checking.ipynb)
    *   **Objetivo:** Crear una herramienta de depuración matemática de alta precisión para verificar que la implementación manual de Backpropagation es matemáticamente perfecta y no presenta bugs sutiles de cálculo.
    *   **Claves:** Estimación del gradiente numérico usando diferencias finitas simétricas bilaterales y su validación cuantitativa frente a los gradientes analíticos a través de la diferencia normalizada (el error relativo debe ser menor a $10^{-7}$).

---

### 📅 Semana 2: Algoritmos de Optimización

*   **Lab 1:** [Métodos de Optimización](./Semana%202%20-%20Algoritmos%20de%20Optimizacion/W2A1/Optimization_methods.ipynb)
    *   **Objetivo:** Superar las limitaciones de velocidad del Descenso de Gradiente tradicional (Batch Gradient Descent) implementando optimizadores modernos capaces de navegar valles y mesetas de forma ultra-rápida.
    *   **Claves:** Implementación de **Mini-batch Gradient Descent** (partición eficiente de los datos), Descenso de Gradiente con **Momentum** (medias móviles exponencialmente amortiguadas para reducir oscilaciones), **RMSprop** (normalización del gradiente mediante raíces cuadradas ponderadas) y el optimizador **Adam** (la fusión definitiva de Momentum y RMSprop). También se programa la atenuación de la tasa de aprendizaje (**Learning Rate Decay**).

---

### 📅 Semana 3: Ajuste de Hiperparámetros, Batch Norm y Frameworks

*   **Lab 1:** [Introducción a TensorFlow](./Semana%203%20-%20Ajuste%20de%20Hiperparametros%20y%20Batch%20Norm/W3A1/Tensorflow_introduction.ipynb)
    *   **Objetivo:** Transicionar de la programación puramente manual en NumPy al uso de frameworks de estándar industrial. Aprender la sintaxis de **TensorFlow 2.x** y la potencia de su API de alto nivel **Keras** para construir redes de manera limpia y ágil.
    *   **Claves:** Fundamentos de tensores, computación en grafos, cálculo automático de gradientes con `tf.GradientTape`, codificación One-Hot y construcción de una red profunda multicapa para clasificar imágenes de señas manuales con números del 0 al 5, implementando flujos de inicialización, optimización y regularización en un par de líneas.

---

## 💡 Aprendizajes Clave del Curso

1.  **Estabilización de Gradientes:** La inicialización inteligente (He/Xavier) como primer paso indispensable para entrenar redes profundas sin sufrir desvanecimiento o explosión de gradientes.
2.  **Mitigación Científica del Overfitting:** El balance óptimo entre sesgo (bias) y varianza (variance) mediante el uso coordinado de L2 y Dropout.
3.  **Aceleración Extrema (Adam):** Cómo optimizadores que usan momentum y adaptabilidad de tasas de aprendizaje pueden acelerar drásticamente la convergencia del entrenamiento.
4.  **Flujos de Trabajo Industriales:** La comprensión del valor de frameworks como TensorFlow para delegar la matemática derivativa automatizada y enfocarse en la arquitectura e iteración del modelo.
