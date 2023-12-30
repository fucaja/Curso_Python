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







