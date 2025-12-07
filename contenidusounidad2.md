## 💾📝CONTENIDOS DE LA UNIDAD 2

### ESTRUCUTRAS CONDICIONALES

---

#### ESTRUCTURA CONDICIONAL SIMPLE (IF)

Esta estructuras se la denomina simple por que evalua una sola condición, si determina que es verdadera ejecuta la instruccion dentro de la condición, si es falsa, lo ignora y continua con el resto de código que no este en la condición.

##### Ejemplo Práctico:

###### Diagrama de Flujo:

<p align="left">
  <img src="https://drive.google.com/uc?export=view&id=1klfSlSxzLzeBvJfXfmoRLSHExsnr0s8V" alt="Descripción" width="70%">
</p>

<p style="text-align:center; font-size:12px;">Fig. 4. Diagrama de Flujo para la demostracion de la Estructura Condicional Simple. (Elaboración Propia). </p>

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

#### Explicación:

Como se puede observar en el diagrama de flujo, el algoritmo empieza definiendo las variables, luego le pide al usuario ingresar el valor de su compra, a continuación sigue con la condición, que evalua si el valor de la compra es mayor o igual a 100. Si determina que sí lo es, ingresa en el camino de la derecha y muestra el mensaje del descuento, continuando realiza los calculos para aplicar el descuento del 20% al valor de la compra y mostrar el mensaje final.

Si determina que la compra es menor a 100 doláres, ignora el "if" y muestra el mensaje final.

---

#### ESTRUCTURA CONDICIONAL DOBLE (IF-ELSE)

Este tipo de estructura evalúa la condición y nos brinda dos caminos que se excluyen entre si, si el programa determina que la condición es verdadera ejecutará lo que este dentro del bloque "if", pero si demuestra que es falsa, ejecuta lo que esta dentro del bloque "else".

##### Ejemplo Práctico:

###### Diagrama de Flujo:

<p align="left">
  <img src="https://drive.google.com/uc?export=view&id=174d5_c5jpGUy7GtAM1tyldWTRBZ9_nke" alt="Descripción" width="90%">
</p>

<p style="text-align:center; font-size:12px;">Fig. 5. Diagrama de Flujo para la demostracion de la Estructura Condicional Doble. (Elaboración Propia). </p>

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

#### Explicación:

Ahora, como observamos en el diagrama de flujo, el alogoritmo empieza definiendo las variables, luego de eso pide al usuario ingresar el valor de su compra.

Continuando con esto, tenemos la condición (if-else) que evalua si el valor de la compra es mayor o igual a 100.

Si determina que es verdadero (if), entra en el camino de la derecha muestra el mensaje del descuento y realiza los cálculos para aplicar el 20% y después mostrar el mensaje final.

Si determina que es falso (else), ingresa por el camino de la izquierda y le muestra al usuario el mensaje de que no aplica al descuento y mostrar a continuacion el mensaje final con el valor original al no haberse aplicado el descuento.

---

#### ESTRUCTURA CONDICIONAL MÚLTIPLE (SWITCH)

Esta estructura nos permite evaluar la condición y comparar su valor con una lista de casos, si el valor coincide con alguno de estos casos, se ejecutara ese bloque de código.

##### Ejemplo Práctico:

###### Diagrama de Flujo:

<p align="left">
  <img src="https://drive.google.com/uc?export=view&id=1T45EJZ3M_0lK4JA5PJfwltqmIh-Tm_t-" alt="Descripción" width="150%">
</p>

<p style="text-align:center; font-size:12px;">Fig. 6. Diagrama de Flujo para la demostracion de la Estructura Condicional Múltiple. (Elaboración Propia). </p>

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

#### Explicación:

Como se ve en el diagrama de flujo, primero definimos las variables, luego de eso se pide al usuario ingresar los dos números y el operador que se desea.

Ahora, seguimos con la estructura del switch, si el usuario escribe un operador que coincida con los diferentes casos (+, -, *, /). Según con cual coincida ejecutara la operación que este dentro de ese caso.

Si ingresa un operador que no coincide con ningún caso, se le mostrara un mensaje de que el operador es inválido.

---

### ESTRUCUTRAS REPETITIVAS

---

#### ESTRUCTURA REPETITIVA (WHILE)








