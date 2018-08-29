# Conceptos basicos de python

### declaracion de variables
~~~
numero1 = 10
numero2 = 20
~~~

### declaracion de metodos
~~~
def suma(num1, num2):
    resultado = num1 + num2
    print "el resultado de la suma es: ",resultado
~~~

suma(5, 19)

suma(numero1, numero2)

~~~
def resta(num1, num2):
    print "Esto es una variable global: ", numero1
    resultado = num1 - num2
    print "El resultado de la resta es: "+str(resultado)
~~~  

### metodos incluidos

print pow(2,3)


### str convertir a string
~~~
print str(resta(10, 5))
~~~

### eliminar una variable
~~~
del numero1
~~~

### Listas
~~~
miLista = [1, 2, 3, "texto1", "texto2", ["texto de otra lista", 1, 2]]
print(miLista)
print(miLista[0])
~~~  

### Tuplas
*no pueden ser modificadas*
~~~
miTupla = (1, 2, 3)
print(miTupla)
print(miTupla[2])
~~~

#### Diccionario
~~~
miDiccionario = {"nombre": "carlos", "apellido": "perez", "edad": 10}

print(miDiccionario["edad"])
~~~  

## Conversiones

#### Flotante a Entero
~~~
  int(4.3)
  >>4
~~~

#### Entero a flotante
~~~
  float(5)
  >>5.0
~~~

#### Entero a String
~~~
  str(6.2)
  >>"6.2"
~~~

___

### Operadores Comunes

*Longitud de una cadena, lista, tupla, etc*
~~~
    >>> len("key")
    3
~~~

*Conocer el tipo de datos*
~~~
    type(4)
    <type int>
~~~

*Aplicar una conversion a un conjunto como una lista*
~~~
    map(str, [1, 2, 3, 4])
    >>>['1', '2', '3', '4']
~~~

*Redondear un flotante con x numero de decimales*
~~~
    round(12.88889, 1)
    >>>12.8
~~~

*Generar un rango en una lista*
~~~
    range(5)
    >>>[0, 1, 2, 3, 4, 5]
~~~

*Sumar un conjunto*
~~~
    sum([1, 2, 3, 4])
    >>>10
~~~

*Organizar un conjunto*
~~~
    sorted([9, 5, 8, 1])
    >>>[1, 5, 8, 9]
~~~

*Conocer los comandos que puedes aplicar a x tipo de datos*
~~~
    li = [1, 2, 3, 5]
    dir(li)
    >>>['append', 'count', 'extend', 'index', 'insert', 'pop', 'remove', 'reverse', 'sort']
~~~

*Informacion sobre una funcion o una libreria*
~~~
    help(sortes)
~~~
se visualizara todo la informacion sobre la funcion sorted

### Clases

*Para crear un contructur definimos una funcion con nombre **init** y de parametros self*
*(que significa, su misma clase)*

~~~
    class Estudiante(object): 
        def __init__(self,nombre_r,edad_r): 
            self.nombre = nombre_r 
            self.edad = edad_r 

        def hola(self): 
            return "Mi nombre es %s y tengo %i" % (self.nombre, self.edad) 

    e = Estudiante(?Arturo?, 21) 
    print e.hola() 
    >>>Mi nombre es Arturo y tengo 21
~~~

### Metodos especiales

**cmp**(self, otro)
Método llamado cuando utilizas los operadores de comparación para comprobar si tu objeto es menor, mayor o igual al objeto pasado como parámetro.

**len**(self)
Método llamado para comprobar la longitud del objeto. Lo usas, por ejemplo, cuando llamas la función len(obj) sobre nuestro código. Como es de suponer el método te debe devolver la longitud del objeto.

**init**(self,otro)
Es un constructor de nuestra clase, es decir, es un ?método especial? que es llamas automáticamente cuando creas un objeto.

### Condicionales IF
~~~
    if ( a > b ):
        elementos 
    elif ( a == b ): 
        elementos 
    else:
        elementos
~~~

### Bucle FOR
~~~
  for i in ____:
 	elementos**

# Ejemplo:

 for i in range(10):
 	print i
~~~

### Bucle WHILE
~~~
    while (condición):
 	    elementos
~~~