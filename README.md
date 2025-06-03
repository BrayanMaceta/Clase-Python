# Clase-Python

Ejercicio 1:

```python
# Pedir dos números al usuario  
numero1 = float(input("Introduce el primer número: "))  
numero2 = float(input("Introduce el segundo número: "))  

# Calcular la suma  
suma = numero1 + numero2  

# Mostrar el resultado  
print("La suma de los dos números es:", suma)  
```
Ejercicio 2:

```python
# Solicitar al usuario la temperatura en grados Celsius
celsius = float(input("Introduce la temperatura en grados Celsius: "))

# Aplicar la fórmula para convertir a Fahrenheit
fahrenheit = celsius * 1.8 + 32

# Mostrar el resultado
print(f"{celsius} grados Celsius equivalen a {fahrenheit} grados Fahrenheit.")
```
Ejercicio 3:

```python
# Pedimos al usuario la base y la altura del triángulo
base = float(input("Introduce la base del triángulo: "))
altura = float(input("Introduce la altura del triángulo: "))

# Calculamos el área
area = (base * altura) / 2

# Mostramos el resultado
print(f"El área del triángulo es: {area}")
```
Ejercicio 4:

```python
# Pide un número y determina si es par o impar

numero = int(input("Introduce un número entero: "))

if numero % 2 == 0:
    print(f"El número {numero} es par")
else:
    print(f"El número {numero} es impar")
```
Ejercicio 5:

```python
# Descripción: Intercambia los valores de dos variables sin usar una tercera variable

# Valores iniciales
a = 5
b = 10

print(f"Valores originales: a = {a}, b = {b}")

# Intercambio usando asignación múltiple
a, b = b, a

print(f"Valores intercambiados: a = {a}, b = {b}")
```
Ejercicio 6:

```python
# Realiza suma, resta, multiplicación y división con dos números

def calculadora():
    print("\n--- CALCULADORA SIMPLE ---")
    num1 = float(input("Ingresa el primer número: "))
    num2 = float(input("Ingresa el segundo número: "))
    
    print("\nOperaciones disponibles:")
    print("1. Suma (+)")
    print("2. Resta (-)")
    print("3. Multiplicación (*)")
    print("4. División (/)")
    
    opcion = input("\nElige una operación (1-4): ")
    
    if opcion == '1':
        print(f"\nResultado: {num1} + {num2} = {num1 + num2}")
    elif opcion == '2':
        print(f"\nResultado: {num1} - {num2} = {num1 - num2}")
    elif opcion == '3':
        print(f"\nResultado: {num1} * {num2} = {num1 * num2}")
    elif opcion == '4':
        try:
            print(f"\nResultado: {num1} / {num2} = {num1 / num2}")
        except ZeroDivisionError:
            print("\nError: No se puede dividir entre cero")
    else:
        print("\nOpción no válida")

calculadora()
```
Ejercicio 7:

```python
# Calcula la cantidad aproximada de meses y días a partir de años

edad_años = int(input("Ingresa tu edad en años: "))

meses = edad_años * 12
dias = edad_años * 365  # Aproximación sin considerar años bisiestos

print(f"\n{edad_años} años equivalen aproximadamente a:")
print(f"- {meses} meses")
print(f"- {dias} días")
```
Ejercicio 8:

```python
# Determina el mayor de tres números ingresados

num1 = float(input("Ingresa el primer número: "))
num2 = float(input("Ingresa el segundo número: "))
num3 = float(input("Ingresa el tercer número: "))

# Determinar el mayor usando comparaciones
mayor = num1
if num2 > mayor:
    mayor = num2
if num3 > mayor:
    mayor = num3

print(f"\nEl número mayor es: {mayor}")
```
Ejercicio 9:

```python
# Determina si el primer número es múltiplo del segundo

num1 = int(input("Ingresa el primer número (múltiplo): "))
num2 = int(input("Ingresa el segundo número (divisor): "))

if num2 == 0:
    print("Error: No se puede dividir por cero")
elif num1 % num2 == 0:
    print(f"{num1} es múltiplo de {num2}")
else:
    print(f"{num1} NO es múltiplo de {num2}")
```
Ejercicio 10:
```python
# Ejercicio 10: Salario con bonificación
# Calcula el salario total con un bono del 10%

salario_base = float(input("Ingrese el salario base del empleado: "))
bono = salario_base * 0.10  # Calcula el 10% de bono
salario_total = salario_base + bono

print(f"\nDetalle de salario:")
print(f"- Salario base: ${salario_base:,.2f}")
print(f"- Bono (10%):   ${bono:,.2f}")
print(f"- Total:       ${salario_total:,.2f}")
```



