# Examen Parcial - alejandrogomez3

**Usuario GitHub:** alejandrogomez3
**Fecha:** 4 de noviembre de 2025
**Retos tenidos en cuenta:** Reto 001, Reto 002, Reto 003

---

## Instrucciones

A continuación encontrarás fragmentos de código extraídos de tus entregas. Cada fragmento contiene una o más situaciones relacionadas con los conceptos vistos en clase.

Para cada pregunta debes:
1) Identificar a qué se refiere la observación
2) Explicar si es o no un error y por qué
3) Proponer la corrección

Nota: Responde 5 de las 10 preguntas (en función a lo indicado en el examen).


---

## Pregunta 1

Archivo: `Reto003EdificioFinal.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/12c10998a8134110cc74b49576117ea2cc5846ba/entregas/masiasManuel/src/Reto003EdificioFinal.java) (Reto 003)

```java
if (d == 1) fila.append("[9]:"); // Ascensor central
```

¿Qué observas en este código?

El error observado en este fragmento de código viene dado por el uso del comentario `// Ascensor central` debido a que en numerosas ocasiones el profesor explica que en ningún momento se debe utilizar comentarios debido a que los ingenieros somos muy vagos y lo hacen lo más fácil posible, así que los comentarios son innecesarios. El `d==1` implica la columna 1 y el `fila.append("[9]:")` implica el añadir texto a la variable de fila.

---

## Pregunta 2

Archivo: `Reto003EdificioFinal.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/12c10998a8134110cc74b49576117ea2cc5846ba/entregas/masiasManuel/src/Reto003EdificioFinal.java) (Reto 003)

```java
System.out.println(" ==================================\n");
System.out.printf("Dia %d - %02d:00h Consumo hora: %d\n\n", dia + 1, hora, consumoHora);
```

¿Qué observas en este código?

En este código, el uso de \n en System.out.println(...) es innecesario, ya que println añade el salto de línea por defecto. Esto puede provocar una línea vacía adicional. Se debe eliminar para mantener la salida limpia, por lo que es un error grave de código y no mantiene esa limpieza y estructura de código pedida por el profesor
---

## Pregunta 3

Archivo: `ConversorDuracion.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/ae507fa3c77a26023f3e1c4a9f7a0aa13c563d32/entregas/ConversorDuracion.java) (Ejercicios)

```java
int dias = segundosTotales / 86400;
segundosTotales %= 86400;
int horas = segundosTotales / 3600;
segundosTotales %= 3600;
int minutos = segundosTotales / 60;
int segundos = segundosTotales % 60;
```

¿Qué observas en este código?

En este código podemos observar que la variable `segundosTotales` se modifica con la operación de `%=`lo que hace que esa variable dependa de las operaciones en cada paso y no se guarda en ningún sitio por lo que si lo necesitamos para otros calculos no disponemos de ella sino que disponemos de la ultima operación. Así como el uso de `segundosTotales`que se toman como el total de segundos, sin embargo no son los segundos originales porque se ven modificados tras las operaciones realizadas anteriormente.

---

## Pregunta 4

Archivo: `DevolverCambio.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/ae507fa3c77a26023f3e1c4a9f7a0aa13c563d32/entregas/DevolverCambio.java) (Ejercicios)

```java
if (entregado < importe) {
    System.out.println("El dinero entregado debe ser mayor que el importe a pagar.");
    return;
}
// ...
Scanner scanner = new Scanner(System.in);
// ...
```

¿Qué observas en este código?

En este código podemos observar el error de los comentarios debido a que en numerosas ocasiones el profesor explica que en ningún momento se debe utilizar comentarios debido a que los ingenieros somos muy vagos y lo hacen lo más fácil posible, así que los comentarios son innecesarios. Así como que el código intenta usar las variables `entregado` e `importe` antes de haber usado el scanner, ya que antes del scanner hay un if. 

---

## Pregunta 5

Archivo: `UnGuerrero.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/ae507fa3c77a26023f3e1c4a9f7a0aa13c563d32/entregas/UnGuerrero.java) (Ejercicios)

```java
int dañoGuerrero = 2;
// ...
int dañoVampiro = 4;
```

¿Qué observas en este código?

En este código podemos observar el error de los comentarios debido a que en numerosas ocasiones el profesor explica que en ningún momento se debe utilizar comentarios debido a que los ingenieros somos muy vagos y lo hacen lo más fácil posible, así que los comentarios son innecesarios. Además los nombres de las constantes son muy ambiguos y podrían tener otro nombre que le diera contexto a dicha constante para que el código se pudiese leer bien y estuviese limpio y preparado para utilizarle, sin necesidad de pensar en que es cada cosa.

---

## Pregunta 6

Archivo: `UnGuerrero.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/ae507fa3c77a26023f3e1c4a9f7a0aa13c563d32/entregas/UnGuerrero.java) (Reto 002, líneas 3-4)

```java
int vidaGuerrero = 20;
int dañoGuerrero = 2;
```

¿Qué observas en este código?

---

## Pregunta 7

Archivo: `UnGuerrero.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/ae507fa3c77a26023f3e1c4a9f7a0aa13c563d32/entregas/UnGuerrero.java) (Reto 002, línea 16)

```java
final double PROBABILIDAD_DE_ATAQUE = 0.5;
```

¿Qué observas en este código?

---

## Pregunta 8

Archivo: `UnGuerrero.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/ae507fa3c77a26023f3e1c4a9f7a0aa13c563d32/entregas/UnGuerrero.java) (Reto 002, línea 19)

```java
System.out.println("¡El guerrero golpea!" + dañoGuerrero + " HP");
```

¿Qué observas en este código?

---

## Pregunta 9

Archivo: `UnGuerrero2.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/ae507fa3c77a26023f3e1c4a9f7a0aa13c563d32/entregas/UnGuerrero2.java) (Reto 002, líneas 43-45)

```java
} else {
    System.out.println("Opción inválida. Pierdes el turno.");
    probabilidadHeroe = 0;
```

¿Qué observas en este código?

---

## Pregunta 10

Archivo: `UnGuerrero2.java` — [Ver archivo](https://github.com/mmasias/25-26-PRG1/blob/ae507fa3c77a26023f3e1c4a9f7a0aa13c563d32/entregas/UnGuerrero2.java) (Reto 002, línea 79)

```java
probabilidadVampiro = 0.30;
```

¿Qué observas en este código?

