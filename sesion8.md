<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 8 


## Actividad: Ejecicios de métodos en Java
#### Implementar los siguientes métodos:

1. Escribe un método que reciba dos números como parámetros y devuelva el mayor de los dos.
2. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de vocales que contiene.
3. Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las letras mayúsculas en minúsculas y viceversa.
4. Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de palabras que contiene.
5. Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las palabras en orden alfabético.


## SOLUCIÓN


1. ### Escribe un método que reciba dos números como parámetros y devuelva el mayor de los dos.

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad8metodosyava;
import java.util.Scanner;
/**
 *
 * @author USer
 */
public class Actividad8metodosyava {

 public static int obtenerMayor(int numero1, int numero2) {
        if (numero1 > numero2) {
            return numero1;
        } else {
            return numero2;
        }
    }

    public static void main(String[] args) {
        int numero1 = 10;
        int numero2 = 20;

        int mayor = obtenerMayor(numero1, numero2);

        System.out.println("El número mayor entre " + numero1 + " y " + numero2 + " es: " + mayor);
    }
}

```

2. ### Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de vocales que contiene.

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad8vocales;
import java.util.Scanner;
/**
 *
 * @author USer
 */
 public class Actividad8vocales{

    public static int Actividad8vocales (String texto) {
    
        texto = texto.toLowerCase();
        
        int contador = 0;

        for (int i = 0; i < texto.length(); i++) {
            char caracter = texto.charAt(i);
            
            if (caracter == 'a' || caracter == 'e' || caracter == 'i' || caracter == 'o' || caracter == 'u') {
                contador++;
            }
        }

        return contador;
    }

    public static void main(String[] args) {
        String texto = "Esta es una cadena de ejemplo con vocales";
        
        int numeroDeVocales = Actividad8vocales (texto);
        
        System.out.println("El número de vocales en la cadena es: " + numeroDeVocales);
    }
}

```
3.  ### Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las letras mayúsculas en minúsculas y viceversa.

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad8cadenasmayusculasminusculas;
import java.util.Scanner;
/**
 *
 * @author USer
 */
public class Actividad8cadenasmayusculasminusculas {

   

    public static String cambiarMayusculasMinisculas(String texto) {
        StringBuilder resultado = new StringBuilder();

        for (int i = 0; i < texto.length(); i++) {
            char caracter = texto.charAt(i);
            if (Character.isUpperCase(caracter)) {
                resultado.append(Character.toLowerCase(caracter));
            } else if (Character.isLowerCase(caracter)) {
                resultado.append(Character.toUpperCase(caracter));
            } else {
                resultado.append(caracter);
            }
        }

        return resultado.toString();
    }

    public static void main(String[] args) {
        String texto = "Ejemplo De Cadena Con Mayúsculas y Minúsculas";
        
        String textoCambiado = cambiarMayusculasMinisculas(texto);
        
        System.out.println("Texto original: " + texto);
        System.out.println("Texto con mayúsculas y minúsculas intercambiadas: " + textoCambiado);
    }
}

```
4. ### Escribe un método que reciba una cadena de texto como parámetro y devuelva el número de palabras que contiene.

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad8metododepalabras;
import java.util.Scanner;
/**
 *
 * @author USer
 */
public class Actividad8metododepalabras {

     
 public static int Actividad8metododepalabras (String texto) {
        
        String[] palabras = texto.split(" ");
        
    
        return palabras.length;
    }

    public static void main(String[] args) {
        String texto = "Esta es una cadena de ejemplo con varias palabras";
        
        int numeroDePalabras = Actividad8metododepalabras(texto);
        
        System.out.println("El número de palabras en la cadena es: " + numeroDePalabras);
    }
}

```
5. ### Escribe un método que reciba una cadena de texto como parámetro y devuelva una nueva cadena con todas las palabras en orden alfabético.

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.actividad8metodoalfabetico;
import java.util.Arrays;
/**
 *
 * @author USer
 */
public class Actividad8metodoalfabetico {

   public static String ordenarPalabras(String texto) {

        String[] palabras = texto.split(" ");
        
    
        Arrays.sort(palabras);
        
        
        String resultado = String.join(" ", palabras);
        
        return resultado;
    }

    public static void main(String[] args) {
        String texto = "Esta es una cadena de ejemplo con palabras desordenadas";
        
        String textoOrdenado = ordenarPalabras(texto);
        
        System.out.println("Texto original: " + texto);
        System.out.println("Texto con palabras ordenadas alfabéticamente: " + textoOrdenado);
    }
}

```