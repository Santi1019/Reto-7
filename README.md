# Reto 7
1. Imprimir un listado con los números del 1 al 100 cada uno con su respectivo cuadrado.
```
   i = 1
while i <= 100:
    numero_ = i
    cuadrado_ = i**2
    print("Numero: ", numero_ ,"Y su cuadrado: ", cuadrado_)
    i += 1
```
2. Imprimir un listado con los números impares desde 1 hasta 999 y seguidamente otro listado con los números pares desde 2 hasta 1000.
```
i: int = 1
while i<= 999:
    print ("Los numeros impares son: ",i)
    i +=2
```
3. Imprimir los números pares en forma descendente hasta 2 que son menores o iguales a un número natural n ≥ 2 dado
```
N = int(input("Ingrese un numero mayor o igual que dos: "))
while N >= 2:
    print (N)
    N-=2 

```
4. En 2022 el país A tendrá una población de 25 millones de habitantes y el país B de 18.9 millones. Las tasas de crecimiento anual de la población serán de 2% y 3% respectivamente. Desarrollar un algoritmo para
```
A = 25
B = 18.9
tasa_a = 0.2
tasa_b = 0.3
edad_xd = 2022

while B <= A:
    A+= A*tasa_a
    B+= B*tasa_b
    edad_xd +=1
print("La poblacion del pais B superará a la del pais A en el año: ", edad_xd)
```
5. informar en que año la población del país B superará a la de A.
```
n = int(input("Ingrese un numero entero: "))
if n>= 0:
    x = 1
    f = 1
    while x<=n:
        f = f*x
        x+=1
    print("El factorial del numero ingresado es: ",f)
```

6. Imprimir el factorial de un número natural n dado.
```
x = int(input("Ingrese numero: "))

def numero_factorial(n):
  i : int = 1
  factorial : int = 1
  while(i <= n):
    factorial *= i
    i += 1
  return factorial

print("El factorial de", x, "es",numero_factorial(x))
```
7. Implementar un algoritmo que permita adivinar un número dado de 1 a 100, preguntando en cada caso si el número es mayor, menor o igual.
```

import random

numero_secreto = random.randint(1, 100)

while True:
    
    m = int(input("Adivina el número entre 1 y 100: "))

    if m < numero_secreto:
        print("El número es mayor.")
    elif m > numero_secreto:
        print("El número es menor.")
    else:
        print("Por fin, casi que no caramonda, el numero es: ", numero_secreto)
```
8. Implementar un programa que ingrese un número de 2 a 50 y muestre sus divisores.
```
n = float(input("Ingrese un un numero que este entre 2 y 50: "))

if 2<= n <= 50:
    for m in range(1, n + 1):
        if n % m == 0:
            print("Sus divisores son: ", m)

        
    
else:
    print ("El numero debe estar entre 2 y 50")
```
9. Implementar el algoritmo que muestre los números primos del 1 al 100. Nota: use funciones
```
def es_primo(i):
    if i == 2: return True
    for a in range(2,int( i**(0.5) )+1):
        if i % a == 0 and i!= a:
            return False
    return True
```

i: int = 2
while i <= 100:
    if es_primo(i) == True:
        print(i)
    i = i + 1
```
