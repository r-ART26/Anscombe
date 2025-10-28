# Anscombe
<img width="1281" height="721" alt="image" src="https://github.com/user-attachments/assets/f36368ea-6d5e-4d07-8ac7-1c0c26b7f799" />

<div align="center">
  <h1>Universidad Politécnica Salesiana</h2>
  <h3>Roberto Alejandro Romero Torres</h1>
  <h3>Periodo 67</h3>
</div>

## Introducción Teórica al Cuarteto de Anscombe

El **Cuarteto de Anscombe** es un conjunto de cuatro colecciones de datos (pares X, Y) que fueron creados por el estadístico **Francis Anscombe** en 1973. Su propósito es demostrar de manera contundente las limitaciones de los estadísticos descriptivos simples y la importancia fundamental de **visualizar los datos** antes de analizarlos.

### La Paradoja: Estadísticas Idénticas

A primera vista, los cuatro conjuntos de datos parecen ser prácticamente idénticos si solo observamos sus propiedades estadísticas básicas.

Todos ellos comparten (con pequeñas variaciones decimales):

* **Media de X:** 9.0
* **Media de Y:** 7.5
* **Varianza de X:** 11.0
* **Varianza de Y:** 4.12
* **Correlación (r) entre X e Y:** 0.816
* **Línea de regresión lineal:** `y = 0.5x + 3`

Basándose únicamente en estos números, uno podría concluir erróneamente que los cuatro conjuntos de datos tienen una distribución similar y una relación lineal positiva fuerte.

### La Revelación: El Poder de la Visualización

Sin embargo, la realidad es drásticamente diferente. Cuando estos cuatro conjuntos se grafican en un diagrama de dispersión, revelan naturalezas completamente distintas:

<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ec/Anscombes_quartet_3.svg/800px-Anscombes_quartet_3.svg.png" alt="Gráficos del Cuarteto de Anscombe" width="700">
</p>

1.  **Conjunto I (Arriba Izquierda):** Muestra una relación lineal clara y simple, con una dispersión de puntos normal. Es el único conjunto que se ajusta bien al modelo de regresión lineal.
2.  **Conjunto II (Arriba Derecha):** Los datos no siguen una línea recta, sino una curva clara (una relación no lineal). La regresión lineal es completamente inapropiada aquí.
3.  **Conjunto III (Abajo Izquierda):** La relación es perfectamente lineal, pero está distorsionada por un único valor atípico (outlier) que desvía la línea de regresión.
4.  **Conjunto IV (Abajo Derecha):** Los datos no tienen relación alguna, excepto por un único punto de palanca (leverage point) en `x=19` que "tira" de la línea de regresión y crea la alta correlación.

> **La lección principal del Cuarteto de Anscombe es: "Nunca confíes ciegamente en las métricas estadísticas. Grafica tus datos primero".**

---

### Referencia

* **Anscombe, F. J. (1973).** "Graphs in Statistical Analysis". *The American Statistician*. 27 (1): 17–21. [doi:10.1080/00031305.1973.10478966](https://doi.org/10.1080/00031305.1973.1047
