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