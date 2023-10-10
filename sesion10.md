<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 10 


## Actividad: Prueba, ejecución y explicación de ejercicios de lógica de programación.

#### Selecciona dos ejercicios de la sesión 10, impleméntalos, ejecútalos y proporciona una explicación detallada de cada uno


### SOLUCIÓN

3. ## Cálculo del índice de masa corporal (IMC)

```
import java.util.Scanner;

public class IMC {
   public static void main(String[] args) {
      Scanner input = new Scanner(System.in);
      double weight, height, imc;
      
      // Solicita el peso y la altura
      System.out.print("Ingrese su peso en kilogramos: ");
      weight = input.nextDouble();
      System.out.print("Ingrese su altura en metros: ");
      height = input.nextDouble();

      // Calcula el IMC
      imc = weight / (height * height);

      // Muestra el resultado en la consola
      System.out.printf("Su IMC es %.2f", imc);
   }
}

```
6. ## Calcular el movimiento parabólico de un proyectil

```
import java.util.Scanner;

public class MovimientoParabolico {
   public static void main(String[] args) {
      Scanner input = new Scanner(System.in);
      double velocidadInicial, angulo, alturaInicial, tiempo;
      final double gravedad = 9.81;
      
      // Solicita la velocidad inicial, el ángulo y la altura inicial
      System.out.print("Ingrese la velocidad inicial en metros por segundo: ");
      velocidadInicial = input.nextDouble();
      System.out.print("Ingrese el ángulo de lanzamiento en grados: ");
      angulo = input.nextDouble();
      System.out.print("Ingrese la altura inicial en metros: ");
      alturaInicial = input.nextDouble();

      // Calcula la velocidad en los ejes x e y
      double velocidadX = velocidadInicial * Math.cos(Math.toRadians(angulo));
      double velocidadY = velocidadInicial * Math.sin(Math.toRadians(angulo));

      // Calcula el tiempo de vuelo
      tiempo = (2 * velocidadY) / gravedad;

      // Calcula la distancia recorrida
      double distancia = velocidadX * tiempo;

      // Calcula la altura máxima alcanzada
      double alturaMaxima = alturaInicial + (velocidadY * velocidadY) / (2 * gravedad);

      // Muestra los resultados en la consola
      System.out.printf("La distancia recorrida es de %.2f metros.", distancia);
      System.out.printf("La altura máxima alcanzada es de %.2f metros.", alturaMaxima);
      System.out.printf("El tiempo de vuelo es de %.2f segundos.", tiempo);
   }
}

```