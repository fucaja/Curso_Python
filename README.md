# Python Curse

Python es un lenguaje de **proposito general**, de **alto nivel** (se puede leer sin dificultad)  y fácil de entender. Además, Python es de **Tipado dinámico** ya que no necesitamos poner qué tipo de dato es el que estamos agregegando. 

```python
nombre = "nombre"
edad = 20
```
## Ventajas


- **Proposito general**
- **Alto nivel**
- **Fácil de aprender**
- **Tipado dinámico**
- **Orientado a Objetos**
- **Lenguaje interpretado**
- **Comunidad grande**

## Utilidad

- **Desarrollo web** con Flask y Django
- **Aplicaciones moviles**
- **Aplicaciones escritorio**
- **Automatización de scripts**
- **Ciencia de datos**
- **Machine Learning**
- **Desarrollo de software**
- **Automatización de pruebas de software**
- **Desarrollo de juegos**
- **Hacking**




## Conceptos básicos

### Tipos de datos

```python
string = "string"
string = 'string'
string = """string
            string"""
string = '''string
            string'''
            
int = 1

float = 1.0

bool = True
bool = False
```

### Variables

Las variables son etiquetas que le asignamos a un valor ya sea string, int, float o bool

```python
nombre = "Jose"
edad = 28
sexo = "Masculino"
```

Existen dos maneras para definir varibles

```python
# Variable camelCase
nombreCompleto = "Jose Fuentes"
# Variable snake_case (RECOMENDADO)
nombre_completo = "Jose Fuentes"
```

La manera recomendada por python es **snake_case** con **_**.


### Print

```python
nombre = "José"
apellido = " Fuentes"
nombre_completo = nombre + apellido
edad = 28
print(nombre + apellido + str(edad))

# Concatenar f string
print(f"Hola {nombre_completo} tu edad es + {edad}")
# Concatenar con +
print(nombre + " " + apellido + str(edad))
```




## Operadores aritmétricos

```python

# suma y resta (+ y -)
suma = 1 + 2
resta = 3 - 2

# multiplicación (* y /)
multip = 2 * 3
division = 1000 / 100 # regresa float

# potenciación o exponenete (**)
exponente = 2 ** 2

# división baja (//) 
division_baja = 12 // 5 # regresa un int 2.4 = 2

# Módulo o resto de la división
resto = 12 % 5

print("suma 1 + 2: ", suma)
print("resta 3 - 2: ", resta)
print("multip 2 * 3: ", multip)
print("division 1000 / 100: ", division)
print("exponente 2 ** 2: ", exponente)
print("division_baja 12 // 5: ", division_baja)
print("resto 12 % 5: ", resto)
```

### Operador de comparación

Cada uno de los operadores regresará como resultado un valor booleano True o False.

- **==** es igual que
- **!=** es distinto de
- **<** es menor que
- **<=** es menor o igual que
- **\>** es mayor que  
- **\>=** esmayor o igual que

### Operadores lógicos
```python
# AND 
resultado1 = True & True  # True 
resultado2 = False & True  # False
resultado3 = True & False  # False
resultado4 = False & False  # False

# OR
resultado5 = True | True  # True 
resultado6 = False | True  # True
resultado7 = True | False  # True
resultado8 = False | False  # False

#NOT
resultado9 = not True  # False 
resultado10 = not False  # True
```
 
### Condicionales

```python
ingreso_mensual = 1000001

if ingreso_mensual > 100000:
    print("Ingreso alto")
elif ingreso_mensual > 50000 and ingreso_mensual <= 100000:
    print("Ingreso medio")
else:
    print("ingreso bajo")

```

### Métodos de cadenas

Todos los métodos son funciones pero no todas las funciones son métodos
Los métodos son funciones específicas de objetos

Función **dir(variable)** devuelve la lista de atributos válidos del objeto

``` python
cadena1 = "Hola soy python"
print(dir(cadena1))

['__add__', '__class__', '__contains__', '__delattr__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__getitem__', '__getnewargs__', '__getstate__', '__gt__', '__hash__', '__init__', '__init_subclass__', '__iter__', '__le__', '__len__', '__lt__', '__mod__', '__mul__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__rmod__', '__rmul__', '__setattr__', '__sizeof__', '__str__', '__subclasshook__', 'capitalize', 'casefold', 'center', 'count', 'encode', 'endswith', 'expandtabs', 'find', 'format', 'format_map', 'index', 'isalnum', 'isalpha', 'isascii', 'isdecimal', 'isdigit', 'isidentifier', 'islower', 'isnumeric', 'isprintable', 'isspace', 'istitle', 'isupper', 'join', 'ljust', 'lower', 'lstrip', 'maketrans', 'partition', 'removeprefix', 'removesuffix', 'replace', 'rfind', 'rindex', 'rjust', 'rpartition', 'rsplit', 'rstrip', 'split', 'splitlines', 'startswith', 'strip', 'swapcase', 'title', 'translate', 'upper', 'zfill']

``` 
Métodos

- **variable.upper()** Convierte a mayusculas
- **variable.lower()** Convierte en minisculas
- **variable.capitalize()** Convierte solo la primera en mayuscula

``` python

"""

cadena1 = "bienvenido"

print(cadena1.upper()) # bienvenido
print(cadena1.lower()) # BIENVENIDO
print(cadena1.capitalize()) # Bienvenido
```

- **variable.find("")** Devuelve la posición iniciar donde encuentra el valor y -1 cuando no encuentra el valor
- **variable.index("")** Devuelve la posición iniciar donde encuentra el valor y ERROR cuando no encuentra el valor

```python
print("Hola a todos".find("a")) # 3
print("Hola a todos".index("a")) # 3
```

- **variable.isnumeric()** Devuelve True o False si es numérico
- **variable.isalpha()** Devuelve True o False si es alfanumérico o solo letras (Regresa False si tiene espacios)

```python
print(cadena1.isnumeric()) # False
print(cadena1.isalpha()) # True
```

- **variable.count("")** Devuelve las coincidencias dentro del texto
    len(variable) Devuelve el tamaño de una cadena

```python
print("Hola a todos".count("a")) # 2
print(len("Hola")) # 4
```


- **variable.startswith("")** Verifica si una cadena empieza con ""
- **variable.endswith("")** Verifica si una cadena termina con ""

```python
print("Hola".startswith("H")) # True
print("Hola".endswith("a")) # True
```

- **variable.replace(buscar,remplazar)** Remplaza los valores que encuentra
- **variable.split()** Separa todo por espacio
- **variable.split(",")** Separa todo por coma

```python
print("Todo va bien".replace("bien","mal")) # Hola todo va mal
print("hola, hola".split()) # ['hola,', 'hola']
print("hola, hola".split(", ")) # ['hola', 'hola']
```


### Métodos de listas

#### Para Listas

- **lista([var,...,var])** Crea una lista
- **len(lista)** Cuenta la cantidad de elementos
- **lista.append(valor)** Agrega un elemento
- **lista.insert(ind,valor)**  Agrega un elemento en un indice especificado
- **lista.extend([valor1,..., valorN])** Agrega varios elementos 
- **lista.pop(indice)** Eliminando un elemento por indice
- **lista.remove("")** Eliminando un elmento por su valor 
- **lista.sort()** Ordena números y boleanos de manera ascendente
- **lista.sort(reverse = True)** Ordena números y boleanos de manera descendente
- **lista.reverse()** Invierte el orden de la lista [1,2,3,4] = [4,3,2,1]
- **lista.clear()** Elimina todos los elementos

```python
lista = list(["Hola", 1 ,True])
print(lista)
print(len(lista))

lista.append("bien")
print(lista)

lista.insert(3, "mal")
print(lista)

lista.extend([True, 5])
print(lista)

lista.pop(0)
print(lista)

lista.remove("mal")
print(lista)

lista = list([95,25,33,74,True, False])
lista.sort()
print(lista)
lista.sort(reverse= True)
print(lista)

lista = list([95,25,33,74,True, False])
lista.reverse()
print(lista)

lista.clear()
print(lista)
```
```python

['Hola', 1, True]
3
['Hola', 1, True, 'bien']
['Hola', 1, True, 'mal', 'bien']
['Hola', 1, True, 'mal', 'bien', True, 5]
[1, True, 'mal', 'bien', True, 5]
[1, True, 'bien', True, 5]
[False, True, 25, 33, 74, 95]
[95, 74, 33, 25, True, False]
[False, True, 74, 33, 25, 95]
[]
```

#### Para Tuplas

- **tupla.count(valor)** Busca los elementos con el mismo valor y cuenta el número de repeticiones
- **tupla.index(valor)** Regresa la posición del elemento buscado

```python
tupla = (1,2,3,4, "hola",1,1,1)

print(dir(tupla))
print(tupla.count(1))
print(tupla.index("hola"))
```
```python
['__add__', '__class__', '__class_getitem__', '__contains__', '__delattr__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__getitem__', '__getnewargs__', '__getstate__', '__gt__', '__hash__', '__init__', '__init_subclass__', '__iter__', '__le__', '__len__', '__lt__', '__mul__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__rmul__', '__setattr__', '__sizeof__', '__str__', '__subclasshook__', 'count', 'index']
4
4
```

#### Para Conjuntos set

- **add:** Agregar un elemento al conjunto.
- **clear:** Eliminar todos los elementos del conjunto.
- **copy:** Crear una copia del conjunto.
- **difference:** Obtener la diferencia entre dos conjuntos.
- **difference_update:** Actualizar el conjunto restando elementos de otro conjunto.
- **discard:** Eliminar un elemento específico del conjunto si está presente.
- **intersection:** Obtener la intersección entre dos conjuntos.
- **intersection_update:** Actualizar el conjunto manteniendo solo los elementos comunes.
- **isdisjoint:** Verificar si dos conjuntos son disjuntos (no tienen elementos en común).
- **issubset:** Verificar si un conjunto es subconjunto de otro.
- **issuperset:** Verificar si un conjunto es superconjunto de otro.
- **pop:** Eliminar y devolver un elemento arbitrario del conjunto.
- **remove:** Eliminar un elemento específico del conjunto.
- **symmetric_difference:** Obtener la diferencia simétrica entre dos conjuntos.
- **symmetric_difference_update:** Actualizar el conjunto con su diferencia simétrica.
- **union:** Obtener la unión de dos conjuntos.
- **update:** Agregar elementos de otro conjunto al conjunto actual.

```python
conj_set = {1, 2, 3, 4, "hola"}

# add: Agregar un elemento al conjunto.
conj_set.add(5)
print("Conjunto después de agregar 5:", conj_set)

# copy: Crear una copia del conjunto.
conjunto_copia = conj_set.copy()
print("Copia del conjunto:", conjunto_copia)

# difference: Obtener la diferencia entre dos conjuntos.
otro_conjunto = {3, 4, 5, 6}
diferencia = conj_set.difference(otro_conjunto)
print("Diferencia entre conjuntos:", diferencia)

# difference_update: Actualizar el conjunto restando elementos de otro conjunto.
conj_set.difference_update(otro_conjunto)
print("Conjunto después de difference_update:", conj_set)

# discard: Eliminar un elemento específico del conjunto si está presente.
conj_set.discard(3)
print("Conjunto después de descartar 3:", conj_set)

# intersection: Obtener la intersección entre dos conjuntos.
conjunto_interseccion = conj_set.intersection(otro_conjunto)
print("Intersección entre conjuntos:", conjunto_interseccion)

# intersection_update: Actualizar el conjunto manteniendo solo los elementos comunes.
conj_set.intersection_update(otro_conjunto)
print("Conjunto después de intersection_update:", conj_set)

# isdisjoint: Verificar si dos conjuntos son disjuntos (no tienen elementos en común).
son_disjuntos = conj_set.isdisjoint(otro_conjunto)
print("¿Los conjuntos son disjuntos?:", son_disjuntos)

# issubset: Verificar si un conjunto es subconjunto de otro.
es_subconjunto = conj_set.issubset(otro_conjunto)
print("¿El conjunto es subconjunto?:", es_subconjunto)

# issuperset: Verificar si un conjunto es superconjunto de otro.
es_superconjunto = conj_set.issuperset(otro_conjunto)
print("¿El conjunto es superconjunto?:", es_superconjunto)

conj_set = {3, 4, 5, 6, 1,2,3,4,5,6,7}
# pop: Eliminar y devolver un elemento arbitrario del conjunto.
elemento_eliminado = conj_set.pop()
print("Elemento eliminado con pop:", elemento_eliminado)

# remove: Eliminar un elemento específico del conjunto.
conj_set.remove(3)
print("Conjunto después de remover 3:", conj_set)

# symmetric_difference: Obtener la diferencia simétrica entre dos conjuntos.
diferencia_simetrica = conj_set.symmetric_difference(otro_conjunto)
print("Diferencia simétrica entre conjuntos:", diferencia_simetrica)

# symmetric_difference_update: Actualizar el conjunto con su diferencia simétrica.
conj_set.symmetric_difference_update(otro_conjunto)
print("Conjunto después de symmetric_difference_update:", conj_set)

# union: Obtener la unión de dos conjuntos.
union_conjuntos = conj_set.union(otro_conjunto)
print("Unión de conjuntos:", union_conjuntos)

# update: Agregar elementos de otro conjunto al conjunto actual.
conj_set.update(otro_conjunto)
print("Conjunto después de update:", conj_set)

# clear: Eliminar todos los elementos del conjunto.
conj_set.clear()
print("Conjunto después de clear:", conj_set)
```

```python
Conjunto después de agregar 5: {1, 2, 3, 4, 5, 'hola'}
Copia del conjunto: {1, 2, 3, 4, 5, 'hola'}
Diferencia entre conjuntos: {1, 2, 'hola'}
Conjunto después de difference_update: {1, 2, 'hola'}
Conjunto después de descartar 3: {1, 2, 'hola'}
Intersección entre conjuntos: set()
Conjunto después de intersection_update: set()
¿Los conjuntos son disjuntos?: True
¿El conjunto es subconjunto?: True
¿El conjunto es superconjunto?: False
Elemento eliminado con pop: 1
Conjunto después de remover 3: {2, 4, 5, 6, 7}
Diferencia simétrica entre conjuntos: {2, 3, 7}
Conjunto después de symmetric_difference_update: {2, 3, 7}
Unión de conjuntos: {2, 3, 4, 5, 6, 7}
Conjunto después de update: {2, 3, 4, 5, 6, 7}
Conjunto después de clear: set()
```

#### Para diccionarios

 - **clear:** Eliminar todos los elementos del diccionario
 - **copy:** Crear una copia del diccionario
 - **fromkeys:** Crear un nuevo diccionario con claves especificadas y un valor predeterminado
 - **get:** Obtener el valor asociado con una clave (manejo seguro para evitar errores si la clave no existe)
 - **items:** Obtener una vista de los pares clave-valor en el diccionario
 - **keys:** Obtener una vista de las claves en el diccionario
 - **pop:** Eliminar y obtener el valor asociado con una clave
 - **popitem:** Eliminar y obtener un par clave-valor arbitrario del diccionario
 - **setdefault:** Obtener el valor asociado con una clave; si la clave no existe, se agrega al diccionario con un valor predeterminado
 - **update:** Actualizar el diccionario con pares clave-valor de otro diccionario
 - **values:** Obtener una vista de los valores en el diccionario

```python
# Diccionario inicial
diccionario = {
    'nombre': "Jose",
    'apellido': "Fuentes",
    'edad': 28
}

# Imprimir directorio del diccionario definido
print("Directorio del diccionario definido:", dir(diccionario))

# copy: Crear una copia del diccionario
diccionario_copia = diccionario.copy()
print("Copia del diccionario:", diccionario_copia)

# fromkeys: Crear un nuevo diccionario con claves especificadas y un valor predeterminado
nuevo_diccionario = dict.fromkeys(['nombre', 'apellido', 'edad'], "Valor Predeterminado")
print("Nuevo diccionario creado con fromkeys:", nuevo_diccionario)

# get: Obtener el valor asociado con una clave (manejo seguro para evitar errores si la clave no existe)
valor_edad = diccionario.get('edad', "Clave no encontrada")
print("Valor de 'edad':", valor_edad)

# items: Obtener una vista de los pares clave-valor en el diccionario
vista_items = diccionario.items()
print("Vista de items:", vista_items)

# keys: Obtener una vista de las claves en el diccionario
vista_claves = diccionario.keys()
print("Vista de claves:", vista_claves)

# pop: Eliminar y obtener el valor asociado con una clave
valor_apellido = diccionario.pop('apellido')
print("Valor eliminado con pop ('apellido'):", valor_apellido)

# popitem: Eliminar y obtener un par clave-valor arbitrario del diccionario
par_arbitrario = diccionario.popitem()
print("Par arbitrario eliminado con popitem:", par_arbitrario)

# setdefault: Obtener el valor asociado con una clave; si la clave no existe, se agrega al diccionario con un valor predeterminado
valor_nombre = diccionario.setdefault('nombre', "Valor Predeterminado")
print("Valor de 'nombre' después de setdefault:", valor_nombre)

# update: Actualizar el diccionario con pares clave-valor de otro diccionario
diccionario.update({'ubicacion': 'Ciudad X', 'ocupacion': 'Programador'})
print("Diccionario después de update:", diccionario)

# values: Obtener una vista de los valores en el diccionario
vista_valores = diccionario.values()
print("Vista de valores:", vista_valores)

# clear: Eliminar todos los elementos del diccionario
diccionario.clear()
print("Diccionario después de clear:", diccionario)
```

```python
Directorio del diccionario definido: ['__class__', '__class_getitem__', '__contains__', '__delattr__', '__delitem__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__getitem__', '__getstate__', '__gt__', '__hash__', '__init__', '__init_subclass__', '__ior__', '__iter__', '__le__', '__len__', '__lt__', '__ne__', '__new__', '__or__', '__reduce__', '__reduce_ex__', '__repr__', '__reversed__', '__ror__', '__setattr__', '__setitem__', '__sizeof__', '__str__', '__subclasshook__', 'clear', 'copy', 'fromkeys', 'get', 'items', 'keys', 'pop', 'popitem', 'setdefault', 'update', 'values']
Copia del diccionario: {'nombre': 'Jose', 'apellido': 'Fuentes', 'edad': 28}
Nuevo diccionario creado con fromkeys: {'nombre': 'Valor Predeterminado', 'apellido': 'Valor Predeterminado', 'edad': 'Valor Predeterminado'}
Valor de 'edad': 28
Vista de items: dict_items([('nombre', 'Jose'), ('apellido', 'Fuentes'), ('edad', 28)])
Vista de claves: dict_keys(['nombre', 'apellido', 'edad'])
Valor eliminado con pop ('apellido'): Fuentes
Par arbitrario eliminado con popitem: ('edad', 28)
Valor de 'nombre' después de setdefault: Jose
Diccionario después de update: {'nombre': 'Jose', 'ubicacion': 'Ciudad X', 'ocupacion': 'Programador'}
Vista de valores: dict_values(['Jose', 'Ciudad X', 'Programador'])
Diccionario después de clear: {}






