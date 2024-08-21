# Calculadora de Fibonacci

Este es un proyecto simple que implementa una calculadora de la secuencia de Fibonacci en una página web. El usuario puede ingresar un número y obtener el valor correspondiente de Fibonacci.

## Descripción

La secuencia de Fibonacci es una serie de números enteros en la que cada número es la suma de los dos anteriores, comenzando con 0 y 1. Esta calculadora permite a los usuarios ingresar un número y obtener el número de Fibonacci correspondiente en la serie.

## Características

- Entrada de número mediante un campo de texto.
- Cálculo instantáneo del número de Fibonacci cuando se hace clic en el botón "Calcular".
- Validación de entrada para asegurar que solo se calculen números no negativos.

## Uso

1. Clona el repositorio o descarga los archivos del proyecto.
2. Abre el archivo `index.html` en un navegador web.
3. Ingresa un número en el campo de texto.
4. Haz clic en el botón "Calcular".
5. El número de Fibonacci correspondiente se mostrará en la página.

## Código Principal

El cálculo de Fibonacci se realiza utilizando la siguiente función JavaScript:

```javascript
function fibonacci(num) {
    const fib = [0, 1];

    for (let i = 2; i <= num; i++) {
        fib[i] = fib[i - 1] + fib[i - 2];
    }

    return fib[num];
}
