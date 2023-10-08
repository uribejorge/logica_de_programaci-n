<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 5 


## Actividad 5: Ejercicios de bucles
Resolver los siguientes ejercicios:

#### Ejercicios - while
- Pedir al usuario que ingrese un número y mostrar su tabla de multiplicar hasta el número 10.
- Pedir al usuario que ingrese una cadena de caracteres y contar la cantidad de caracteres que son números.
### Ejercicios - do while
- Escribe un programa en Java que imprima los números del 1 al 100, pero que se detenga si el usuario introduce un número negativo.
- Escribe un programa en Java que pida al usuario un número entero e imprima la tabla de multiplicar de ese número, pero que se detenga si el usuario introduce el número 0.
### Ejercicios - for
- Imprimir los números impares del 1 al 50.
- Imprimir los números primos del 1 al 100.

## Solución

- Pedir al usuario que ingrese un número y mostrar su tabla de multiplicar hasta el número 10.
```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividadelogica5;
import java.util.Scanner;
/**
 *
 * @author USer
 */
public class Actividadelogica5 {

    public static void main(String[] args) {
    Scanner scanner = new Scanner(System.in); {
            System.out.print("Ingresa un número: ");{
            int numero = scanner.nextInt();
            
            System.out.println("Tabla de multiplicar del " + numero + ":");
            
            for (int i = 1; i <= 10; i++) {
                int resultado = numero * i;
                System.out.println(numero + " x " + i + " = " + resultado);
            }
        }
    }
}
    }
```
2. ## Pedir al usuario que ingrese una cadena de caracteres y contar la cantidad de caracteres que son números.
```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad5delogicajorgeuribe;
import java.util.Scanner;
/**
 *
 * @author USer
 */
public class Actividad5delogicajorgeuribe {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        
       Scanner scanner = new Scanner(System.in);

        // Solicitar al usuario ingresar una cadena de caracteres
        System.out.print("Ingrese una cadena de caracteres: ");
        String cadena = scanner.nextLine();

        // Inicializar el contador de números
        int contadorNumeros = 0;

        // Recorrer la cadena y contar los caracteres que son números
        for (int i = 0; i < cadena.length(); i++) {
            char caracter = cadena.charAt(i);
            if (Character.isDigit(caracter)) {
                contadorNumeros++;
            }
        }

        // Mostrar la cantidad de caracteres que son números
        System.out.println("La cantidad de caracteres que son números en la cadena es: " + contadorNumeros);

        scanner.close();
    }
}
```

## Ejercicios - do while
- Escribe un programa en Java que imprima los números del 1 al 100, pero que se detenga si el usuario introduce un número negativo.
```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad5jorgeuribelogica;
import java.util.Scanner;
/**
 *
 * @author USer
 */
public class Actividad5jorgeuribelogica {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        System.out.println("Números primos del 1 al 100:");
        
        for (int numero = 2; numero <= 100; numero++) {
            if (esPrimo(numero)) {
                System.out.print(numero + " ");
            }
        }
    }
    
    // Método para verificar si un número es primo
    public static boolean esPrimo(int num) {
        if (num <= 1) {
            return false;
        }
        
        if (num <= 3) {
            return true;
        }
        
        if (num % 2 == 0 || num % 3 == 0) {
            return false;
        }
        
        for (int i = 5; i * i <= num; i += 6) {
            if (num % i == 0 || num % (i + 2) == 0) {
                return false;
            }
        }
        
        return true;
    }
}

```

- ## Escribe un programa en Java que pida al usuario un número entero e imprima la tabla de multiplicar de ese número, pero que se detenga si el usuario introduce el número 0.
```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad5logicajorgeuribe;
import java.util.Scanner;
/**
 *
 * @author USer
 */
public class Actividad5logicajorgeuribe {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        
       Scanner scanner = new Scanner(System.in);
        
        int numero;
        
        do {
            System.out.print("Ingrese un número entero (0 para salir): ");
            numero = scanner.nextInt();
            
            if (numero != 0) {
                System.out.println("Tabla de multiplicar del " + numero + ":");
                for (int i = 1; i <= 10; i++) {
                    System.out.println(numero + " x " + i + " = " + (numero * i));
                }
            }
        } while (numero != 0);
        
        System.out.println("Programa detenido.");
        
        scanner.close();
    }
}
```
## Ejercicios - for
- ## Imprimir los números impares del 1 al 50.
```

/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad5jorgeuribe;
import java.util.Scanner;
/**
 *
 * @author USer
 */
public class Actividad5jorgeuribe {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        System.out.println("Números impares del 1 al 50:");
        
        for (int i = 1; i <= 50; i += 2) {
            System.out.println(i);
        }
    }
}
```
- ### Imprimir los números primos del 1 al 100.
```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad5jorgeuribelogica;
import java.util.Scanner;
/**
 *
 * @author USer
 */
public class Actividad5jorgeuribelogica {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        System.out.println("Números primos del 1 al 100:");
        
        for (int numero = 2; numero <= 100; numero++) {
            if (esPrimo(numero)) {
                System.out.print(numero + " ");
            }
        }
    }
    
    // Método para verificar si un número es primo
    public static boolean esPrimo(int num) {
        if (num <= 1) {
            return false;
        }
        
        if (num <= 3) {
            return true;
        }
        
        if (num % 2 == 0 || num % 3 == 0) {
            return false;
        }
        
        for (int i = 5; i * i <= num; i += 6) {
            if (num % i == 0 || num % (i + 2) == 0) {
                return false;
            }
        }
        
        return true;
    }
}
```



