# Análisis de datos con Numpy, Panda y Matplotlib

# ¿Qué es Data Analysis o el Análisis de datos?

Es el proceso de inspección, limpieza de datos, transformación de datos con el objetivo de descubrir datos útiles y
ayude al soporte de toma de decisiones.

# ¿Qué pasos tenemos que dar para realizar un análisis exploratorio de datos?

1. Transformar los datos como llegan al formato que necesito
2. Limpieza de datos (preprocesado de la información)
3. Visualización de los datos
4. Preparar el modelo de datos
5. Realizar un análisis aprendizaje automático

# Numpy. Pero ¿Qué es Numpy?

Numpy, es un paquete para realizar computación científica y operaciones y cálculos.

## Estructuras Array Numpy

#### Ejercicio 1: Crea un array de una dimensión. (Vector)

```python
vector = np.arange(5)
print(vector)
```

#### Ejercicio 2: Crea un array de dos dimensiones. (Array)

```python
matriz = np.arange(4).reshape(2,2)
print(matriz)
```

#### Ejercicio 3: Crea un vector y un array a partir de la siguiente lista
[1,11,111,1111]

*pista tienes que crear una lista y utilizar np.array()*

``` python
lista = [1, 11, 111, 1111]
vector = np.array(lista)
array = np.array([lista])

print(vector)
print(array)
```

#### Ejercicio 4: Crea un array 5x5 de zeros
``` python
zero = np.zeros([5,5])
print(zero)
```

#### Ejercicio 5: Crea un vector cuyo límite inferior sea 0 y el límite superior sea 20 y tenga 5 elementos comprendidos en ese intervalo que sean liealmente iguales

 ```python
pasos = np.linspace(start=0, stop=20, num=5)
print(pasos)
```

#### Ejercicio 6: Crea un array de 8 elementos de 2x2x2 de ceros (Tensor)

```python
tensor = np.zeros((2,2,2))
print(tensor)
```

####  Ejercicio 7: Crea un array que vaya de 2 al 20 y obten el elememnto de la posición 7


```python
seven = np.arange(2,20)
print(seven[7])
#Este codigo crea un array de veinte elementos y luego imprime tpdps los elementos de ese array partiendo de la posicion 2 en adelante
```

#### Ejercicio 8: crea un vector de 20 elementos y mediante el método slice() crea otro vector a partir del vector de 20 elementos que empiece en 1, termine en 10 y tenga los números de dos en dos

``` python

```

#### Ejercicio 9: Explica el siguiente código:

``` python
arr7 = np.arange(20)
print(arr7[2:])
```

Escribe aquí tu explicación:

#### Ejercicio 10: Utilizando lo anterior a partir del arr7 quiero obtener una lista que va de 0 a 15

``` python

```
#### Ejercicio 11: Crea un array de ceros de 3x3. A partir de ese array prueba el atributo shape, ndim, y itemsize. Explica que nos dicen estos atributos sobre la estructura


# LEER Y ESCRIBIR EN FICHEROS

descarga el siguiente fichero que es una base de datos de huracanes

https://github.com/rmcelreath/rethinking/blob/master/data/Hurricanes.csv

```python
arr_csv = np.genfromtxt('./Hurricanes.csv', delimiter = ',')
np.savetxt('newfilex.csv', arr_csv, delimiter = ',')
```

Explcia que hace este código

