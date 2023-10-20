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
      
      
      System.out.print("Ingrese su peso en kilogramos: ");
      weight = input.nextDouble();
      System.out.print("Ingrese su altura en metros: ");
      height = input.nextDouble();

      
      imc = weight / (height * height);

      
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
      
      
      System.out.print("Ingrese la velocidad inicial en metros por segundo: ");
      velocidadInicial = input.nextDouble();
      System.out.print("Ingrese el ángulo de lanzamiento en grados: ");
      angulo = input.nextDouble();
      System.out.print("Ingrese la altura inicial en metros: ");
      alturaInicial = input.nextDouble();

      
      double velocidadX = velocidadInicial * Math.cos(Math.toRadians(angulo));
      double velocidadY = velocidadInicial * Math.sin(Math.toRadians(angulo));

      
      tiempo = (2 * velocidadY) / gravedad;

      
      double distancia = velocidadX * tiempo;

      
      double alturaMaxima = alturaInicial + (velocidadY * velocidadY) / (2 * gravedad);

      
      System.out.printf("La distancia recorrida es de %.2f metros.", distancia);
      System.out.printf("La altura máxima alcanzada es de %.2f metros.", alturaMaxima);
      System.out.printf("El tiempo de vuelo es de %.2f segundos.", tiempo);
   }
}

```