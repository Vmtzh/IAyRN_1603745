Act 2

Ejercicio 1
Escribe un programa que le pida al usuario por su nombre y que lo salude con su nombre, excepto si se llama “Ana”, “Juan”, y “Pedro”.

nombre1="Ana"
nombre2="ana"
nombre3="Juan"
nombre4="juan"
nombre5="Pedro"
nombre6="pedro"
print("¿Cual es su nombre?")
nombre = input()
if nombre == nombre1 or nombre == nombre2 or nombre == nombre3 or nombre == nombre4 or nombre == nombre5 or nombre == nombre6:
  print("Hola Bienvenido")
else:
  print("Hola", nombre, "Bienvenido")


  Ejercicio 2
Escribe una función que regrese el último elemento de una lista y que revierta el orden de la lista e imprima la lista revertida.

from google.colab import drive
drive.mount('/content/drive')
lista = [1,2,3,4,5,6,7,8,9,10]
ultimo_elemento = lista[9]
def invertir_lista(lista):
  if lista == []:
    return lista
  else:
     return [lista[-1]] + invertir_lista(lista[:-1])

print(ultimo_elemento)
print(invertir_lista(lista))


#### Ejercicio 3

Escribe una función que toma una lista de strings y los imprima línea por línea en un marco rectangular. Por ejemplo, la lista [“Hola”, “a”, “todos”, “esto”, “es”, “un”, “marco”] se imprime: 

********** 

* Hola    * 

* a          *

* todos  * 

* esto    * 

* es        * 

* un        * 

* marco * 

********** 

lista = ["**********", "* Hola   *", "* a      *", "* todos  *", "* esto   *", "* es     *", "* un     *", "* marco  *", "**********"]
resultado = "\n".join([str(sublista) for sublista in lista])

print(lista)
print()
print(resultado)
