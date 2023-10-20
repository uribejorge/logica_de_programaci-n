<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 11 


### Actividad: Ejercicios de Lógica de Programación
1. Basándose en el algoritmo 1 de la sesión 11, aplicar la siguiente variante: Dado un conjunto de números enteros, se debe determinar si existe algún número que aparezca más de una vez. Si es así, se deben imprimir todos los números que aparezcan más de una vez.

2. Desarrollar un algoritmo que realice la conversión de binario a decimal.

## SOLUCIÓN

## Ejercicio 1

Conversión de decimal a binario. La conversión de decimal a binario es el proceso de convertir un número decimal a su representación binaria. El sistema binario es un sistema de numeración basado en dos dígitos, 0 y 1.

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Project/Maven2/JavaApp/src/main/java/${packagePath}/${mainClassName}.java to edit this template
 */

package com.mycompany.actividad11;

/**
 *
 * @author CESDE
 */
public class Actividad11 {

    public static void main(String[] args) {
        System.out.println("Hello World!");
     

    
        
        int numeroDecimal = 10;

        
        String numeroBinario = "";

    
        int i = 0;
        while (numeroDecimal > 0) {

            
            int resto = numeroDecimal % 2;

            
            numeroBinario = resto + numeroBinario;

            
            numeroDecimal = numeroDecimal / 2;

        
            i++;
        }

        
        System.out.println("El número binario es: " + numeroBinario);
    }
}

```

## Ejercicio 2.

Dado un conjunto de números enteros, se debe determinar si existe un número que aparezca más de una vez. Si existe, se debe imprimir su valor.

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Project/Maven2/JavaApp/src/main/java/${packagePath}/${mainClassName}.java to edit this template
 */

package com.mycompany.ejercicio11enteros;

/**
 *
 * @author CESDE
 */
public class EJERCICIO11ENTEROS {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        

    
        
        int[] numeros = {1, 2, 3, 4, 5, 2, 7, 9};


        int numeroRepetido = 0;


        for (int i = 0; i < numeros.length; i++) {
            // Comprobamos si el número actual ya ha aparecido
            for (int j = 0; j < i; j++) {
                if (numeros[i] == numeros[j]) {
                    // El número actual ya ha aparecido
                    numeroRepetido = numeros[i];
                    break;
                }
            }
        }

        
        if (numeroRepetido != 0) {
            System.out.println("El número repetido es: " + numeroRepetido);
        } else {
        
            System.out.println("No hay ningún número repetido");
        }
    }
}

```

## Utilizando bucle for

```

/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Project/Maven2/JavaApp/src/main/java/${packagePath}/${mainClassName}.java to edit this template
 */

package com.mycompany.actividad;

/**
 *
 * @author CESDE
 */
public class Actividad {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        

    
        
        int numeroDecimal = 10;

        
        String numeroBinario = "";

        
        for (int i = numeroDecimal; i > 0; i /= 2) {

            
            int resto = i % 2;

            
            numeroBinario = resto + numeroBinario;
        }

        
        System.out.println("El número binario es: " + numeroBinario);
    }

    }

```




