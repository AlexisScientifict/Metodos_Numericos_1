# Métodos Numéricos: Interpolación y Aproximación 🧮

Este repositorio contiene implementaciones en Python de diversos algoritmos de análisis numérico orientados a la interpolación y aproximación de funciones. Es el resultado de mi primer curso  a la algoritmia numérica.

## 📌 Contenido

El repositorio está dividido en scripts de Python (`.py`) y notebooks interactivos (`.ipynb`) e incluye los siguientes métodos:

* **Interpolación de Lagrange:** Polinomio interpolador de grado n.
* **Método de Newton (Diferencias Divididas):** Construcción del polinomio usando diferencias divididas.
* **Método de Neville:** Evaluación iterativa de polinomios de interpolación.
* **Interpolación de Hermite:** Polinomio osculador que coincide en valores de función y derivadas.
* **Trazadores (Splines):** Interpolación mediante splines cúbicos.

## 🛠️ Tecnologías Utilizadas
* Python 3.x
* Jupyter Notebook / Google Colab
* Bibliotecas: `numpy`, `matplotlib`, `sympy`, `math`

## 📐 Fundamento Matemático

A continuación, se presentan las bases matemáticas de dos de los métodos principales implementados en este repositorio:

**Interpolación de Lagrange**
El polinomio de interpolación de Lagrange de grado $n$ se define como:
$$P(x) = \sum_{j=0}^{n} f(x_j) L_j(x)$$

Donde $L_j(x)$ representa los polinomios base, calculados de la siguiente manera:
$$L_j(x) = \prod_{\substack{k=0 \\ k \neq j}}^{n} \frac{x - x_k}{x_j - x_k}$$

**Método de Newton (Diferencias Divididas)**
El polinomio interpolador de Newton se expresa en función de sus diferencias divididas como:
$$P(x) = f[x_0] + \sum_{k=1}^{n} f[x_0, x_1, \dots, x_k] \prod_{i=0}^{k-1} (x - x_i)$$

## 🚀 Cómo usar este repositorio

1. Clona el repositorio en tu máquina local:
   ```bash
   git clone [https://github.com/AlexisScientifict/Metodos_Numericos_1.git](https://github.com/AlexisScientifict/Metodos_Numericos_1.git)
