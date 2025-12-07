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

<p style="text-align:center; font-size:12px;">Fig. 2. Diagrama de Flujo para el Cálculo del Cambio (Elaboración Propia). </p>


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

En este código primero pedimos al usuario que ingrese el valor de su compra, una vez es ingresado y leído por la computadora, procede a evaluar si cumple con la condición, si el valor de la compra es de 100 dólares en adelante, se le mostrara un mensaje en el cual se menciona un descuento del 20%, se realizara el descuento del 20% al valor de su compra y se mostrara el precio final de la compra, si la compra es de menor a 100 dólares no se mostrare el mensaje del descuento, el programa ignora la instrucción del descuento y procede con la línea final en la que se muestra el precio final.

