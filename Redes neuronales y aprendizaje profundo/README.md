#  Curso 1: Redes Neuronales y Aprendizaje Profundo

En este primer curso de la especialización, el enfoque principal es entender los fundamentos lógicos y matemáticos del Deep Learning, construyendo los algoritmos paso a paso sin depender de frameworks de alto nivel como TensorFlow o PyTorch.

## Proyectos y Notebooks

### 1. Conceptos Básicos de Python con NumPy
**Notebook:** [`Python_Basics_with_Numpy.ipynb`](./Python_Basics_with_Numpy.ipynb)

Una introducción fundamental a la vectorización utilizando NumPy. El objetivo principal de este ejercicio es demostrar por qué los bucles `for` son ineficientes en Machine Learning y cómo las operaciones matriciales paralelizadas aceleran drásticamente el cálculo de activaciones, gradientes y funciones de pérdida.

### 2. Regresión Logística con mentalidad de Red Neuronal
**Notebook:** [`Logistic_Regression_with_a_Neural_Network_mindset.ipynb`](./Logistic_Regression_with_a_Neural_Network_mindset.ipynb)

En este proyecto, implementé un clasificador de imágenes (Gato vs No Gato) utilizando Regresión Logística pura.
- Se implementaron las funciones matemáticas clave: `sigmoid`, propagación hacia adelante (para el costo) y propagación hacia atrás (para los gradientes).
- Se aplicó el algoritmo de **Gradient Descent** (Descenso de Gradiente) para optimizar los pesos y sesgos.
- El código está documentado línea por línea en el notebook para explicar la mecánica del álgebra lineal involucrada (dimensiones de matrices, broadcasting, etc).

##  Aprendizajes Clave
- **Vectorización:** Cómo eliminar ciclos anidados usando `np.dot()` y multiplicaciones elemento a elemento.
- **Backpropagation (Básico):** Cómo el gradiente de la función de costo nos guía para actualizar nuestros pesos $w$ y sesgo $b$.
- **Broadcasting en Python:** Una de las herramientas más útiles de NumPy para aplicar operaciones entre matrices de diferentes tamaños.
