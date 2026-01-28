## 💾📝CONTENIDOS DE LA UNIDAD 3

### 🧩🍱 MODULARIDAD

---

#### 📋🛡️Pase de párametro por Valor

---

Este método trata de que creamos una copia del valor de una variable, a esa copia se la pasa a otra función y cualquier cambio que se realice dentro de esa funcion no afecta a la variable original ya que esta fuera de esa función.

##### 🧑‍💻 Ejemplo Práctico:

###### Código en C:

```

#include <stdio.h>

float calculoPotencia(float v, float i){

    float p = v * i;

    return p;
}

int main(){

    float voltaje = 3.3;
    float corriente = 1.2;

    float potencia = calculoPotencia(voltaje, corriente);

    printf("La Potencia calculada es de: %.2f", potencia);

    return 0;
}

```

#### 💡Explicación:

Como se puede visualizar, en este código se usa la modularidad diviéndolo en dos funciones "main" y "calculoPotencia", esta última funcion recibe los datos de voltaje y corriente por el método de pase por valor, en esta función declaramos los párametros como float v y float i para que este lista para recibir y almacenar números decimales creando así recipientes para las copias de los datos originales y operar de forma segura. El resultado de esta operación regresa a la función "main" para ser mostrada en pantalla.

---

#### 📍☁️ Pase de párametro por Referencia

---

Por otro lado, en este método no se envian copias de las variables, sino que enviamos la dirección de memoria de la variable, esto es lo que permite que la función acceda directamente al valor original y puede modificarlo, en C usamos punteros ("*" y "&").

##### 🧑‍💻 Ejemplo Práctico:

###### Código en C:


```

#include <stdio.h>

void procesoVenta(int *stockDisponible, int cantidadVendida){

    if (*stockDisponible >= cantidadVendida){

        *stockDisponible = *stockDisponible - cantidadVendida;

        printf("Venta exitosa\n");
    }else{
        printf("Stock insuficiente\n");
    }
}

int main(){

    int stockCamisas = 50; 
    int ventaRealizada = 12;

    printf("Inventario inicial: %i unidades\n", stockCamisas);

    procesoVenta(&stockCamisas, ventaRealizada);

    printf("Inventario actualizado: %i unidades\n", stockCamisas);

    return 0;
}

```

#### 💡Explicación:

Aquí tambien usamos la modularidad para dividir en dos funciones, y aplicamos el pase por referenica para manejar eficientemente el inventerio de un sistema. Como se menciono en el pase por referencia la variable en este caso "procesoVenta" recibe la dirección de memoria de la variable orginal utilizando el puntero "int *stockDisponible", y como usamos el operador "&" en la función main le damos permiso a la función para que acceda y modifique el valor almacenado y con las estructuras condicionles controlamos que se realicen cálculos válidos.

---

### 🚃🗄️ARREGLOS

---

#### 🎞️📏 Arreglo Unidimensional o Vector 

---

Este tipo de arreglos se caracteriza por que tienen una sola fila y varias columnas en el cual las posiciones de este arreglo empiezan en cero y se los llama índices.

##### 🧑‍💻 Ejemplo Práctico:

###### Código en C:

```

#include <stdio.h>

int main(){

    float voltajes[5] = {3.3, 3.5, 3.2, 3.4, 3.3};
    
    printf("Registro de Voltajes:\n");

    for(int i = 0; i < 5; i++) {

        printf("Lectura %i: %.1f V\n", i + 1, voltajes[i]);
    }

    return 0;

}

```

#### 💡Explicación:

Como se puede observar, usamos un arreglo unidimensional, cuando declaramos "float voltajes[5]" le decimos al programa que reserve 5 espacios seguidos en la memoria, asignandole a cada espacio un número de índice para luego ser encontrado más fácil y con el "for" recorremos los casilleros automáticamente para mostrar el contenido guardado.

---

#### 🗓️🏁 Arreglo Bidimensional o Matriz 

---

Este otro tipo de arrelgo se caracteriza por que tiene varias filas y columnas y su representación es m[i][j], en la cual i es el número de filas y j el número de columnas.

##### 🧑‍💻 Ejemplo Práctico:

###### Código en C:

```

#include <stdio.h>

int main() {
    int laboratorio[3][3] = {
        {1, 0, 1}, 
        {0, 1, 0}, 
        {1, 1, 1}  
    };

    printf("Estado del Laboratorio (0:Libre, 1:Ocupado)\n");

    for(int i = 0; i < 3; i++) {
        for(int j = 0; j < 3; j++) {
            printf("[%d] ", laboratorio[i][j]);
        }
        printf("\n"); 
    }

    return 0;
}

```

#### 💡Explicación:

En este ejemplo usamos el arreglo bidimensional para representar el estado de los laboratorios de computación, cunado declaramos "int laboratorios[3][3]", el programa reserva los espacios y además organiza los datos en una cuadrículas con filas y columnas, en este caso es una matriz 3x3, para acceder a los datos utilizamos los índices uno para filas y otro para columnas, y con el los ciclos que están anidados recorremos la tabla completa.

---

#### 🧊📚 Arreglo Tridimensional 

---

Este arreglo esta caracterizado por que tiene filas, columnas y profundidad, se lo representa como m[i][j][k] donde i es la profundidad, j es el número de filas y k es el número de columnas.

##### 🧑‍💻 Ejemplo Práctico:

###### Código en C:

```

#include <stdio.h>

int main() {

    float notas[2][2][2] = {
        {{8.5, 9.0}, {7.0, 8.2}}, 
        {{9.5, 8.8}, {6.5, 7.5}}  
    };

    printf("NOTAS\n");


    for (int i = 0; i < 2; i++) {        
        for (int j = 0; j < 2; j++) {     
            for (int k = 0; k < 2; k++) { 
                printf("Nota: %.1f\n", notas[i][j][k]);
            }
        }
    }

    return 0;
}

```

#### 💡Explicación:

Para este ejemplo usamos el arreglo tridimensional que organiza en capas, cuando declaramos "float notas[2][2][2]" le decimos al programa que vamos a tener 2 capas, 2 filas y 2 columnas, y asi reserva espacios en la memoria en odnde cada valor se identifica mediante 3 índices que con ayuda de los 3 "for" anidados recorren de manera automática toda la estrucutra para mostrar la información de manera ordenada.

---

### ⚠️🤔 PRINCIPALES DIFICULTADES EN LA APLICACIÓN DE LOS CONTENIDOS 

En esta unidad se me dificulto un poco aprender como hacer los pases por referencia y por valor, cuando y como usar los punteros para hacer los pases por referencia y también se me dificulo aprender a como invocar funciones que estan fuera del main.

---

### 🧠💡 REFLEXIÓN CRÍTICA DE LOS APRENDIZAJES DE LA UNIDAD 

La unidad me permitio ver que pasar de una programación simple a una programación lógica y organizada es muy importante, además, de que el domino de la memoria a través de punteros y la jerarquización de datos mediante arreglos multidimensionales son aprendizajes que me serviran mucho en mi formación como ingeniero en computación.

---

### 📋 ANEXOS

🗨️ [Ejercicios de la U3](https://drive.google.com/drive/folders/1mhOx9bjmWn1IUFQxHCDZ_GvRwpzb-qE7?usp=sharing)

---

<p align="right">
  <a href="index.md">Volver a la página principal</a>
</p>


