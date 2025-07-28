# Multiplicación de Matrices: Algoritmo de Strassen

El algoritmo de Strassen es una mejora del método clásico de multiplicación de matrices que utiliza la estrategia de divide y vencerás. En lugar de realizar 8 multiplicaciones como el método tradicional para matrices 2x2, Strassen reduce este número a 7, compensándolo con operaciones adicionales de suma y resta. Esta optimización mejora la eficiencia asintótica, especialmente para matrices grandes.

## Caso 1: Multiplicación de matrices 2x2

Strassen divide cada matriz 2x2 en sus elementos individuales y calcula 7 productos intermedios que luego se combinan para formar la matriz resultado. Esta versión es ideal para explicar el funcionamiento del algoritmo en su forma más básica.

### Ejemplo

![WhatsApp Image 2025-07-28 at 01 54 44_6f20661a](https://github.com/user-attachments/assets/96b75d3c-8e9c-4a9a-96d6-cb4ace58bc0f)


## Caso 2: Multiplicación de matrices 4x4

Para matrices más grandes como las 4x4, se aplica Strassen de forma recursiva. Cada matriz se divide en cuatro submatrices de 2x2:

```
| 0 0 | 0 0 |
| 0 0 | 0 0 |
+-----+-----+
| 0 0 | 0 0 |
| 0 0 | 0 0 |
```

Luego se aplican las mismas operaciones del algoritmo de Strassen entre esas submatrices, tratándolas como si fueran elementos de una matriz 2x2. Finalmente, los resultados se ensamblan para obtener la matriz final de 4x4.

### Ejemplo

![WhatsApp Image 2025-07-28 at 01 55 02_dd815624](https://github.com/user-attachments/assets/510097d5-360d-45af-9003-f8590b4ae820)


## Conclusión

Strassen es una alternativa eficiente al método clásico de multiplicación de matrices, especialmente útil cuando se trabaja con matrices grandes o cuando se busca mejorar el rendimiento mediante técnicas de divide y vencerás. Aunque introduce más operaciones de suma y resta, reduce la cantidad de multiplicaciones, lo que se traduce en una mejor complejidad algorítmica en casos grandes.
