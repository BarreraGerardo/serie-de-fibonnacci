# serie-de-fibonnacci
def fibonacci(n):
    fib_series = [0, 1]

    while len(fib_series) < n:
        fib_series.append(fib_series[-1] + fib_series[-2])

    return fib_series[:n]

# Ejemplo de uso
n = int(input("Ingrese el número de términos de la serie de Fibonacci que desea generar: "))

if n <= 0:
    print("Por favor, ingrese un número positivo.")
else:
    result = fibonacci(n)
    print(f"Serie de Fibonacci con {n} términos: {result}")
