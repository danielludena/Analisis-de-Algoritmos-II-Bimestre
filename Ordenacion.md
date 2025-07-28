# Algoritmos de Ordenación: Merge Sort y Quick Sort

Los algoritmos de ordenación son fundamentales en la informática, ya que muchas tareas dependen de tener datos ordenados para funcionar de manera eficiente. A continuación se presentan dos algoritmos clásicos basados en la técnica de **divide y vencerás**: **Merge Sort** y **Quick Sort**.

---

## Merge Sort

### Descripción

**Merge Sort** (ordenación por mezcla) es un algoritmo que divide el arreglo en mitades de forma recursiva hasta que cada subarreglo tiene un solo elemento, y luego los combina (merge) en orden ascendente.

### Pasos del algoritmo

1. Dividir el arreglo en dos mitades.
2. Aplicar Merge Sort recursivamente a cada mitad.
3. Mezclar las mitades ordenadas en un solo arreglo ordenado.

### Ejemplo: Prueba de escritorio

Arreglo inicial: `[54, 26, 93, 17, 77, 31, 44, 55, 20]`

#### Imagen del proceso:

![WhatsApp Image 2025-07-28 at 01 33 20_dc999b75](https://github.com/user-attachments/assets/27e4e72b-fc09-46cc-b8a5-38a2547b6b9d)

## Quick Sort

### Descripción

**Quick Sort** es un algoritmo de ordenación que selecciona un elemento pivote y particiona el arreglo de manera que todos los elementos menores que el pivote queden a la izquierda, y los mayores a la derecha. Luego aplica Quick Sort recursivamente a cada subarreglo.

### Pasos del algoritmo

1. Elegir un pivote (normalmente el primero, último o uno aleatorio).
2. Reorganizar el arreglo de modo que:
   - Los elementos menores al pivote queden a la izquierda.
   - Los mayores al pivote queden a la derecha.
3. Aplicar recursivamente Quick Sort a las sublistas izquierda y derecha.

### Complejidad

- **Tiempo promedio:** O(n log n)
- **Peor caso:** O(n²) (cuando la partición es muy desequilibrada)
- **Espacio:** O(log n) por el uso del stack de recursión

### Ejemplo: Prueba de escritorio

Arreglo inicial: `[3, 1, 4, 1, 5, 9, 2]`  
Se usará el **último elemento como pivote** en cada paso.

#### Paso 1: pivote = 2

Comparaciones:
- 3 > 2 → se queda
- 1 < 2 → intercambia con 3 → `[1, 3, 4, 1, 5, 9, 2]`
- 4 > 2 → se queda
- 1 < 2 → intercambia con 3 → `[1, 1, 4, 3, 5, 9, 2]`

Colocamos el pivote en su lugar → `[1, 1, 2, 3, 5, 9, 4]`  
`2` queda en su posición final (índice 2)

#### Paso 2: subarreglo izquierdo `[1, 1]` → ya está ordenado

#### Paso 3: subarreglo derecho `[3, 5, 9, 4]`, pivote = 4

Comparaciones:
- 3 < 4 → OK
- 5 > 4 → se queda
- 9 > 4 → se queda

Colocamos el pivote → intercambiamos 5 y 4 → `[1, 1, 2, 3, 4, 9, 5]`  
`4` queda en posición final (índice 4)

#### Paso 4: subarreglo `[9, 5]`, pivote = 5

- 9 > 5 → se queda

Intercambiamos 9 y 5 → `[1, 1, 2, 3, 4, 5, 9]`

#### Arreglo final ordenado: `[1, 1, 2, 3, 4, 5, 9]`

---

## Conclusión

Tanto **Merge Sort** como **Quick Sort** utilizan la técnica de divide y vencerás, pero se comportan de manera distinta en cuanto a rendimiento y uso de memoria.  
- **Merge Sort** garantiza un rendimiento estable en O(n log n), pero requiere espacio adicional.
- **Quick Sort** es más rápido en la práctica, pero puede degradarse a O(n²) si no se elige bien el pivote.
