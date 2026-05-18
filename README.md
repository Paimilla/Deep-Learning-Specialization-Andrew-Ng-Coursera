<div align="center">
  <h1>🧠 Especialización en Deep Learning (Coursera)</h1>
  <p><strong>Mis soluciones, notas de aprendizaje e implementaciones detalladas de la especialización impartida por Andrew Ng (DeepLearning.AI).</strong></p>

  <p>
    <img src="https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
    <img src="https://img.shields.io/badge/NumPy-1.20+-777BB4?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy">
    <img src="https://img.shields.io/badge/TensorFlow-2.0+-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" alt="TensorFlow">
    <img src="https://img.shields.io/badge/Jupyter-F37626.svg?style=for-the-badge&logo=Jupyter&logoColor=white" alt="Jupyter">
  </p>
</div>

---

## 📋 Sobre este repositorio

Este repositorio es mi portafolio de estudio práctico sobre **Deep Learning** y **Redes Neuronales**. En lugar de simplemente completar los ejercicios sugeridos, he documentado exhaustivamente cada notebook con **anotaciones en español línea por línea y comentarios personales explicativos**. 

El objetivo principal es consolidar un entendimiento profundo de la matemática detrás del aprendizaje profundo (álgebra lineal, cálculo de gradientes y optimización) y construir algoritmos desde cero utilizando principalmente **Python y NumPy**, para luego transicionar a frameworks industriales como **TensorFlow y Keras**.

---

## 🗺️ Estructura de la Especialización

| Curso | Estado | Descripción y Proyectos Destacados |
| :--- | :---: | :--- |
| 📘 [**1. Redes Neuronales y Aprendizaje Profundo**](./Redes%20neuronales%20y%20aprendizaje%20profundo/) | **Completado** 🚀 | Construcción paso a paso de Regresión Logística y Redes Neuronales Profundas ($L$-capas) desde cero con NumPy para clasificación de imágenes. |
| 📙 [**2. Mejora de Redes Neuronales Profundas**](./Mejora%20de%20redes%20neuronales%20profundas/) | **Completado** 🚀 | Optimización del rendimiento: inicialización matemática (He/Xavier), regularización (L2, Dropout), algoritmos avanzados (Momentum, RMSprop, Adam) e introducción práctica a TensorFlow 2. |

*(Nota: A medida que avance en los siguientes cursos de la especialización, se irán integrando al índice del repositorio).*

---

## 🛠️ Tecnologías y Herramientas utilizadas

- **Python** como lenguaje de programación principal.
- **NumPy** para operaciones vectoriales eficientes y manejo matricial de alta velocidad.
- **Matplotlib** para visualizar fronteras de decisión, curvas de pérdida y análisis cualitativo de predicciones.
- **H5py y SciPy** para procesamiento e importación de datasets complejos (por ejemplo, imágenes en formato H5).
- **TensorFlow 2 y Keras** para el desarrollo rápido y la escalabilidad de modelos profundos en las últimas etapas.

---

## 🚀 Cómo ejecutar los proyectos localmente

Para explorar los notebooks y experimentar con los modelos:

1. **Clona este repositorio:**
   ```bash
   git clone https://github.com/fpaim/Deep-Learning-Specialization-Andrew-Ng-Coursera.git
   cd Deep-Learning-Specialization-Andrew-Ng-Coursera
   ```

2. **Crea y activa un entorno virtual de Python:**
   ```bash
   python -m venv .venv
   # En Windows:
   .venv\Scripts\activate
   # En macOS/Linux:
   source .venv/bin/activate
   ```

3. **Instala las dependencias necesarias:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Inicia Jupyter Notebook o ejecuta en tu IDE favorito (como VS Code):**
   ```bash
   jupyter notebook
   ```

---

## ✍️ Mi Filosofía de Aprendizaje
Cada línea de código en estos notebooks ha sido analizada y comentada detalladamente. Mi enfoque es:
1. **No usar cajas negras:** Programar primero desde cero ($w$ y $b$, activaciones, costes y gradientes) para interiorizar el flujo real.
2. **Documentar el "Por qué":** Explicar en español las dimensiones matriciales, el broadcasting y la lógica detrás del código.
3. **Análisis de Hiperparámetros:** Evaluar de forma práctica cómo impacta variar la tasa de aprendizaje ($\alpha$), el número de épocas, la regularización o el método de inicialización en el comportamiento final del modelo.
