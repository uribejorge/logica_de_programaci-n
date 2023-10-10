<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 3 


## Actividad 3: Ejercicios de operaciones básicas en Java.
1. Suma y multiplicación: Escribe un programa que solicite al usuario dos números enteros y luego imprima la suma y multiplicación de esos números.

2. Resta y división: Escribe un programa que tome dos números enteros ingresados por el usuario y calcule la resta y división de esos números.

3. Operaciones combinadas: Escribe un programa que solicite al usuario tres números enteros y realice las siguientes operaciones: suma de los tres números, multiplicación del primer número por el segundo y división del resultado entre el tercer número.

4. Operaciones con decimales: Escribe un programa que solicite al usuario dos números decimales y realice las siguientes operaciones: suma, resta, multiplicación y división.

5. Incremento y decremento: Escribe un programa que declare una variable entera y la inicialice con un valor. Luego, incrementa su valor en 1 y muestra el resultado. Después, decrementa su valor en 1 y muestra el resultado nuevamente.

6. Operador de asignación compuesta: Escribe un programa que declare una variable entera y la inicialice con un valor. Utiliza el operador de asignación compuesta para sumar 5 a la variable y luego mostrar su valor.

7. operadores lógicos: Escribe un programa que tome dos valores booleanos ingresados por el usuario y muestre el resultado de las operaciones lógicas AND, OR y NOT entre esos valores.

8. Operador ternario: Escribe un programa que tome un número entero ingresado por el usuario y utilice el operador ternario para determinar si el número es positivo o negativo. Luego, muestra el resultado en la salida.


## SOLUCIÓN



1. ## Suma y multiplicacion.

```

/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad1logica;
import java.util.Scanner;

/**
 *
 * @author USer
 */
public class Actividad1logica {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        Scanner scanner = new Scanner(System.in);
        
        
        System.out.print(
       
"Ingrese el primer número entero: ");
        int numero1 = scanner.nextInt();
        
        System.out.print("Ingrese el segundo número entero: ");
        int numero2 = scanner.nextInt();

        
       
int suma = numero1 + numero2;
        int multiplicacion = numero1 * numero2;

        // Imprimir los resultados
        System.out.println(
       
"La suma de los números es: " + suma);
        
        System.out.println (

        
"La multiplicación de los números es: " + multiplicacion);
        
        // Cerrar el objeto Scanner
        scanner.close();    
    }
}

```
2. ## Resta y división:

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad2logica;
import java.util.Scanner;

/**
 *
 * @author USer
 */
public class Actividad2logica {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        Scanner Scanner = new Scanner(System.in);
        
        
        System.out.print(
     " ingrese el primer numero entero: ");
          int numero1 = Scanner.nextInt();
          
          System.out.print("ingrese el segundo numero entero: ");
          int numero2 = Scanner.nextInt();
        
          
          
          int resta = numero1 - numero2; 
          double division =numero1 / numero2;
          
          
          System.out.println( "la resta de los numeros es: " +  resta );
          System.out.println("");
          System.out.println("");
          
          System.out.println(
                  "la division de los numeros es: " + division);
          
                  
                Scanner.close();  

    }
}

```
3. ## Operaciones combinadas:

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad3logica;

import java.util.Scanner;

/**
 *
 * @author USer
 */
public class Actividad3logica {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        Scanner scanner = new Scanner(System.in);
        
        // Solicitar al usuario tres números enteros
        System.out.print(
       
"Ingrese el primer número entero: ");
        int numero1 = scanner.nextInt();
        
        System.out.print("Ingrese el segundo número entero: ");
        int numero2 = scanner.nextInt();
        
        System.out.print("Ingrese el tercero número entero: ");
        int numero3 = scanner.nextInt();
        
        
        // Calcular la suma de los tres numeros
        
       
int suma = numero1 + numero2 + numero3;
        int multiplicacion = numero1 * numero2;
        double division = multiplicacion / numero3;

        // Imprimir los resultados
        System.out.println(
       
"La suma de los números es: " + suma);
        
        System.out.println (

        
"La multiplicación de los números es: " + multiplicacion);
        
        // Cerrar el objeto Scanner
        
        System.out.println("la division de la operacion es " + division);
        
        scanner.close(); 
        
        
    }
}

```
4. ## Operaciones con decimales:

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad4logica;

import java.util.Scanner;


/**
 *
 * @author USer
 */
public class Actividad4logica {
    
    
    public static void main(String[] args) {
        System.out.println("Hello World!");
        Scanner scanner = new Scanner(System.in);
        
        // Solicitar al usuario tres números enteros
        System.out.print(
       
"Ingrese el primer número entero: ");
        double numero1 = scanner.nextDouble();
        
        System.out.print("Ingrese el segundo número entero: ");
        double numero2 = scanner.nextDouble();
        
        
       
double suma = numero1 + numero2 ;
double resta = numero1 - numero2;
double multiplicacion = numero1 * numero2;
double division = numero1 / numero2;

        // Imprimir los resultados
        System.out.println(
       
"La suma de los números es: " + suma);
        
        System.out.println (
                
 "La resta de los números es: " + resta);
        
        System.out.println(
                
 "La multiplicacion de los números es: " + multiplicacion );
        
        System.out.println(
                 "la division de los numeros es: " +  division );
        
        
       
        
        scanner.close(); 
        
    }
}

```
5. ### Incremento y decremento:

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad5logica;
import java.util.Scanner;


/**
 *
 * @author USer
 */
public class Actividad5logica {
    
    

    public static void main(String[] args) {
        System.out.println("Hello World!");
        Scanner scanner = new Scanner(System.in);
        
        int numero = 9;

        
        System.out.println(
         numero);
        numero++;
        
        

        

        System.out.println("Después de incrementar: " +numero++);

        
        int numerodecrementar = numero - 3;
        System.out.println("Después de decrementar: " + numerodecrementar);
        

        
       
        
        scanner.close(); 
        
    }
}

```

6. ## Operador de asignación compuesta: 

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad6logica;
import java.util.Scanner;


/**
 *
 * @author USer
 */
public class Actividad6logica {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        
        
        int numero = 10;

        

        numero += 
        numero += 5;

        
        System.out.println("El valor después de sumar 5 es: " + numero);
        
        
    }
}

```
7. ### operadores lógicos:

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad7logica;
import java.util.Scanner;


/**
 *
 * @author USer
 */
public class Actividad7logica {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        
        Scanner scanner = new Scanner(System.in);


        System.out.print(
        
"Ingrese el primer valor booleano (true o false): ");
        
       
boolean valor1 = scanner.nextBoolean();

        System.out.print(

        


       "Ingrese el segundo valor booleano (true o false): ");
        boolean valor2 = scanner.nextBoolean();

        

        boolean resultadoAND = valor1 && valor2;
        boolean resultadoOR = valor1 || valor2;
        
       
boolean resultadoNOT1 = !valor1;
        
       
boolean resultadoNOT2 = !valor2;

        

        System.out.println(
        
"Resultado de la operación AND: " + resultadoAND);
        System.out.println(
        
"Resultado de la operación OR: " + resultadoOR);
        System.out.println(
        
"Resultado de la operación NOT para el primer valor: " + resultadoNOT1);
        System.out.println(
        

       
"Resultado de la operación NOT para el segundo valor: " + resultadoNOT2);

        
        scanner.close();
    }
}

```
8. ## Operador ternario:

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad8logica;
import java.util.Scanner;

/**
 *
 * @author USer
 */
public class Actividad8logica {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        
        
        

        
Scanner scanner = new Scanner(System.in);

        

       

        System.out.print(
       
"Ingrese un número entero: ");
        int numero = scanner.nextInt();

        


        String resultado = (numero >= 0) ? "positivo" : "negativo";

        

       

        System.out.println(
        
"El número es " + resultado);

        


        scanner.close();

    }
}
```
