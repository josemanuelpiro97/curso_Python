# Tarea_Integradora_2

---

## 1)

- Genere una lista (llamada "A") de la cantidad de elementos que ustedes quieran (UTILICE LA LIBRERÍA NUMPY).
- Realice una función que acomode los valores de esta lista de manera descendiente, o de manera ascendente dependiendo de un parámetro "flag" que indicara cual de los dos ordenamientos realizar
- Genere una lista (llamada "B") de la misma cantidad de elementos que "A", pero estos elementos deberán ser aleatorios (no utilice random, busque resolverlo con numpy)
- Luego de tener los dos arreglos generados, realice una función que reciba estas dos listas como parámetros de entrada. Esta función deberá recorrer las dos listas que recibe revisando que valores contiene dentro, y luego en una nueva lista (llamada "C") ira aumentando en 1 cada ves que encuentre un valor equivalente al index que aumentara. Por ultimo retorne esta lista generada
  - Ej: si la lista A = [1,3,3,6] y B=[1,1,2,2] entonces C=[0,3,2,2,0,0,1]

- Con esta lista "C" realice un gráfico de barras que refleje las veces que se han repetido los valores en A y B.

---

## 2) (para este punto use la libreria pandas)

- Cree una tabla de 3 columnas por 10 filas
- Ingrese por teclado 3 títulos para el cabecera de las 3 columnas
- Luego realice una función que reciba dicha tabla y que rellene las 3 columnas con valores aleatorios (de entre 3 y 17). Por ultimo retorne la tabla rellenada
- Luego realice una función que reciba esta tabla rellenada y en aquellos lugares donde el numero es mayor a 9 reemplace los valores por la palabra "null"
- Por ultimo realice una función que reciba la tabla con los valores modificados , un flag que puede ser (1,2 o 3) y un tercer valor llamado "buscado".
  - si el flag es 1 la función deberá retornar la cantidad de nulls en la tabla
  - si el flag es 2 la función deberá retornar la suma total de los valores dentro de la tabla
  - si el flag es 3 la función tendrá en cuenta el ultimo parámetro("buscado") y retornara la cantidad de este numero que se encuentre en la tabla.
