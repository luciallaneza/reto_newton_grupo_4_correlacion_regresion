# *Definiciones básicas* 🔠
Veremos muy brevemente:
- Ouliers
- Keepdims
- Asimetría - Skewness
- Cuartiles
- p-value


## **Outlier**
Un outlier, o valor atípico en estadística, es una observación numéricamente distante del resto de los datos, indicando un comportamiento inusual o un posible error en la muestra.   
 Estos valores pueden distorsionar los análisis (como la media), por lo que suelen identificarse con métodos gráficos (diagramas de caja) o analíticos (rango intercuartílico, 1.5 x IQR) para investigar si son errores o hallazgos genuinos.

 ------

 ## **Keepdims**
 Keepdims es un parámetro fundamental en bibliotecas de computación científica como NumPy en Python, utilizado para mantener la dimensionalidad original de un array al realizar operaciones estadísticas de reducción (como media, suma, varianza).   

¿Qué hace keepdims en estadística y programación?   
Sin keepdims (valor por defecto False): Cuando calculas una estadística (por ejemplo, la media) a lo largo de un eje (axis), ese eje desaparece, reduciendo el rango (número de dimensiones) del array original.   
Con keepdims=True: La dimensión reducida se mantiene como una dimensión de tamaño uno (1). Esto permite que el resultado sea “transmitible” (broadcastable) de vuelta con el array original, lo cual es crucial para la normalización de datos.

------

## **Asimetría - Skewness**

Mide si los datos están sesgados hacia un lado.   
`from scipy.stats import stew`

---

## **Cuartiles**

Los cuartiles (Q1, Q2, Q3) son medidas estadísticas de posición que dividen un conjunto de datos ordenados en cuatro partes iguales, cada una representando el 25% de las observaciones. El Q1 (25%) marca el primer cuartil, Q2 es la mediana (50%), y Q3 (75%) representa el tercer cuartil. Se usan para analizar la distribución y dispersión.

---

## **p-value**

Los cuartiles (Q1, Q2, Q3) son medidas estadísticas de posición que dividen un conjunto de datos ordenados en cuatro partes iguales, cada una representando el 25% de las observaciones. El Q1 (25%) marca el primer cuartil, Q2 es la mediana (50%), y Q3 (75%) representa el tercer cuartil. Se usan para analizar la distribución y dispersión.  

### Puntos clave del p-value:

•	**Interpretación:** Mide la compatibilidad de los datos con la hipótesis nula. Valores pequeños implican que los datos son improbables bajo la H0.

•	**Umbral estándar:** Se utiliza comúnmente un nivel de significancia de 0.05. Si p<=0.05, se rechaza H0. Si p>0.05, no se rechaza H0.

•	**Significado de los valores:**

    - p < 0.01: Resultado muy significativo.
    - p < 0.05: Resultado significativo.
    - p > 0.05: Resultado no significativo (no hay evidencia suficiente para rechazar H0).
•	**Limitaciones:** No mide la magnitud del efecto, solo la significancia estadística. Un tamaño de muestra grande puede generar p-values pequeños incluso con diferencias triviales.

•	**Errores comunes:** No es la probabilidad de que la hipótesis nula sea falsa. Un p-value de 0.01 no significa que haya un 99% de probabilidad de que la hipótesis alternativa sea cierta. 

### ¿Cuándo rechazar la hipótesis nula? 🤔💭
Si el p-value calculado es menor o igual al nivel de significancia prefijado (normalmente 0.05), se rechaza la hipótesis nula (H0), concluyendo que existen diferencias significativas.

----




