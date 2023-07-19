En esta carpeta se almacenarán las actividades del curso de verano.
# Nombre: Abel Dávila Fraire
# Matricula: 1946116
# Programa 1 para sumar 2 numeros 
print("Suma de 2 numeros")

#Colocar Valores
Primer_número = input("Dame el primer número: \n " )
Segundo_número = input("Dame el segundo número: \n ")

#Convertir los valores a enteros debido a que son str
Primer_número = int (Primer_número)
Segundo_número = int (Segundo_número)

#Realizar la suma e imprimirlos seguidamente
Suma = Primer_número + Segundo_número
print("la suma es: ", Suma)
Suma de 2 numeros
Dame el primer número: 
 12
Dame el segundo número: 
 12
la suma es:  24

#Programa 2 para sacar el factorial de un número solicitado por alguien externo

print("Programa para sacar el factorial de un número")
# Pedir el número y convertimos a valor a entero
Número = input("Ingresar el número: \n ")
Número = int(Número)

# Definir la nueva función
def factorial(Número):
  # Analizar si el número es negativo
    if Número < 0:
        print("No se puede sacar factorial a números negativos...")

  # Hacer otra comparativa por si el valor ingresado es igual a 0
    elif Número == 0:
        return 1
  # Realizar las operaciones de multiplicación para el factorial
    else:
        fact = 1
        while(Número > 1):
            fact *= Número
            Número -= 1
        return fact

# Imprimir el resultado
print("El número factorial de ",Número,"es: ", factorial(Número))
Programa para sacar el factorial de un número
Ingresar el número: 
 25
El número factorial de  25 es:  15511210043330985984000000

# Programa 3 que solicita una lista de elementos y busca un elemento en especifico y te dice su posición 

print("Programa para crear una lista además de buscar un elemento especificando la posición en la que se encuentra")

# Definir la nueva variable:
def buscar_elemento():
  # Solicitar datos a ingresar y el elemento a buscar
    lista = input("Ingresar una lista de elementos separados entre espacios:").split() 
    elemento = input("Ingresar el elemento a buscar: ")

    try:
        posición = lista.index(elemento) # El método devuelve el índice del elemento dado anteriormente
        print(f"El elemento '{elemento}' se encuentra en la posición {posición} de la lista.")

    except ValueError: # Si no se encuentra el elemento, se genera un aviso
        print(f"El elemento '{elemento}' no se encuentra en la lista.")

buscar_elemento()
Programa para crear una lista además de buscar un elemento especificando la posición en la que se encuentra
Ingresar una lista de elementos separados entre espacios:0 1 2 3 4
Ingresar el elemento a buscar: 2
El elemento '2' se encuentra en la posición 2 de la lista.

# Programa 4 que especifica si un texto es palidromo o no lo es
print("Programa para checar si un texto es polidromo o no lo es")

cadena_texto = input("Ingresar la frase a analizar: \n ")
def es_palindromo(cadena):
    # Convertir la cadena a minúsculas además de eliminar los espacios en blanco
    cadena = cadena.lower().replace(" ", "")

    # Comparar la cadena original con el reverso
    if cadena == cadena[::-1]:
        return True
    else:
        return False

# Imprimir el resultado dependiendo el resultado
if es_palindromo(cadena_texto):
    print("La oración '", cadena_texto, "' Es un palíndromo.")
else:
    print("La oración '", cadena_texto, "' No es un palíndromo.")
Programa para checar si un texto es polidromo o no lo es
Ingresar la frase a analizar: 
 Veranos
La oración ' Veranos ' No es un palíndromo.
