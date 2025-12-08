## 💾📝CONTENIDOS DE LA UNIDAD 2

### 🚦🔶 ESTRUCTURAS CONDICIONALES

---

#### 🚪 ESTRUCTURA CONDICIONAL SIMPLE (IF)

Estas estructuras se la denomina simple porque evalúa una sola condición, si determina que es verdadera ejecuta la instrucción dentro de la condición, si es falsa, la ignora y continúa con el resto de código que no esté en la condición.

##### 🧑‍💻 Ejemplo Práctico:

###### Diagrama de Flujo:

<p align="left">
  <img src="https://drive.google.com/uc?export=view&id=1klfSlSxzLzeBvJfXfmoRLSHExsnr0s8V" alt="Descripción" width="70%">
</p>

<p style="text-align:center; font-size:12px;">Fig. 5. Diagrama de Flujo para la demostración de la Estructura Condicional Simple. (Elaboración Propia). </p>

###### Código en C:


```

#include <stdio.h>

int main( ){

    float gastoTotal;
    float descuento;

    printf("Ingrese cuanto gasto en su compra: \n");
    scanf("%f", &gastoTotal);
    getchar();

    if(gastoTotal>=100){
        printf("Felicidades, tiene un descuento del 20 porciento por su compra de $100 en adelante\n");
        descuento = gastoTotal * 0.20;
        gastoTotal = gastoTotal - descuento;
    }

    printf("El precio final de su compra es: %.2f\n", gastoTotal);

    return 0;

}

```

#### 💡Explicación:

Como se puede observar en el diagrama de flujo, el algoritmo empieza definiendo las variables, luego le pide al usuario ingresar el valor de su compra, a continuación sigue con la condición, que evalúa si el valor de la compra es mayor o igual a 100. Si determina que sí lo es, ingresa en el camino de la derecha y muestra el mensaje del descuento, continuando realiza los cálculos para aplicar el descuento del 20% al valor de la compra y mostrar el mensaje final.

Si determina que la compra es menor a 100 dólares, ignora el "if" y muestra el mensaje final.

---

#### 🔀 ESTRUCTURA CONDICIONAL DOBLE (IF-ELSE)

Este tipo de estructura evalúa la condición y nos brinda dos caminos que se excluyen entre sí, si el programa determina que la condición es verdadera ejecutará lo que esté dentro del bloque "if", pero si demuestra que es falsa, ejecuta lo que está dentro del bloque "else".

##### 🧑‍💻 Ejemplo Práctico:

###### Diagrama de Flujo:

<p align="left">
  <img src="https://drive.google.com/uc?export=view&id=174d5_c5jpGUy7GtAM1tyldWTRBZ9_nke" alt="Descripción" width="90%">
</p>

<p style="text-align:center; font-size:12px;">Fig. 6. Diagrama de Flujo para la demostración de la Estructura Condicional Doble. (Elaboración Propia). </p>

###### Código en C:

```

#include <stdio.h>

int main( ){

    float gastoTotal;
    float descuento;

    printf("Ingrese cuanto gasto en su compra: \n");
    scanf("%f", &gastoTotal);
    getchar();

    if(gastoTotal>=100){
        printf("Felicidades, tiene un descuento del 20 porciento por su compra de $100 en adelante\n");
        descuento = gastoTotal * 0.20;
        gastoTotal = gastoTotal - descuento;
    }else {
        printf("Usted no aplica para el descuento, su compra es menor a $100\n");
    }

    printf("El precio final de su compra es: %.2f\n", gastoTotal);

    return 0;

}

```

#### 💡Explicación:

Ahora, como observamos en el diagrama de flujo, el algoritmo empieza definiendo las variables, luego de eso pide al usuario ingresar el valor de su compra.

Continuando con esto, tenemos la condición (if-else) que evalúa si el valor de la compra es mayor o igual a 100.

Si determina que es verdadero (if), entra en el camino de la derecha muestra el mensaje del descuento y realiza los cálculos para aplicar el 20% y después mostrar el mensaje final.

Si determina que es falso (else), ingresa por el camino de la izquierda y le muestra al usuario el mensaje de que no aplica al descuento y mostrar a continuación el mensaje final con el valor original al no haberse aplicado el descuento.

---

#### 🗂️ ESTRUCTURA CONDICIONAL MÚLTIPLE (SWITCH)

Esta estructura nos permite evaluar la condición y comparar su valor con una lista de casos, si el valor coincide con alguno de estos casos, se ejecutará ese bloque de código.

##### 🧑‍💻 Ejemplo Práctico:

###### Diagrama de Flujo:

<p align="left">
  <img src="https://drive.google.com/uc?export=view&id=1T45EJZ3M_0lK4JA5PJfwltqmIh-Tm_t-" alt="Descripción" width="150%">
</p>

<p style="text-align:center; font-size:12px;">Fig. 7. Diagrama de Flujo para la demostración de la Estructura Condicional Múltiple. (Elaboración Propia). </p>

###### Código en C:

```

#include <stdio.h>
#include <string.h>

int main(){

    float numero1;
    float numero2;
    float resultado;
    char operador;

    printf("Ingrese el primer numero: \n");
    scanf("%f", &numero1);

    printf("Ingrese el segundo numero: \n");
    scanf("%f", &numero2);

    printf("Escriba el operador a usar (+, -, *, /): \n");
    scanf(" %c", &operador);

    switch (operador){

        case '+':
        resultado = numero1 + numero2;
        printf("El resultado de su operacion es: %.2f\n", resultado);
        break;

        case '-':
        resultado = numero1 - numero2;
        printf("El resultado de su operacion es: %.2f\n", resultado);
        break;

        case '*':
        resultado = numero1 * numero2;
        printf("El resultado de su operacion es: %.2f\n", resultado);
        break;

        case '/':

        resultado = numero1 / numero2;
        printf("El resultado de su operacion es: %.2f\n", resultado);
        break;
        
        default:
        printf("Operador invalido\n");
    }

    return 0;

}

```

#### 💡Explicación:

Como se ve en el diagrama de flujo, primero definimos las variables, luego de eso se pide al usuario ingresar los dos números y el operador que se desea.

Ahora, seguimos con la estructura del switch, si el usuario escribe un operador que coincida con los diferentes casos (+, -, *, /). Según con cuál coincida ejecutará la operación que esté dentro de ese caso.

Si ingresa un operador que no coincide con ningún caso, se le mostrará un mensaje de que el operador es inválido.

---

### 🔄 ESTRUCTURAS REPETITIVAS

---

#### ⏳ ESTRUCTURA REPETITIVA (WHILE)

While es una estructura repetitiva del tipo controlada por entrada, es decir, antes de ingresar al bucle primero evalúa la condición, si la condición es verdadera se repetirá mientras siga siendo verdadera, en cambio, si la instrucción es falsa nunca se ejecutará.

##### 🧑‍💻 Ejemplo Práctico:

###### Diagrama de Flujo:

<p align="left">
  <img src="https://drive.google.com/uc?export=view&id=1wIQCxgAo_GYaYPpGFqJux1AVMqyiR78s" alt="Descripción" width="30%">
</p>

<p style="text-align:center; font-size:12px;">Fig. 8. Diagrama de Flujo para la demostración de la Estructura Repetitiva While. (Elaboración Propia). </p>

###### Código en C:

```

#include <stdio.h>

int main(){

    int i = 0; 

    printf("Numeros del 0 al 10:\n");
    while (i <= 10) {
        printf("%i \n", i); 
        i++; 
    }
}

```

#### 💡Explicación:

Este algoritmo nos presenta el funcionamiento de "While", que básicamente lo que hace en este programa es que imprime los números del 0 al 10, para realizar esto en cada repetición evalúa si la variable es menor o igual a 10, mientras lo sea el bucle imprime un número y aumenta su valor en 1 hasta que "i" sea mayor a 10, que es cuando considera que la condición es falsa y termina el bucle.

---

#### ▶️ ESTRUCTURA REPETITIVA (DO - WHILE)

El Do-While es una estructura del tipo controlado por salida, es decir, primero se ejecuta el bloque de código, luego se evalúa la condición, si se cumple la condición se repetirá hasta que sea falsa o sea el cuerpo del bucle se cumplirá al menos una vez.

##### 🧑‍💻 Ejemplo Práctico:

###### Diagrama de Flujo:

<p align="left">
  <img src="https://drive.google.com/uc?export=view&id=1_cIyLkr-tfhA4kqDnIXm9pnGdAs04m7K" alt="Descripción" width="30%">
</p>

<p style="text-align:center; font-size:12px;">Fig. 9. Diagrama de Flujo para la demostración de la Estructura Repetitiva Do-While. (Elaboración Propia). </p>

###### Código en C:

```

#include <stdio.h>

int main(){

    int i = 0; 

    printf("Numeros del 0 al 10:\n");

    do{
        printf("%i \n", i);
        i++; 
    }while (i <= 10);

    return 0;
    
}

```

#### 💡Explicación:

En este algoritmo podemos ver cómo funciona el do-while, este programa primero imprime el número y va aumentando en 1, luego de ejecutar esa instrucción el programa evalúa la condición para ver si la variable "i" sigue siendo menor o igual a 10 para verificar si sigue imprimiendo números o parar si es que ya sobrepasó la condición.

---

#### 🔢 ESTRUCTURA REPETITIVA (FOR)

Este es una estrucutra del tipo controlada por entrada en la cual se juntan la inicialización de la variable, la condición y el aumento o decremento en una línea, esta estructura evalúa primero la condición antes de la instrucción para poder ejecutarla.

##### 🧑‍💻 Ejemplo Práctico:

###### Diagrama de Flujo:

<p align="left">
  <img src="https://drive.google.com/uc?export=view&id=1lYnKvvJL3-q4W-dmALQ7P0YDAagyhJ0B" alt="Descripción" width="30%">
</p>

<p style="text-align:center; font-size:12px;">Fig. 10. Diagrama de Flujo para la demostración de la Estructura Repetitiva For. (Elaboración Propia). </p>

###### Código en C:

```

#include <stdio.h>

int main(){

    int i;

    for(i=0; i<=10; i++){
        printf("%i \n", i);
    }

    return 0;

}

```

#### 💡Explicación:

Este otro algoritmo muestra cómo funciona el "For", este programa junta en una sola línea que controla todo la inicialización, la condición lógica y la actualización del contador, el programa empieza con la variable en 0 y evaluando que sea menor o igual a 10, mientras eso se cumpla el programa va a ejecutar el bloque de código, imprime el número y automáticamente aumenta en  1 en cada repetición; este proceso se repite hasta que la variable sea mayor a 10, deteniéndose por sí solo cuando la variable supera el 10.

---

### 🧑‍💻 EJERCICIO COMBINANDO ESTRUCTURA CONDICIONAL Y REPETITIVA (Java o Python).

#### 🧠 Contexto del Problema

Desarrollar un programa que permita gestionar las notas finales de un grupo de estudiantes. El algoritmo debe solicitar inicialmente la cantidad de alumnos a evaluar.

Mediante un ciclo repetitivo, el sistema pedirá la nota de cada estudiante, validando obligatoriamente que el valor esté entre 0 y 10 (si es incorrecto, debe volver a pedirlo). Basándose en la nota válida, el programa determinará si el estudiante está "Aprobado" (nota >= 7) o "Reprobado", mostrando al finalizar el proceso el conteo total de cada categoría.

###### Diagrama de Flujo (Bucle y Condición):

<p align="left">
  <img src="https://drive.google.com/uc?export=view&id=10Gut1QkJncwJ3v9skE-4l3TBpDfQ9brN" alt="Descripción" width="30%">
</p>

<p style="text-align:center; font-size:12px;">Fig. 11. Diagrama de Flujo para la demostración del problema Combinado. (Elaboración Propia). </p>

###### Código en Python

```
def main():

    aprobados = 0
    reprobados = 0

    print("CALIFICACIONES")
    
    cantidad_alumnos = int(input("Ingrese cuantos estudiantes van a ser evaluados: "))
    contador = 1

    while contador <= cantidad_alumnos:
        
        print(f"Notas del Estudiante {contador}")
        nota = float(input("Ingresa la nota: "))

        while nota < 0 or nota > 10:
            print("Ingresa una nota entre 0 y 10")
            nota = float(input("Nota: "))

        if nota >= 7:
            print("APROBADO")
            aprobados = aprobados + 1
        else:
            print("REPROBADO")
            reprobados = reprobados + 1

        contador = contador + 1

    print(f"Estudiantes Evaluados: {cantidad_alumnos}")
    print(f"Aprobados: {aprobados}")
    print(f"Reprobados: {reprobados}")

if __name__ == "__main__":
    main()
```

###### Verificación:

<p align="left">
  <img src="https://drive.google.com/uc?export=view&id=1oXkTDo23ePDD2idHXQxi5aUq4tvH4aMG" alt="Descripción" width="90%">
</p>

<p style="text-align:center; font-size:12px;">Fig. 12. Compilación y Ejecución del Código en Python. (Elaboración Propia). </p>

##### 💡Explicación:

Este algoritmo es un sistema para gestionar las calificaciones mediante un while, el cual controla el procesamiento de la cantidad de estudiantes que va a ser definida por el usuario. Luego con un bucle anidado que hace la validación de entrada, es decir, verifica que los datos ingresados estén en el rango de 0 a 10, cuando verifica que sea verdadero, con el if-else clasifica el rendimiento del alumno y actualiza los contadores antes de repetir el siguiente registro.

---

### ⚠️🤔 PRINCIPALES DIFICULTADES EN LA APLICACIÓN DE LOS CONTENIDOS 

Se me dificultó un poco aprender lo que hacía cada estructura, repetitiva y condicional, deducir cuándo usar cada tipo de estructura, aprender las restricciones y sintaxis de estas, sin olvidar que la introducción a Java que se me hizo un poco difícil el gran cambio para programar en este lenguaje estando acostumbrado al lenguaje C.

---

### 🧠💡 REFLEXIÓN CRÍTICA DE LOS APRENDIZAJES DE LA UNIDAD 

En esta unidad aprendí a usar las estructuras repetitivas y condicionales que son de mucha ayuda para el futuro, ya que son las que me ayudan a optimizar y dinamizar mi código pasando de uno simple y lineal a uno que puede procesar información compleja. Esta unidad ha sido de gran ayuda para mi formación, aunque se me dificultó un poco, ha sido una Unidad muy completa y educativa.

---

### 📋 ANEXOS

🗨️ [Ejercicios en C de la U2](https://drive.google.com/drive/folders/1tKoqiJzLP1xzlgG0zQEEf0gIEfGTwtf4?usp=sharing)

🗨️ [Ejercicios en Java](https://drive.google.com/drive/folders/1LoXlwtd0ydXIsZ-LheY-3o-qDdHWErG-?usp=sharing)

---

<p align="right">
  <a href="index.md">Volver a la página principal</a>
</p>

