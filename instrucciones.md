# TODO
## Parámetros de entrada
Por lo que vi esperas que el parámetro de la funcion sea una matriz de adyacencia
el formato de información que es enviado por mi js es distinto, envia nodos y aristas por separado
de la manera:

```python
nodos = ["A", "B", "C", "D"]
aristas = [
    ["A", "B"],
    ["A", "C"],
    ["B", "C"],
    ["B", "D"],
    ["C", "D"]
]  

Que es lo mismo (creo) que:

matriz = [
    [0, 1, 1, 0],
    [1, 0, 1, 1],
    [1, 1, 0, 1],
    [0, 1, 1, 0]
]
```

Todas esas son aristas bidireccionales, ahora, alguno de los dos puede hacer un método para
transformar esto en una matriz de adyacencia, podemos darselo a alguien más para que lo haga
o no se si es más facil cambiar el código tuyo directamente.

## Return de la función
También vi que el programa que hiciste lo que hace es imprimir a la consola la información de que 
si es euleriano, hamiltoniano, camino, circuito, etc... Pero para que el programa funcione bien necesito
que tus funciones devulvan esa infomación de alguna manera, preferiblemente como String o array de Strings:

```python
respuestas = ["Es camino euleriano"]

respuestas = [
    "Es circuito euleriano",
    "Es camino hamiltoniano",
]
```