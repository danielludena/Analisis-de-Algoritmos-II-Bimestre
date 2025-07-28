# Algoritmos Voraces

Los algoritmos voraces (también conocidos como *greedy algorithms*) son una estrategia fundamental en el diseño de algoritmos que resuelve problemas mediante la toma de decisiones óptimas locales en cada paso, con la esperanza de que dichas decisiones conduzcan a una solución óptima global.

## Características clave

- **Rápidos y fáciles de implementar**: Suelen tener una estructura sencilla y requieren menos recursos computacionales en comparación con otras técnicas como la programación dinámica.
- **Ideales para problemas de optimización**: Se usan donde se busca minimizar o maximizar una cantidad (costos, ganancias, tiempos, etc.).
- **Toman decisiones heurísticas**: Cada paso se toma de forma "miopemente óptima", es decir, eligiendo lo mejor en ese momento sin mirar el panorama completo.
- **Enfoque paso a paso**: No se reconsideran decisiones anteriores.
- **Esperanza de alcanzar el óptimo global**: Aunque no siempre garantizan la mejor solución, sí lo hacen en muchos problemas clásicos.

## Aplicaciones comunes

- Selección de actividades.
- Árbol de recubrimiento mínimo (Kruskal y Prim).
- Codificación de Huffman.
- Problema del cambio de monedas (siempre que la estructura de monedas lo permita).
- Caminos mínimos en grafos con restricciones específicas.

## Ventajas y desventajas

| Ventajas                           | Desventajas                                                   |
|------------------------------------|----------------------------------------------------------------|
| Simplicidad y eficiencia           | No garantiza el óptimo global en todos los problemas           |
| Buena aproximación en muchos casos | Requiere análisis formal para validar su efectividad           |
| Bajo consumo de memoria            | Puede dar resultados incorrectos si no se cumple la propiedad  |

## Ejemplo visual con prueba de escritorio

![WhatsApp Image 2025-07-27 at 23 21 03_1ef937d4](https://github.com/user-attachments/assets/0e9d1c2d-063b-460e-a0b6-cc86f406f1ed)
