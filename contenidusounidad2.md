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

<p style="text-align:center; font-size:12px;">Fig. 4. Diagrama de Flujo para la demostracion de la Estructura Condicional. (Elaboración Propia). </p>

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

Como se puede observar en el diagrama de flujo, el algoritmo empieza definiendo las variables, luego le pide al usuario ingresar el valor de su compra, a continuación sigue con la condición, que evalua si el valor de la compra es mayor o igual a 100. Si determina que sí lo es, ingresa en el camino de la derecha y muestra el mensaje del descuento, continuando realiza los calculos para aplicar el 20% al valor de la compra y mostrar el mensaje final.

Si determina que la compra es menor a 100 doláres, ignora el "if" y muestra el mensaje final.

---

#### ESTRUCTURA CONDICIONAL DOBLE (IF-ELSE)





