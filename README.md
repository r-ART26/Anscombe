# El Cuarteto de Anscombe: La Importancia de Visualizar los Datos

<p align="center">
  <img width="1281" height="721" alt="image" src="https://github.com/user-attachments/assets/f36368ea-6d5e-4d07-8ac7-1c0c26b7f799" />
</p>

<div align="center">
  <h1>Universidad Politécnica Salesiana</h1>
  <h3>Roberto Alejandro Romero Torres</h3>
  <h3>Periodo 67</h3>
</div>

## 1. Resumen del Proyecto

Este documento presenta un análisis del **Cuarteto de Anscombe**, un conjunto de cuatro bases de datos publicadas por el estadístico Francis Anscombe in 1973. El objetivo principal de este cuarteto es servir como una demostración categórica de la **importancia fundamental de la visualización de datos** en el análisis estadístico.

Demuestra cómo métricas estadísticas descriptivas idénticas pueden ocultar realidades subyacentes drásticamente diferentes, subrayando los peligros de confiar únicamente en los resúmenes numéricos para comprender un conjunto de datos.

---

## 2. El Engaño de las Métricas Estadísticas

El cuarteto consiste en cuatro conjuntos de datos (I, II, III, IV), cada uno compuesto por 11 pares de puntos (x, y). La paradoja central es que, al calcular las propiedades estadísticas descriptivas más comunes, los cuatro conjuntos parecen ser virtualmente idénticos.

Como documentó Anscombe en su artículo de 1973, todos comparten las siguientes propiedades (con una precisión de dos o tres decimales):

| Propiedad Estadística | Valor |
| :--- | :--- |
| Media de X | 9.0 |
| Varianza de X | 11.0 |
| Media de Y | 7.50 |
| Varianza de Y | 4.125 |
| Correlación entre X e Y ($r$) | 0.816 |
| Línea de regresión lineal | $y = 3.00 + 0.500x$ |
| Coef. de determinación ($R^2$) | 0.67 |

Un analista que observara únicamente esta tabla concluiría, erróneamente, que los cuatro conjuntos de datos describen la misma relación lineal positiva y moderadamente fuerte.

---

## 3. La Revelación de la Visualización

La verdadera naturaleza de los datos solo se revela al graficarlos. Cada conjunto de datos cuenta una historia completamente diferente, invalidando la suposición inicial de similitud.

<p align="center">
  <img width="1200" height="800" alt="Visualización del Cuarteto de Anscombe" src="https://github.com/user-attachments/assets/296f1e8c-f415-4ad6-b8a0-ac41cef26e17" />
</p>

* **Conjunto I (Arriba Izquierda):** Es el único conjunto que se ajusta a la expectativa. Muestra una **relación lineal simple** y ruidosa, donde un modelo de regresión lineal es apropiado.

* **Conjunto II (Arriba Derecha):** Los datos exhiben una **relación no lineal** evidente (específicamente, una curva cuadrática). La línea de regresión lineal es completamente inadecuada para describir la tendencia real.

* **Conjunto III (Abajo Izquierda):** Muestra una **relación lineal casi perfecta** entre $x$ e $y$ para 10 de los 11 puntos. Sin embargo, un único **valor atípico (outlier)** desvía significativamente la línea de regresión, distorsionando la correlación.

* **Conjunto IV (Abajo Derecha):** No existe una relación lineal entre la mayoría de los puntos (que comparten el mismo valor $x=8$). La alta correlación y la línea de regresión están causadas enteramente por un único **punto de alta palanca (leverage point)** en `x=19`.

---

## 4. Referencias

* **Fuente Original:** Anscombe, F. J. (1973). "Graphs in Statistical Analysis". *The American Statistician*. 27 (1): 17–21. [doi:10.1080/00031305.1973.10478966](https://doi.org/10.1080/00031305.1973.10478966).
* **Análisis Moderno:** Tableau Software. (s.f.). *¿Qué es el cuarteto de Anscombe y por qué es importante?* Recuperado de: [https://www.tableau.com/es-es/learn/articles/anscombes-quartet](https://www.tableau.com/es-es/learn/articles/anscombes-quartet)
* **Contexto Adicional:** "Cuarteto de Anscombe". (2025). En *Wikipedia, la enciclopedia libre*. Recuperado el 30 de octubre de 2025, de: [https://es.wikipedia.org/wiki/Cuarteto_de_Anscombe](https://es.wikipedia.org/wiki/Cuarteto_de_Anscombe)
