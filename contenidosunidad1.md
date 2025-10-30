## 💾📝CONTENIDOS DE LA UNIDAD 1

### 🚪🧠 ***Algoritmos, pseudocódigo, diagramas de flujo***

Los algoritmos son pasos secuenciales que siguen una lógica, que permiten resolver problemas específicos.
Estos algoritmos se dividen en dos categorías: 

##### 🔡 Algoritmos Cualitativos

Son los que se concentran en el "qué" de las cosas, los pasos de estos algoritmos están escritos de forma textual sin ninguna fórmula matemática, como puede ser una receta de cocina [1].

##### 🔢 Algoritmos Cuantitativos

Son los algoritmos que usan las fórmulas algebraicas y cálculos númericos para resolver los problemas que sean propuestos como sumas, restas, multiplicaciones, divisiones [2].

---

 #### 📝🧠 ***Pseudocódigo***

El pseudocódigo es la base para entrar al mundo de la programación, porque este programa es utilizado en escuelas, colegios, universidades. Permite escribir instrucciones en nuestro lenguaje a un lenguaje en el que la computadora logre entenderlo y procese lo que necesitamos para resolver los problemas que propongamos.

---

#### 📄 *Ejercicio Práctico*

Para demostrar lo que es el pseudocódigo utilizaremos el siguiente problema el cual requiere saber que cambio recibira el consumidor por la compra de un producto:

```
Algoritmo cambio_a_recibir

	Definir cambio, cantidadDeDineroDisponible, costoDelProducto Como Real;
	
	//Datos de entrada
	
	Escribir "Ingrese el dinero que dispone: ";
	Leer cantidadDeDineroDisponible;
	
	Escribir "Ingrese el costo del producto: ";
	Leer costoDelProducto;
	
	//Proceso 
	
	cambio= cantidadDeDineroDisponible - costoDelProducto;
	
	//Datos de salida
	
	Escribir "El cambio a recibir por la compra del producto es: ", cambio;

FinAlgoritmo

```

  ---

#### 🤓 *Explicación del código:*

➥ Primero se debe definir las variables, en este caso se definieron como Real las tres variables.

➥ Dentro del código se veran "//" es una función la cual permite escribir comentarios por ejemplo de guía, estos comentarios no afectan en la ejecución del programa.

➥ Como segundo paso usaremos la funcion "Escribir" que lo que hara es mostrar el texto guia para que el usuario vea que tiene que anotar en ese apartado.

➥ El tercer paso es  usar la funcion "Leer" y luego la variable a la cual será asignada el dato que el usuario lo escribirá en ese apartado.

➥ En el cuarto paso se repetira lo mismo del paso 2 y 3 en el mismo orden, únicamente cambiando el mensaje a mostrar y la variable.

➥ Definidas las variables continuaremos con el cálculo, escribimos la variable, luego de eso un "=" lo que significa que lo escrito luego de ese igual es el valor que se le asignara a la variable, en este caso una resta para encontrar el valor del cambio a recibir.

➥ Definida la fórmula que dara el resultado, volveremos a usar la funcion "Escribir" para mostrar el mensaje final, seprando con una coma y luego la variable, lo cual  mostrara al usuario el resultado de la operación, en este caso, el cambio que recibirá por la compra de su producto.

---

#### *Pruebas de Escritorio*

| N° | Dinero Disponible | Costo del Producto | Operación | Resultado |
| :--- | :---: | :---: | :---: | ---: |
| 1    | $50   | $35   | cambio= 50 - 35 | $15 |
| 2    | $80   | $25   | cambio= 80 - 25 | $55 |
| 3    | $67   | $45   | cambio= 67 - 45 | $22 |


---

#### 💠👇🌊 ***Diagrama de flujo***

Son aquellos que describen procesos mediante diagramas, son utilizados para facilitar la lectura de los procesos, estos diagramas utilizan figuras en las cuales cada figura cumple un rol, acompañadas de flechas que ayudan a revisar la secuencia de los pasos [3]. En resumen facilitan la lectura de los procesos y agiliza la toma de decisiones. 

#### 📄 *Ejercicio Práctico*

Ahora para demostrar lo que es el diagrama de flujo usaremos el mismo ejemplo que en el pseudocódigo.

<p align="center">
  <img src="https://drive.google.com/uc?id=1OI--OIPueuTOHYwLQBicntgUm2ADjmMs" alt="Descripción" width="35%">
</p>

---

#### 🤓 *Explicación del diagrama* 

🔵 Muestra la estructura del algoritmo de forma visual.

🔵 Las cajas punteadas de gris representan  las anotaciones o comentarios.

🔵 La figura del rectángulo representa la función "Asignar".

🔵 Las figuras de paralelogramos funcionan tanto como la función "Escribir " que sería el paralelogramo en verde y la función "Leer" que sería el paralelogramo en rojo.

🔵 Las flechas demuestran el flujo y secuencia que sigue el algoritmo.

---

### 🦺🧱 ***Programación por bloques*** 

En este entorno las instrucciones están escritas en bloques, para construir los programas se deben arrastrar los bloques y juntarlos a otros, este tipo de programación tiene una mayor ventaja que la programación escrita, por el simple hecho de que aqui se evitan los errores de sintaxis muy comunes en lo escrito, es por eso que en este modo de programar el programador se concentra únicamente en la construcción del algoritmo razón por la cual es muy utilizada en institutos de educacion para introducir a los estudiantes a conceptos básicos y al mundo de la progrmacion [4].

<p align="center">
  <img src="https://drive.google.com/uc?id=1-ElZ1z_ib5P8S3YJVHsf6-lSRKNo1ieb" alt="Descripción" width="75%">
</p>

---

#### 🤓 *Explicación práctica de la programación por bloques*

En la imágen se muestra una estructura simple de un algoritmo construido por bloques. En el que se visualizan dos bloques:

☑️ Bloque de Inicio: Es el bloque de verde, quien es el que da comienzo a la ejecucion del programa, cuando se haga clic a ejectuar, todo lo que este dentro o conectado al bloque de verde dara inicio su ejecución.

☑️ Bloques de accion: En este caso son los 6 bloques verdes contenidos en el bloque de inicio, son los bloques que le dan las instrucciones individuales las cuales el personaje realizará para moverse dentro del campo.

La forma en que estan apilados los bloques (de abajo hacia arriba) demuestran la secuencia y el orden en el que se ejecutara cada acción.


---

### 💡***Ejemplos de algoritmos con estructuras lineales/secuenciales***

Para esta sección elegí un algoritmo que permita calcular el promedio de las notas de un estudiante, pasará de estar escrito en PSeint al lenguaje de programación C.

Algoritmo en PSeint:

```
Algoritmo promedioNotas
	
	Definir nota1, nota2, nota3, promedio como Real;
	
	//Datos de entrada
	
	Escribir "Ingresa el valor de la nota 1: ";
	Leer nota1;
	
	Escribir "Ingresa el valor de la nota 2: ";
	Leer nota2;
	
	Escribir "Ingrese el valor de la nota 3: ";
	Leer nota3;
	
	//Proceso 
	
	promedio = (nota1 + nota2 + nota3) / 3;
	
	//Datos de salida
	
	Escribir "EL promedio de las notas es: ", promedio;

FinAlgoritmo

```

---

#### 🤓 Explicación del código

Para este algoritmo primero se le muestra al usuario el mensaje para que ingrese el valor de su primera nota, y asi llene los dos campos restantes con los valores de las notas, a continuacion viene la fórmula para sacar el promedio que seria sumando las 3 notas y diviendolas para 3 en este caso, con la fórmula planteada procedemos a escribir el mensaje final donde se mostrará el resultado de la operacion, siendo el promedio de las 3 notas.

---

### Código en C

```
#include <stdio.h>

int main() {


    float nota1;
    float nota2;
    float nota3;
    float promedio;

    //Datos de Entrada

    printf("Ingrese el valor de la nota 1: \n");
    scanf("%f", &nota1);

    printf("Ingrese el valor de la nota 2: \n");
    scanf("%f", &nota2);

    printf("Ingrese el valor de la nota 3: \n");
    scanf("%f", &nota3);

    //Proceso 

    promedio = (nota1 + nota2 + nota3) / 3;

    //Datos de Salida

    printf("El valor del promedio de las notas es: %f\n", promedio);

    return 0;


}

```

---

#### 🤓 Explicación del Código

✤ Primero se debe incluir la biblioteca "<stdio.h>" ya que es la que permitira incluir las funciones "printf" y "scanf" que a su vez son necesarias para escribir los datos de entrada y salida.

✤ Luego se escribira "int main() {" que viene siendo el iniciador del programa, ya que "main" es el nombre de la función de C que permite el inicio y ejecución de todo lo que este escrito dentro de las llaves, cabe recalcar que en cada línea del código se terminara con un ";" que quiere decir que hasta ahi termina la instrucción.

✤ Como en PSeint primero se define las variables, pero en C hay un ligero cambio, ya que aqui primero se pone que tipo de variable será y luego el nombre de la variable, existen diferentes tipos de variables (int, float, double, char, bool).

✤ Continuando con el proceso ahora vienen los datos de entrada, en donde se usara "printf()" y "scanf()", el printf es similar al "Escribir" de PSeint, y el scanf es parecido al "Leer". En la linea del printf se usa "\n" para ejecutar un tipo de enter y la proxima función scanf se muestre debajo del texto, en esta función se usa la máscara "%f" para decirle al programa que se espera un valor tipo "float", seguido de esto se pone una coma, luego de la coma ira el simbolo "&" que le dice al programa que guarde el valor escrito por el usuario dentro de la varibale escrita luego de dicho simbolo.

✤ Una vez escrita esa parte se puede escribir la formula que resolvera el problema, aqui no hay mayor cambio con respecto a C, se escribe la variable seguido de un igual y luego el procedimiento que dara el valor que se asignara a la variable.

✤ Ahora vienen los datos de salida, usamos igualmente printf, pero hay un cambio ya que luego de escribir el mensaje final se escribe la máscara "%f" que es como si diera un espacio reservado para el resultado, seguido de esto se pone una coma y la variable, con eso se le dira a printf que variable debe ir en el espacio reservado por la máscara escrita previamente.

✤ Por último el "return 0;" le dice el programa que "main" termino sin problemas, y se cierra el código con "}" (Continuacion de la llave del inicio).

---

#### Pruebas de escritorio 

| N°1 | Nota 1 | Nota 2 | Nota 3 | Proceso | Resultado |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 8.9 | 9.9 | 6.9 | promedio = (8.9 + 9.9 + 6.9) / 3 | 8.56 |
| 2 | 10 | 7.55 | 8.9 | promedio =(10 + 7.55 + 8.9) / 3 | 8.81 |
| 3 | 9.5 | 4.6 | 7.7 | promedio = (9.5 + 4.6 + 7.7) / 3| 7.26 |


---

### 🤔🛑 ***Principales dificultades en la aplicación de los contenidos***

Dentro de la materia he tenido dificultad para adaptarme a los símbolos usados tanto en PSeint como en el lenguaje de C, además de eso cuando escribía mi código en C a veces no compilaba, y se me complico un poco usar los nuevos términos de C ya que en PSeint se escribe con términos diferentes y que en C se escribe las líneas de código en inglés mientras que en PSeint se lo hace en español.

---


### ✨✍️ ***Reflexión crítica de los aprendizajes de la unidad***

Para finalizar, en esta unidad he aprendido muchos términos nuevos y los conceptos básicos de la programación, como del pseudocódigo se puede pasar al lenguaje de programación y hacer un programa mucho más avanzado. Esta unidad me ayudo a aprender la lógica que siguen los programas, como se debe estructurarlos y como ser ordenado en todo aspecto mejora mucho la efectividad y eficiencia al momento de realizar alguna tarea.

---

### 📸 *Anexos*

🔎 [Actividades PSeint](https://drive.google.com/drive/folders/1RzWP6Gr5CPKaEf53AyLn-GCuPNheCflT?usp=sharing)

🔎 [Actividades PSeint Diagramas de Flujo](https://drive.google.com/drive/folders/12pXgqAJp3yEe0kTQveeYL6HXcfKj0qNv?usp=sharing)

🔎 [Actividades Programación por Bloques](https://drive.google.com/drive/folders/1BkyhZvw1LZubSUEDsrqpakbkp0FwE_FZ?usp=sharing)

🔎 [Ejericicios PSeint/C](https://drive.google.com/drive/folders/1eZEG4GpI1JA795921ehuytX2KHslluqt?usp=sharing)

🔎 [Ejercicios de C](https://drive.google.com/drive/folders/1WwCeyrolFfQ_Y8z_QAtsYR6tsRsWBmhv?usp=sharing)

--- 

<p align="right">
  <a href="index.md">Volver a la página principal</a>
</p>

