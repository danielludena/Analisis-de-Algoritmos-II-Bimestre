# Árboles de Recubrimiento Mínimo (MST)

Un **árbol de recubrimiento mínimo** (Minimum Spanning Tree, MST) es un subconjunto de las aristas de un grafo no dirigido, conectado y ponderado, que conecta todos los vértices sin formar ciclos y con el peso total mínimo posible.

Este concepto es ampliamente utilizado en problemas de redes, rutas, planificación y estructuras óptimas.

## 1. Grafos No Dirigidos

En los grafos no dirigidos con pesos asociados a las aristas, los algoritmos clásicos para encontrar el árbol de recubrimiento mínimo son:

### Algoritmo de Kruskal

- Ordena todas las aristas por peso.
- Agrega aristas al árbol si no forman un ciclo (utilizando estructuras como conjuntos disjuntos).
- Se detiene cuando el MST tiene `n - 1` aristas, donde `n` es el número de vértices.

### Algoritmo de Prim

- Comienza en un vértice arbitrario.
- Agrega la arista de menor peso que conecte un vértice dentro del MST con uno fuera.
- Repite hasta que todos los vértices estén conectados.

Ambos algoritmos encuentran el mismo resultado, pero su eficiencia depende de la estructura del grafo y de la implementación.

#### Ejemplo gráfico de grafo no dirigido

![WhatsApp Image 2025-07-27 at 23 42 23_c4bfbeaa](https://github.com/user-attachments/assets/c4f2cfa7-2e02-4e81-bd7f-534c8eecbaab)

## 2. Grafos Dirigidos

En grafos dirigidos, **no se puede construir un MST en el mismo sentido**, ya que el concepto de árbol de recubrimiento mínimo requiere que el grafo sea no dirigido. Sin embargo, existe un concepto análogo llamado **árbol de expansión dirigido o árbol de recubrimiento arborescente** (*arborescence*), y su versión mínima se llama:

### Árbol Arborescente de Costo Mínimo

- Este problema se conoce como el **problema de Edmonds** o **Chu–Liu/Edmonds algorithm**.
- Dado un vértice raíz, se construye un árbol dirigido que alcanza todos los vértices del grafo con el menor costo total.
- Las aristas deben respetar la dirección.

Este tipo de estructura tiene aplicaciones en redes dirigidas y diseño de sistemas donde las conexiones no son bidireccionales.

#### Ejemplo gráfico de grafo dirigido

![WhatsApp Image 2025-07-27 at 23 43 07_ed3430f5](https://github.com/user-attachments/assets/a79cb879-55ff-444b-bd99-cda27e466896)

![WhatsApp Image 2025-07-27 at 23 42 44_e10eb4ee](https://github.com/user-attachments/assets/4eec0125-b3a1-4eea-a263-3817831d7a3c)
