## 💾📝CONTENIDOS DE LA UNIDAD 2

### ESTRUCUTRAS CONDICIONALES

---

#### ESTRUCTURA CONDICIONAL SIMPLE (IF)

Esta estructuras se la denomina simple por que evalua una sola condición, si determina que es verdadera ejecuta la instruccion dentro de la condición, si es falsa, lo ignora y continua con el resto de código que no este en la condición.

##### Ejemplo en C:

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


