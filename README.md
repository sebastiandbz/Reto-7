# Reto-7

#### 1. Imprimir un listado con los números del 1 al 100 cada uno con su respectivo cuadrado.

```python 
n = 0
while ( n < 100):
    n += 1
    print (n, n**2)
```

#### 2. Imprimir un listado con los números impares desde 1 hasta 999 y seguidamente otro listado con los números pares desde 2 hasta 1000.

```python 
p = 2
i = 1
print(i)
while (i < 999):
    i += 2
    print(i)
print(p)
while (p < 1000):
    p += 2
    print(p)
```

#### 3. Imprimir los números pares en forma descendente hasta 2 que son menores o iguales a un número natural n ≥ 2 dado.

```python 
n = int(input("numero deseado: "))

while (n >= 2):
    if n == 2: 
        print (n)
        break
    if n %2 == 0 :
        print(n)
        n -=1
    else: n -=1
if n < 2 : print("ingrese un numero mayor o igual a 2")
```

#### 4. Imprimir los números de 1 hasta un número natural n dado, cada uno con su respectivo factorial.

```python 
n = int(input("Ingrese un número natural n (n ≥ 1): "))

if n < 1:
    print("El número debe ser un entero positivo.")
else:
    i = 1
    while i <= n:
        factorial = 1
        j = 1
        while j <= i:
            factorial *= j
            j += 1
        print(f"{i}! = {factorial}")
        i += 1
```

#### 5. Calcular el valor de 2 elevado a la potencia n usando ciclos for.

```python 
n = int(input("Ingrese un número natural n (n ≥ 0): "))

if n < 0:
    print("El exponente debe ser un número entero no negativo.")
else:
    resultado = 1
    for _ in range(n):
        resultado *= 2

    print(f"2 elevado a la {n} es {resultado}")
```

#### 6. Leer un número natural n, leer otro dato de tipo real x y calcular x^n usando ciclos for. Disclaimer: Trate de no utilizar el operador de potencia (**).

```python 
n = int(input("Ingrese un número natural n (n ≥ 0): "))
x = float(input("Ingrese un número real x: "))

if n < 0:
    print("El exponente n debe ser un número natural (n ≥ 0).")
else:
    resultado = 1.0
    for _ in range(n):
        resultado *= x

    print(f"{x} elevado a la {n} es {resultado}")
```

#### 7. Diseñe un programa que muestre las tablas de multiplicar del 1 al 9.

```python 
i = 1
while i <= 9:
    print(f"\nTabla del {i}:")
    
    j = 1
    while j <= 10:
        print(f"{i} x {j} = {i * j}")
        j += 1
    
    i += 1
```
