# reto_10_re_facil
### arreglos y listas
1. Desarrollar un algoritmo que calcule el promedio de un arreglo de reales.

```pseudocode
print("promedio de una lista de reales #4.0, 2.5, 3.8, 5.7, -1.0")
lista:float = [4.0, 2.5, 3.8, 5.7, -1.0] #arreglo de reales con 5 componentes
#funcion para calcular el promedio
def calcular_promedio(lista) -> float:
    cantidad = len(lista)
    suma = sum(lista)
    return suma / cantidad
if __name__ == "__main__":
#imprime el promedio
    promedio = calcular_promedio(lista)
print("el promedio de el arreglo de reales es: " +str(promedio))
```

2. Desarrollar un algoritmo que calcule el producto punto de dos arreglos de números enteros (reales) de igual tamaño.

```pseudocode
#dos arreglos de enteros reales con 4 componentes 
lista1:float = [2, 6, 8, 3]
lista2:float = [4, 7, 1, 5]
#funcion para calcular el producto punto de los dos arreglos
def calcular_producto_punto(lista1:float, lista2:float) -> float:
    producto_punto = 0
    for i in range(0, len(lista1)):
        producto_punto += lista1[i] * lista2[i]
    return producto_punto
if __name__ == "__main__":
#imprime el producto punto 
    producto_punto:float = calcular_producto_punto(lista1, lista2)
print("el producto punto de los dos arreglos es: " + str(producto_punto))
```

3. Hacer un algoritmo que deje al final de un arreglo de números todos los ceros que aparezcan en dicho arreglo.

```pseudocode
lista = [11, 16, 23, 20, 0, 15, 0, 50, 0, 17] #lista con arreglo denumeros enteros
def mover_ceros_al_final(lista) -> int:
    #cree dos listas vacias para ir agregando los numeros ceros o diferentes de cero
    diferentes_de_cero = []
    ceros = []
    for n in lista:
        if n != 0:
            #use append para para agregar los numeros a la lista si cumple con la condicion dada
            diferentes_de_cero.append(n) 
        else:
            ceros.append(n)
    return diferentes_de_cero + ceros
if __name__ == "__main__":
#imprime el resultado
    resultado = mover_ceros_al_final(lista)
print(resultado)
```
4. Revisar que son los algoritmos de sorting, entender bubble-sort (enlace a implementación).

* Los algoritmos de ordenamiento, también conocidos como algoritmos de sorting, son procedimientos que organizan elementos en una secuencia particular, generalmente en orden ascendente o descendente. Estos algoritmos son fundamentales en la informática y la ciencia de la computación, ya que se utilizan en una amplia variedad de aplicaciones, desde bases de datos hasta búsqueda y clasificación de datos.
* Bubble Sort (Ordenamiento de Burbuja) es un algoritmo simple que funciona comparando elementos adyacentes en una lista y, si están en el orden incorrecto, los intercambia. Este proceso se repite hasta que toda la lista esté ordenada. Aunque es fácil de entender e implementar, su eficiencia es baja en comparación con otros algoritmos de ordenamiento, lo que lo hace poco adecuado para listas grandes. Su complejidad temporal promedio y en el peor de los casos son altas, lo que significa que requiere más tiempo para ordenar listas de tamaño considerable. Por lo tanto, Bubble Sort no es una elección eficiente para aplicaciones que manejan grandes conjuntos de datos.
