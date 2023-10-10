<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 4


## Actividad 4: Ejercicios de control de flujo con expresiones compuestas

```
// Variables de tipo String
String nombre = "Juan Pérez";
String apellido = "González";
String identificación = "1000000001";
String correo = "juan.perez@ejemplo.com";
String carrera = "Desarrollo de Software";
String universidad = "Cesde";
// Variable de tipo int
int edad = 20;
// Variable de tipo boolean
boolean esActivo = true;
boolean becado = false;
// Variable de tipo char
char género = 'M';
// Variable de tipo double
double promedio = 4.5;
// Variable de tipo int
int semestre = 2;

```

#### Con la información anterior, implementa los siguientes ejercicios:

1. Determinar si el estudiante es mayor de edad y tiene un estado activo.
2. Determinar si el estudiante tiene una beca o una carrera relacionada con el desarrollo de software.
3. Determinar si el estudiante está en el último semestre de su - carrera y tiene un estado activo.
4. Determinar si el estudiante tiene una carrera relacionada con el desarrollo de software y un promedio superior a 4.0.
5. Mostrar toda la información del estudiante si está matriculado en el Cesde.
6. Asignar una beca del 50% si el estudiante está matriculado en el Cesde, tiene un promedio superior a 4.0 y está activo.
7. Determinar la cantidad de beca que recibe el estudiante según su promedio:
- 0.0 - 3.4: El estudiante no recibe beca.
- 3.5 - 3.9: El estudiante recibe una beca parcial del 25%.
- 4.0 - 4.4: El estudiante recibe una beca parcial del 50%.
- 4.5 - 5.0: El estudiante recibe una beca completa.

## Solución
1. ### Determinar si el estudiante es mayor de edad y tiene un estado activo.

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.ejercicio7;

import java.util.Scanner;

/**
 *
 * @author USer
 */
public class Ejercicio7 {

    public static void main(String[] args) {
        System.out.println("Hello World!");// Variables de tipo String
        Scanner scanner = new Scanner(System.in);
   
        System.out.print(true);
        
String nombre = "Juan Pérez";
String apellido = "González";
String identificación = "1000000001";
String correo = "juan.perez@ejemplo.com";
String carrera = "Desarrollo de Software";
String universidad = "Cesde";
// Variable de tipo int
int edad = 20;
// Variable de tipo boolean
boolean esActivo = true;
boolean becado = false;
if (edad >= 18 && esActivo) {
            System.out.println("El estudiante es mayor de edad y tiene estado activo.");
        } else {
            System.out.println("El estudiante no cumple con los requisitos.");

// Variable de tipo char
char género = 'M';
// Variable de tipo double
double promedio = 4.5;
// Variable de tipo int
int semestre = 2;

    
        
        }
    }
}

```
2. ### Determinar si el estudiante tiene una beca o una carrera relacionada con el desarrollo de software.

```
package com.mycompany.ejercicio10;
import java.util.Scanner;

/**
 *
 * @author USer
 */
public class Ejerciciodiez {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        
        // Variables de tipo String
String nombre = "Juan Pérez";
String apellido = "González";
String identificación = "1000000001";
String correo = "juan.perez@ejemplo.com";
String carrera = "Desarrollo de Software";
String universidad = "Cesde";
// Variable de tipo int

int edad = 20;
// Variable de tipo boolean
boolean esActivo = true;
boolean becado = false;

// Variables proporcionadas en tu código

// Variable de tipo char
char género = 'M';
// Variable de tipo double
double promedio = 4.5;
// Variable de tipo int
int semestre = 2;

        if (becado || carrera.equals(" Desarrollo de Software")) {
            System.out.println("El estudiante tiene una beca o está en una carrera relacionada con desarrollo de software.");
        } else {
            System.out.println("El estudiante no cumple con los requisitos.");
        }
    }
 
}

```
 3. ## Determinar si el estudiante está en el último semestre de su - carrera y tiene un estado activo  

```
      /*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.ejercicioonce;
import java.util.Scanner; 

/**
 *
 * @author USer
 */
public class Ejercicioonce {

    public static void main(String[] args) {
        System.out.println("Hello World!");
         // Variables de tipo String
String nombre = "Juan Pérez";
String apellido = "González";
String identificación = "1000000001";
String correo = "juan.perez@ejemplo.com";
String carrera = "Desarrollo de Software";
String universidad = "Cesde";
// Variable de tipo int
int edad = 20;
// Variable de tipo boolean
boolean esActivo = true;
boolean becado = false;
// Variable de tipo char
char género = 'M';
// Variable de tipo double
double promedio = 4.5;
// Variable de tipo int
int semestre = 2;
        
        // Comprobar si el estudiante está en el último semestre de su carrera y tiene estado activo
        if (semestre == 3 && esActivo==true) {
            System.out.println("El estudiante está en el último semestre de su carrera y tiene estado activo.");
        } else {
            System.out.println("El estudiante no cumple con los requisitos.");
        }
    }
} 

```
4. ## Determinar si el estudiante tiene una carrera relacionada con el desarrollo de software y un promedio superior a 4.0.

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.ejercicio12;

import java.util.Scanner;

/**
 *
 * @author USer
 */
public class Ejercicio12 {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        System.out.println("Hello World!");// Variables de tipo String
        Scanner scanner = new Scanner(System.in);
   
        System.out.print(true);
        
    // Variables de tipo String
String nombre = "Juan Pérez";
String apellido = "González";
String identificación = "1000000001";
String correo = "juan.perez@ejemplo.com";
String carrera = "Desarrollo de Software";
String universidad = "Cesde";
// Variable de tipo int
int edad = 20;
// Variable de tipo boolean
boolean esActivo = true;
boolean becado = false;
// Variable de tipo char
char género = 'M';
// Variable de tipo double
double promedio = 4.5;
// Variable de tipo int
int semestre = 2;

        
        // Comprobar si el estudiante tiene una carrera relacionada con desarrollo de software
        // y un promedio superior a 4.0
        if (carrera.equals("Desarrollo de Software") && promedio > 4.0) {
            System.out.println(" El estudiante tiene una carrera relacionada con desarrollo de software y un promedio superior a 4.0.");
        } else {
            System.out.println("El estudiante no cumple con los requisitos.");
        }
    
    }
}

```
5. ## Mostrar toda la información del estudiante si está matriculado en el Cesde.

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.ejerciciotrece;

import java.util.Scanner;

/**
 *
 * @author USer
 */
public class Ejerciciotrece {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        // Variables de tipo String
String nombre = "Juan Pérez";
String apellido = "González";
String identificación = "1000000001";
String correo = "juan.perez@ejemplo.com";
String carrera = "Desarrollo de Software";
String universidad = "Cesde";
// Variable de tipo int
int edad = 20;
// Variable de tipo boolean
boolean esActivo = true;
boolean becado = false;
// Variable de tipo char
char género = 'M';
// Variable de tipo double
double promedio = 4.5;
// Variable de tipo int
int semestre = 2;

 if (universidad.equals("Cesde")) {
            System.out.println("El estudiante estudia en el cesde");    
            System.out.println("nombre juan perez");
            System.out.println("apellido gonzales");
            System.out.println("identificacion 1000000001");
            System.out.println("correo juan.perez@ejemplo.com");
            System.out.println("carrera desarrollo de software");
            System.out.println("universidad cesde");
            
        } else {
            System.out.println("El estudiante no cumple con los requisitos.");
        }
    }
}

```
6. ## Asignar una beca del 50% si el estudiante está matriculado en el Cesde, tiene un promedio superior a 4.0 y está activo.

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.ejerciciocatorce;

import java.util.Scanner;

/**
 *
 * @author USer
 */
public class Ejerciciocatorce {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        // Variables de tipo String
String nombre = "Juan Pérez";
String apellido = "González";
String identificación = "1000000001";
String correo = "juan.perez@ejemplo.com";
String carrera = "Desarrollo de Software";
String universidad = "Cesde";
// Variable de tipo int
int edad = 20;
// Variable de tipo boolean
boolean esActivo = true;
boolean becado = false;
// Variable de tipo char
char género = 'M';
// Variable de tipo double
double promedio = 4.5;
// Variable de tipo int
int semestre = 2;

if (universidad.equals("Cesde") && promedio > 4.0 && esActivo == true) {
            System.out.println(" El estudiante tiene una beca del 50% se encuentra matriculado en el cesde y tiene un promedio superior a 4.0.");
        } else {
            System.out.println("El estudiante no cumple con los requisitos.");
        }
    }
}

```
7. ## Determinar la cantidad de beca que recibe el estudiante según su promedio:
- 0.0 - 3.4: El estudiante no recibe beca.
- 3.5 - 3.9: El estudiante recibe una beca parcial del 25%.
- 4.0 - 4.4: El estudiante recibe una beca parcial del 50%.
- 4.5 - 5.0: El estudiante recibe una beca completa.

```
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 */

package com.mycompany.ejercicioquince;

import java.util.Scanner;

/**
 *
 * @author USer
 */
public class Ejercicioquince {

    public static void main(String[] args) {
        System.out.println("Hello World!");
        
        // Variables de tipo String
String nombre = "Juan Pérez";
String apellido = "González";
String identificación = "1000000001";
String correo = "juan.perez@ejemplo.com";
String carrera = "Desarrollo de Software";
String universidad = "Cesde";
// Variable de tipo int
int edad = 20;
// Variable de tipo boolean
boolean esActivo = true;
boolean becado = false;
// Variable de tipo char
char género = 'M';
// Variable de tipo double
double promedio = 4.5;
// Variable de tipo int
int semestre = 2;

    if (promedio > 0.0 && promedio <= 3.4 ) 
    {
        System.out.println("el estudiante no recibe beca");
    } 
    else 
    {
        if (promedio >= 3.5 && promedio <= 3.9 )
            {
               System.out.println("El estudiante recibe una beca parcial del 25%.");
            }
        else 
            { 
               if (promedio >= 4.0 && promedio <= 4.4 )
               {
                    System.out.println("El estudiante recibe una beca parcial del 50%");
               }
               else 
               {
                   if ( promedio >= 4.5 && promedio <= 5.0 )
                   {
                       System.out.println("El estudiante recibe una beca completa");
                   }
                }
            }
                }
}
}

```




