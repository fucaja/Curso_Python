# Curso de Python

Python es un lenguaje de programación de **propósito general** que se destaca por su legibilidad y facilidad de aprendizaje. Algunas de sus características distintivas son su **tipado dinámico, orientación a objetos y su naturaleza interpretada**. Estas características hacen que Python sea una elección popular para una amplia variedad de aplicaciones.

```python
#Ejemplo de tipado dinámico
nombre = "nombre"
edad = 20
```
## Ventajas


- **Proposito general**: Python es versátil y se utiliza en una amplia gama de campos, desde desarrollo web hasta ciencia de datos y machine learning.
- **Alto nivel**: Al ser de alto nivel, Python permite a los programadores expresar ideas en menos líneas de código, lo que facilita la lectura y el mantenimiento.
- **Fácil de aprender**: La sintaxis simple y clara de Python facilita la entrada a la programación para principiantes, pero también es poderosa y flexible para desarrolladores más experimentados.
- **Tipado dinámico**: No es necesario declarar el tipo de variable al principio; Python infiere automáticamente el tipo de datos, lo que hace que el código sea más flexible y fácil de escribir.
- **Orientado a Objetos**: Python admite programación orientada a objetos, facilitando la organización y estructuración del código.
- **Lenguaje interpretado**: El código Python se ejecuta línea por línea, facilitando la detección de errores y permitiendo una rápida prueba y depuración.
- **Comunidad grande**: Python cuenta con una comunidad activa y solidaria que proporciona recursos, bibliotecas y soporte, lo que facilita la resolución de problemas y el aprendizaje continuo.

## Desventajas

- **Rendimiento Relativo**: Comparado con lenguajes de bajo nivel como C++ o Rust, Python puede ser más lento en términos de ejecución, especialmente en aplicaciones que requieren un alto rendimiento computacional.
- **Gestión de Memoria**: Python utiliza un recolector de basura para gestionar la memoria automáticamente, lo que puede resultar en cierta pérdida de control sobre la gestión de la memoria en comparación con lenguajes de bajo nivel.
- **Menos Adecuado para Aplicaciones Móviles Nativas**: Aunque existen soluciones para el desarrollo móvil con Python, no es tan común o eficiente como otros lenguajes diseñados específicamente para este propósito.
- **Interpretación vs Compilación**: Python es un lenguaje interpretado, lo que puede afectar su rendimiento en comparación con lenguajes compilados, especialmente en aplicaciones que requieren alta velocidad de ejecución.
- **Tamaño del Ecosistema para Desarrollo de Juegos**: Aunque Python se utiliza en el desarrollo de juegos, su presencia no es tan fuerte como en otros lenguajes como C++ en este ámbito, especialmente en juegos de alta gama.
- **Compatibilidad con Versiones**: La transición entre versiones principales de Python (por ejemplo, de Python 2 a Python 3) puede generar problemas de compatibilidad en el código existente.
- **Recursos Limitados para Desarrollo Empotrado**: En comparación con lenguajes como C o C++, Python puede no ser la elección más adecuada para el desarrollo de sistemas embebidos debido a su consumo de recursos.
- **Gestión de Hilos y Concurrencia**: Aunque Python admite hilos, su capacidad para manejar concurrencia puede no ser tan eficiente como en algunos lenguajes diseñados específicamente para este propósito.
- **Falta de Soporte para Desarrollo de Aplicaciones de Tiempo Real**: En comparación con algunos lenguajes diseñados para aplicaciones de tiempo real, Python puede no ser la opción más óptima en términos de predictibilidad y gestión de tiempos estrictos.


## Utilidad

- **Desarrollo web**: Python es ampliamente utilizado para desarrollar aplicaciones web, con frameworks como Flask y Django que simplifican el proceso.
- **Aplicaciones moviles**: A través de frameworks como Kivy o BeeWare, Python se puede utilizar para el desarrollo de aplicaciones móviles.
- **Aplicaciones escritorio**: Con herramientas como Tkinter o PyQt, Python se utiliza para crear aplicaciones de escritorio con interfaces gráficas de usuario (GUI).
- **Automatización de scripts**: Python es ideal para escribir scripts que automatizan tareas repetitivas y simplifican procesos.
- **Ciencia de datos y Machine Learning**: Con bibliotecas como NumPy, pandas y scikit-learn, Python es esencial en el ámbito de la ciencia de datos y machine learning.
- **Desarrollo de software**: Python es utilizado para desarrollar una amplia variedad de software, desde pequeñas herramientas hasta sistemas complejos.
- **Automatización de pruebas de software**: Frameworks como Selenium y Pytest permiten la automatización eficiente de pruebas de software.
- **Desarrollo de juegos**: Aunque no es tan común como en otros lenguajes, Python se utiliza en el desarrollo de juegos, especialmente para prototipos y juegos 2D.
- **Hacking**: Python es una opción popular en el campo de la seguridad informática y el hacking ético debido a su sintaxis clara y a las herramientas disponibles.



# 1 Conceptos básicos

## Tipos de datos

```python
# Cadena de texto (String) - Se puede definir usando comillas simples, dobles o triples
string_single = 'string con comillas simples'
string_double = "string con comillas dobles"
string_triple_double = """string
                        en múltiples líneas
                        con comillas dobles"""
string_triple_single = '''string
                        en múltiples líneas
                        con comillas simples'''

# Número entero (Integer)
integer = 1

# Número decimal (Float)
floating_point = 1.0

# Booleano (Boolean)
boolean_true = True
boolean_false = False
```

## Definir variables


Las variables en Python son **etiquetas** que asignamos a valores, ya sean de tipo string, int, float o bool. Sirven para almacenar y referenciar información dentro de un programa. Aquí tienes un ejemplo:

```python
nombre = "Jose"
edad = 28
sexo = "Masculino"
```

Ahora, al hablar sobre las dos maneras de definir variables en Python, podemos utilizar:

**Camel Case**: En Camel Case, la primera letra de cada palabra, excepto la primera, se escribe en mayúscula. Aunque es aceptable en Python, no es la convención más comúnmente usada.

```python
nombreCompleto = "Jose Fuentes"
```

**Snake Case (Recomendado)**: En Snake Case, las palabras se escriben en minúsculas y se separan por guiones bajos **_**. Este estilo es ampliamente recomendado por la PEP 8, la guía de estilo para código en Python. Es más legible y preferido en la comunidad Python.

```python
nombre_completo = "Jose Fuentes"
```

La elección entre Camel Case y Snake Case no solo se trata de preferencias estilísticas, sino también de seguir las convenciones de la comunidad para facilitar la colaboración y la lectura del código. En Python, la recomendación general es utilizar Snake Case para nombrar variables.


### Eliminar variable

Si queremos limpiar de memoria la variable despues de utlizarla podemos utilizar el comando **del**.

```python
del variable
```

### Asignar nuevo valor

```python
variable = None  # Asignar un nuevo valor (puede ser None u otro valor)
```


Si queremos asignar un nuevo valor lo podemos realizar mediante un variable = None
cantidad = None  # Asignar un nuevo valor (puede ser None u otro valor)

### Imprimir variables


```python
# Definición de variables
nombre = "José"
apellido = " Fuentes"
edad = 28

# Concatenación con el operador '+'
nombre_completo = nombre + apellido

# Imprimir el nombre, apellido y edad concatenados
print("1. Concatenación con '+' (sin espacio):", nombre + apellido + " " + str(edad))

# Concatenación con f-string
mensaje_fstring = f"Hola {nombre_completo}, tu edad es {edad}"
print("2. Concatenación con f-string:", mensaje_fstring)

# Concatenación con el operador '+' y espacio adicional
mensaje_con_espacio = nombre + " " + apellido + " " + str(edad)
print("3. Concatenación con '+' (con espacio):", mensaje_con_espacio)
```

# 2 Variables compuestas

## Listas

Una lista es una estructura de datos que se utiliza para almacenar una colección ordenada de elementos. Estos elementos pueden ser de cualquier tipo, como números, cadenas de texto, booleanos, otras listas, entre otros. **La lista es un tipo de dato mutable**, lo que significa que se pueden modificar después de su creación.

Características clave de las listas en Python:

- **Ordenadas:** Los elementos de la lista están ordenados y se accede a ellos mediante un índice. El primer elemento tiene índice 0, el segundo índice 1, y así sucesivamente.

- **Mutables:** Puedes cambiar, agregar o eliminar elementos de una lista después de su creación.

- **Pueden contener diferentes tipos de datos:** Una lista puede contener elementos de diferentes tipos, como enteros, cadenas de texto, booleanos, e incluso otras listas u objetos más complejos.

- **Soportan operaciones y métodos:** Las listas en Python ofrecen una variedad de operaciones y métodos que facilitan la manipulación de los datos almacenados en ellas, como agregar elementos, eliminar elementos, obtener la longitud, invertir el orden, entre otros.

```python
# Maneras de como definir una lista
lista1 = [1, "dos", 3.0, True]

#Usando la Función list():
lista2 = list([1, 2, 3, 4, 5])

#Lista Vacía:
lista_vacia = []

#Usando un for
numeros = [x for x in range(1, 6)]

#Usando el Método append():
lista = []
lista.append(1)
lista.append(2)
lista.append(3)

#Usando el Método extend():
lista = [1, 2, 3]
lista.extend([4, 5, 6])

#Usando la Función list() con Otra Secuencia (por ejemplo, una Tupla):
tupla = (1, 2, 3)
lista_desde_tupla = list(tupla)

#Usando el Método split() con una Cadena de Texto:
cadena = "a b c"
lista_desde_cadena = cadena.split()

#Usando Repetición:
lista_repetida = [0] * 5  # Crea una lista con cinco elementos 0


# Imprimiendo los datos
lista_datos = ["Jose", "Alberto", 28]

# Desempaquetado de datos
nombre, apellido, edad = lista_datos

# Impresión de datos de la lista
print(f"Lista de Datos: Nombre: {nombre} {apellido} y Edad: {edad}")

# Acceso a elementos de la lista con bucle for
print("Acceso a elementos con bucle for:")
for dato in lista_datos:
    print(dato)
```

## Tuplas


Una tupla es una estructura de datos que permite almacenar un conjunto ordenado e inmutable de elementos. Las tuplas son similares a las listas, pero tienen algunas diferencias clave:

- **Inmutabilidad:** Una tupla no puede ser modificada después de su creación. Esto significa que no puedes agregar, eliminar o cambiar elementos en una tupla una vez que ha sido creada. En contraste, las listas son mutables.

- **Sintaxis:** Las tuplas se definen utilizando paréntesis () o, en el caso de las tuplas vacías, simplemente con paréntesis vacíos. Por ejemplo, (1, 2, 3) o ().

- **Tamaño fijo:** El tamaño de una tupla es fijo después de su creación. No puedes cambiar la longitud de una tupla añadiendo o eliminando elementos.

- **Indexación:** Al igual que las listas, las tuplas son indexadas, lo que significa que puedes acceder a sus elementos utilizando índices.

- **Heterogeneidad:** Una tupla puede contener elementos de diferentes tipos (por ejemplo, números, cadenas, booleanos, otras tuplas, etc.).

```python
#Usando paréntesis:
tupla1 = ('cadena', 14, 3.14, True)

#Sin paréntesis (Empaquetado de Tupla):
tupla2 = 4, 5, 6

#Con un solo elemento (debe tener una coma al final):
tupla3 = (7,)

#Construcción de tuplas mediante la función tuple():
lista = [8, 9, 10]
tupla4 = tuple(lista)

#Usando la función zip() para combinar iterables:
nombres = ('Alice', 'Bob', 'Charlie')
edades = (25, 30, 22)
tupla5 = tuple(zip(nombres, edades))

#Desempaquetado de Tupla:
tupla6 = 11, 12, 13
a, b, c = tupla6  # Desempaquetado

#Creación de una tupla vacía:
tupla_vacia = ()

#Creación de una tupla con el constructor tuple():
tupla_construida = tuple()

#Usando comprensiones de tuplas:
tupla_comprension = tuple(x for x in range(5))


#Imprimir tuplas
mi_tupla = (1, 'dos', 3.0, True)

print("Tupla completa:", mi_tupla)

print("Primer elemento:", mi_tupla[0])
print("Segundo elemento:", mi_tupla[1])
print("Tercer elemento:", mi_tupla[2])
print("Cuarto elemento:", mi_tupla[3])

# Iterar sobre los elementos de la tupla e imprimirlos
print("Iterar e imprimir:")
for elemento in mi_tupla:
    print(elemento)
```

## Conjuntos

Los conjuntos son una colección desordenada y sin duplicados de elementos. Se definen utilizando llaves {} o la función set(). Los conjuntos en Python son similares a los conjuntos en matemáticas y proporcionan operaciones comunes de conjuntos como unión, intersección y diferencia.

- **Elementos Únicos:** Los conjuntos no pueden contener elementos duplicados. Si intentas agregar un elemento que ya está presente, el conjunto no cambiará.

- **Desordenados:** Los elementos en un conjunto no tienen un orden específico. No puedes confiar en el orden en que se almacenan los elementos en un conjunto.

- **Mutables:** Los conjuntos son mutables, lo que significa que puedes agregar y eliminar elementos después de haber creado el conjunto.

```python
conjunto_vacio = set()

# Definición de un conjunto con elementos
conjunto1 = {1, 2, 3, 4, 5}

# Convertir una lista a un conjunto usando set()
lista = [3, 4, 5, 6, 7]
conjunto2 = set(lista)

# Acceder a elementos de un conjunto (los conjuntos no tienen índices)
# Por lo tanto, se utiliza un bucle para acceder a los elementos
print("Acceder a elementos:")
for elemento in conjunto1:
    print(elemento)

# Verificar si un elemento está en el conjunto
elemento_a_verificar = 3
print(f"¿El elemento {elemento_a_verificar} está en conjunto1?:", elemento_a_verificar in conjunto1)

# Operaciones con conjuntos (unión, intersección, diferencia)
conjunto3 = {4, 5, 6, 7, 8}
union = conjunto1.union(conjunto3)
interseccion = conjunto1.intersection(conjunto3)
diferencia = conjunto1.difference(conjunto3)

# Imprimir conjuntos y resultados de operaciones
print("Conjunto3:", conjunto3)
print("Unión de conjunto1 y conjunto3:", union)
print("Intersección de conjunto1 y conjunto3:", interseccion)
print("Diferencia entre conjunto1 y conjunto3:", diferencia)
```

## Diccionarios


Un diccionario es una estructura de datos que permite almacenar y organizar información de manera eficiente. A diferencia de las listas o tuplas, los diccionarios no tienen un orden específico, y los datos se acceden mediante claves en lugar de índices. Cada elemento en un diccionario consiste en una clave y su correspondiente valor asociado.

- **Claves Únicas:** Cada clave en un diccionario es única, lo que significa que no puede haber duplicados. Sin embargo, los valores asociados pueden repetirse.

- **Mutable:** Los diccionarios son objetos mutables, lo que significa que puedes modificar, agregar o eliminar elementos después de haber sido creados.

- **Dinámico:** Puedes modificar la estructura del diccionario durante su vida útil, agregando nuevas claves o eliminando claves existentes.

- **Heterogéneo:** Los valores en un diccionario pueden ser de cualquier tipo de dato, y cada valor está asociado a una clave.

- **Sin Orden Definido:** A diferencia de las listas, los diccionarios no tienen un orden predefinido. No puedes asumir que los elementos estarán en un orden específico cuando los iteras.

```python
diccionario1 = {
    'nombre': 'Alice',
    'edad': 25,
    'ciudad': 'Ejemplo'
}
print("Diccionario1:", diccionario1)

# Acceder a valores mediante llaves
nombre_dicc = diccionario1['nombre']
edad_dicc = diccionario1['edad']

# Creación de un diccionario desde listas de claves y valores usando zip()
claves = ['nombre', 'edad', 'ciudad']
valores = ['Bob', 30, 'Otro Ejemplo']
diccionario2 = dict(zip(claves, valores))
print("Diccionario2:", diccionario2)

# Creación de un diccionario mediante comprensión de diccionario
numeros = [1, 2, 3, 4, 5]
diccionario_cuadrados = {x: x**2 for x in numeros}
print("Diccionario de Cuadrados:", diccionario_cuadrados)

# Iterar sobre claves y valores de un diccionario
print("Iterar sobre claves y valores:")
for clave, valor in diccionario1.items():
    print(f"{clave}: {valor}")

# Creación de un diccionario con un solo elemento
diccionario_un_elemento = {'clave_unica': 'valor único'}
print("Diccionario con un solo elemento:", diccionario_un_elemento)

# Creación de un diccionario con la función dict() y una lista de tuplas clave-valor
lista_clave_valor = [('nombre', 'David'), ('edad', 28), ('ciudad', 'Ejemplo')]
diccionario_desde_lista = dict(lista_clave_valor)
print("Diccionario desde lista de tuplas:", diccionario_desde_lista)

# Creación de un diccionario con valores predeterminados usando fromkeys()
claves = ['nombre', 'edad', 'ciudad']
diccionario_con_valores_predeterminados = dict.fromkeys(claves, 'Valor Predeterminado')
print("Diccionario con valores predeterminados:", diccionario_con_valores_predeterminados)
```


# 3 Operadores 

## Operadores aritmétricos

Los operadores aritméticos son utilizados para realizar operaciones matemáticas sobre números. Aquí están los operadores aritméticos básicos:

- **Suma (+):** Suma dos valores.

```python
resultado_suma = 5 + 3  # resultado_suma será 8
```

- **Resta (-):** Resta el segundo valor del primero.

```python
resultado_resta = 7 - 4  # resultado_resta será 3
```

- **Multiplicación** (*): Multiplica dos valores.

```python
resultado_multiplicacion = 2 * 6  # resultado_multiplicacion será 12
```

- **División (/):** Divide el primer valor por el segundo. El resultado siempre es un número de punto flotante, incluso si la división es exacta.

```python
resultado_division = 8 / 4  # resultado_division será 2.0
```

- **División Entera (//):** Divide el primer valor por el segundo y redondea hacia abajo al entero más cercano.

```python
resultado_division_entera = 9 // 4  # resultado_division_entera será 2
```

- **Módulo (%):** Devuelve el resto de la división entre el primer valor y el segundo.


```python
resultado_modulo = 9 % 4  # resultado_modulo será 1
```

- **Exponente ():** Eleva el primer valor a la potencia del segundo.

```python
resultado_exponente = 2 ** 3  # resultado_exponente será 8
```

## Operadores de comparación

Los operadores de comparación en Python permiten comparar dos valores y devuelven un resultado booleano (True o False) que indica si la comparación es verdadera o falsa. Aquí están los operadores de comparación:

- **Igualdad (==):** Comprueba si dos valores son iguales.

```python 
resultado_igualdad = 5 == 5  # resultado_igualdad será True
```
- **Desigualdad (!=):** Comprueba si dos valores no son iguales.

```python
resultado_desigualdad = 5 != 3  # resultado_desigualdad será True
```
- **Mayor que (>):** Comprueba si el primer valor es mayor que el segundo.

```python
resultado_mayor_que = 7 > 4  # resultado_mayor_que será True
```

- **Menor que (<):** Comprueba si el primer valor es menor que el segundo.

```python
resultado_menor_que = 3 < 6  # resultado_menor_que será True
```

-**Mayor o igual que (>=):** Comprueba si el primer valor es mayor o igual que el segundo.

```python
resultado_mayor_igual_que = 5 >= 5  # resultado_mayor_igual_que será True
```

- **Menor o igual que (<=):** Comprueba si el primer valor es menor o igual que el segundo.

```python
resultado_menor_igual_que = 4 <= 7  # resultado_menor_igual_que será Tru
```



## Operadores lógicos

Los operadores lógicos en Python se utilizan para combinar expresiones booleanas y realizar operaciones lógicas:

- **AND (and):** Devuelve True si ambas expresiones booleanas son verdaderas, de lo contrario, devuelve False.
- **OR (or):** Devuelve True si al menos una de las expresiones booleanas es verdadera, de lo contrario, devuelve False.
- **NOT (not):** Devuelve True si la expresión booleana es falsa, y viceversa.

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
 
## Condicionales


Las estructuras condicionales en Python, principalmente representadas por las instrucciones if, elif (else if), y else, permiten que un programa tome decisiones basadas en condiciones lógicas. Estas condiciones se expresan mediante expresiones booleanas que evalúan a True o False.

- **if** La instrucción if se utiliza para ejecutar un bloque de código si una condición es verdadera. Si la condición es falsa, el bloque de código no se ejecuta.
- **elif (else if)** La instrucción elif se utiliza para evaluar múltiples condiciones después de un if. Se ejecuta solo si la condición del if es falsa y la condición elif es verdadera.
- **else** La instrucción else se utiliza para ejecutar un bloque de código cuando ninguna de las condiciones anteriores (if o elif) es verdadera.


```python
ingreso_mensual = 1000001

if ingreso_mensual > 100000:
    print("Ingreso alto")
elif ingreso_mensual > 50000 and ingreso_mensual <= 100000:
    print("Ingreso medio")
else:
    print("ingreso bajo")

```
Las estructuras condicionales pueden anidarse, permitiendo condiciones más complejas y toma de decisiones más sofisticadas en un programa. Estos son elementos clave para controlar el flujo de ejecución en Python y en la programación en general.
