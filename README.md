# Trabajo Fin de Grado

Este repositorio contiene mi Trabajo Fin de Grado para la titulación de Doble Grado en Ingeniería Informática y Matemáticas de la Universidad de Granada. 

En el trabajo se presentan los conceptos más relevantes de la Teoría de Distribuciones con el objetivo de desarrollar los resultados presentados por Chen y Chen en el artículo [Universal approximation to nonlinear operators by neural networks with arbitrary activation functions and its application to dynamical systems](https://ieeexplore.ieee.org/document/392253). Los avances más relevantes que se proponen son: 

- Toda función de Tauber-Wiener es válida como función de activación de una red neuronal profunda.
- Para que una función  continua $g\in S'(\mathbb{R})$ sea de Tauber-Wiener, basta con que $g$ no sea un polinomio. 
- Para cualquier función de activación de Tauber-Wiener, podemos encontrar una arquitectura de red neuronal profunda que aproxime funcionales y operadores sobre conjuntos compactos en espacios de Banach.  
- Como consecuencia, es posible aproximar e identificar sistemas dinámicos regidos por operadores, lineales o no, mediante redes neuronales profundas.

Posteriormente se realiza un estudio del estado del arte para la aproximación de sistemas dinámicos mediante redes neuronales, que se corresponde con el enfoque de las Physics-Informed-Neural-Networks (PINNs) y la librería de referencia para la implementación de PINNs: [SciANN](https://github.com/sciann/sciann). Además, desarrollamos una serie de experimentos para mostrar las características [SciANN](https://github.com/sciann/sciann) y sus diferencias con las librerías más populares orientadas al aprendizaje profundo. Por último, se propone una implementación para un aproximador de operadores en [SciANN](https://github.com/sciann/sciann) y se compara con el aproximador de operadores propuesto en [DeepONet](https://github.com/lululxvi/deeponet).

El trabajo compilado puede consultarse [aquí](tfg.pdf).

# Estructura del repositorio 

Las fuentes se organizan en dos carpetas:
- En el directorio `Memoria` se encuentran las fuentes en latex de la memoria del trabajo. 
- En el directorio `Experimentos` se encuentran los cuadernos de Jupyter desarrollados para la experimentación con SciANN discutida en el capítulo 8 de la memoria:
  - El cuaderno `experimento-1` implementa varios modelos de regresión en SciANN con el objetivo de estudiar cómo escala la librería. 
  - En el cuaderno `experimento-2` se trabaja en un aproximador de la función que describe el problema de Burgers.  
  - En los cuadernos `experimento-3-a` y `experimento-3-b` se proponen dos implementaciones de modelos para la aproximación de operadores en [SciANN](https://github.com/sciann/sciann) y se realiza un estudio comparativo con la implementación propuesta en [DeepONet](https://github.com/lululxvi/deeponet).
