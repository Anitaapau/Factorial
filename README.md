# Factorial
## ¿Qué es el factor de un numero?
 #### Un factor es un número que divide exactamente a otro número. Así que 4 ‍ es un factor de 32
![image](https://github.com/user-attachments/assets/3f8f1def-3679-4d3a-b9eb-b45a6459fc3c)
## PROGRAMA DE KOTLIN 
Este programa es un punto de partida clásico para cualquier lenguaje de programación. Si quieres algo más avanzado o específico, como una calculadora, una aplicación de consola que maneje entradas, o algo relacionado con la programación orientada a objetos, házmelo saber. 

![image](https://github.com/user-attachments/assets/466b02a3-103d-4bc0-a843-6a2260887096)

El cálculo del factorial de un número es un ejemplo clásico de recursividad. El factorial de un número 
𝑛 (denotado como 𝑛!) es el producto de todos los números enteros positivos menores o iguales a 𝑛. La fórmula recursiva para el factorial es:

![image](https://github.com/user-attachments/assets/79a1e237-faa5-4de6-b3c1-6f22dde6ecd4)

Aquí está la implementación en Kotlin:

![image](https://github.com/user-attachments/assets/1c6fb59f-a426-44a7-84d1-ffa6c992ac3a)


### Explicacion del Código
1_ Definición de la función factorial
   * fun factorial(n: Int): Int define una función llamada factorial que toma un parámetro n de tipo Int y devuelve un valor de tipo Int.
   * Dentro de la función, usamos una expresión if para determinar si n es menor o igual a 1.
   * Si n <= 1, la función devuelve 1. Este es el caso base de la recursividad, donde el cálculo termina. En matemáticas, 0!=1 y 1!=1, por lo que el caso base se establece en 1.
   * Si n es mayor que 1, la función devuelve el producto de n y el resultado de llamar a la función factorial con el argumento n - 1. Esta es la llamada recursiva, donde la función se llama a sí misma con un valor decrementado de n.
##### ¿Cómo funciona la recursividad aquí?
      * La llamada recursiva factorial(n - 1) sigue reduciendo el valor de n hasta que llega al caso base n <= 1.
      *Cada llamada recursiva se apila, y se resuelve al llegar al caso base. Una vez que se resuelve el caso base, las llamadas recursivas se van resolviendo en orden inverso.
      ![image](https://github.com/user-attachments/assets/247cf8d6-f1d1-4442-8f15-f771436a2f84)

   2_ Uso de la función en main
   * fun main() es la función principal donde se ejecuta el programa.
   * val number = 5 define una variable llamada number y le asigna el valor 5.
   * println("El factorial de $number es ${factorial(number)}") imprime el resultado del cálculo del factorial de number. La expresión ${factorial(number)} llama a la función factorial con el valor de number (que es 5) y muestra el resultado.
![image](https://github.com/user-attachments/assets/8000ce97-aa81-4224-a9e9-62dee12f0130)
##### Ejecución Paso a Paso
Para entender cómo se calcula el factorial de 5, veamos el proceso de recursividad:
1_ Llamada inicial: factorial(5)
* n > 1, entonces 5 * factorial(4)
2_ Llamada a factorial(4)
* n > 1, entonces 4 * factorial(3)
3_Llamada a factorial(3)
* n > 1, entonces 3 * factorial(2)
4_Llamada a factorial(2)
 * n > 1, entonces 2 * factorial(1)
5_  Llamada a factorial(1)   
* n <= 1, entonces retorna 1
Ahora resolvemos las llamadas recursivas en orden inverso:

* factorial(2) regresa 2 * 1 = 2
* factorial(3) regresa 3 * 2 = 6
* factorial(4) regresa 4 * 6 = 24
* factorial(5) regresa 5 * 24 = 120
Entonces, el resultado final de factorial(5) es 120, y el programa imprime: "El factorial de 5 es 120".






