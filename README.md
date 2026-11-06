# Simulador de display de números mayas

Página web para diseñar y probar la lógica combinacional de un display LED de **números mayas** (0–19).

**Demo:** https://alexcarvjal.github.io/mayan_displays/

## El display

- **4 puntos** (`p1`–`p4`, de izquierda a derecha): valen 1 cada uno.
- **3 barras** de 3 segmentos cada una (`s1–s3` superior, `m1–m3` media, `i1–i3` inferior): cada barra vale 5.
- **1 concha** (`c`): es un solo LED y representa el 0.

En total son **14 LEDs** controlados por **5 entradas** (`A` = 16, `B` = 8, `C` = 4, `D` = 2, `E` = 1).

## Cómo se usa

1. Escribe una expresión booleana en función de A, B, C, D y E para cada LED.
2. Mueve los interruptores o haz clic en una fila de la tabla de verdad para probar una combinación.
3. La columna **Muestra** lee el número maya que aparece en el display y se marca en rojo si no coincide con la entrada.

Incluye dos decodificadores precargados:

- **Maya (0–19):** expresiones mínimas tratando 20–31 como «no importa».
- **Estricto:** igual, pero deja el display apagado de 20 a 31.

Los dos llenan los puntos de izquierda a derecha y las barras de abajo hacia arriba.

Es un único archivo `index.html` sin dependencias (solo fuentes de Google Fonts). Basado en el diseño del [simulador de 7 segmentos](https://dquezada2108.github.io/7_segment_displays/).
