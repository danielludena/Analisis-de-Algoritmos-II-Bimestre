# Búsqueda Binaria y Divide y Vencerás

La **búsqueda binaria** es un algoritmo eficiente para encontrar un elemento en una colección ordenada. Este algoritmo se basa en dividir el espacio de búsqueda en mitades sucesivas, descartando la mitad en la que el elemento no puede estar. Su eficiencia lo convierte en una herramienta fundamental en estructuras de datos y algoritmos.

## Búsqueda Binaria

### Descripción

Dado un arreglo ordenado de tamaño `n` y un valor objetivo `x`, la búsqueda binaria compara `x` con el elemento del medio del arreglo:

1. Si `x` es igual al elemento del medio, se ha encontrado el valor.
2. Si `x` es menor, la búsqueda continúa en la mitad izquierda.
3. Si `x` es mayor, la búsqueda continúa en la mitad derecha.

Este proceso se repite hasta encontrar el elemento o hasta que el subarreglo quede vacío.

### Requisitos

- El arreglo debe estar ordenado previamente (de menor a mayor, generalmente).
- Puede implementarse de forma iterativa o recursiva.

### Complejidad

- **Tiempo (mejor caso):** O(1) – si el elemento está en el centro en la primera comparación.
- **Tiempo (peor y caso promedio):** O(log n)
- **Espacio:** O(1) en versión iterativa, O(log n) en versión recursiva (por el stack de llamadas).

### Ejemplo

Supongamos el arreglo ordenado: `[2, 4, 7, 10, 13, 18, 21]`  
Queremos buscar el número `10`.

1. Comparamos con el centro: `10` vs `10` → coincide → encontrado.

Si buscáramos el `13`, descartaríamos la mitad izquierda tras la primera comparación y repetiríamos el proceso en la mitad derecha.

## Divide y Vencerás

La **búsqueda binaria** es un ejemplo clásico de la técnica de diseño de algoritmos llamada **divide y vencerás**, que consiste en:

1. **Dividir** el problema en subproblemas más pequeños.
2. **Resolver** cada subproblema (a menudo de forma recursiva).
3. **Combinar** las soluciones si es necesario.

En el caso de búsqueda binaria:

- **Dividir:** se reduce el arreglo a la mitad en cada paso.
- **Vencer:** se compara con el elemento central.
- **No es necesario combinar**, ya que solo se busca un elemento.

Esta técnica es poderosa y se aplica en muchos otros algoritmos como mergesort, quicksort, y transformada rápida de Fourier (FFT), entre otros.

## Conclusion con prueba de escritorio

![WhatsApp Image 2025-07-27 at 23 48 50_50c34e86](https://github.com/user-attachments/assets/8d069ce7-a833-427c-9b41-a9e9cd0b3c02)
