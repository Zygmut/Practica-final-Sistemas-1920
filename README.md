# Practica-final-Sistemas-1920

### Fecha máxima de entrega obligatoria: 7/01/2020 a las 8:00

## Practica de sistemas combinacionales

Esta práctica consiste en la creación de una ALU para números de 4 bits codificados en Complemento a 2. Esto significa que el circuito tendrá 4 entradas de datos (A3 A2 A1 A0 ) que corresponden al primer operador en complemento a 2 y otros 4 bits de entrada que corresponden al segundo operador en complemento a 2 (B3 B2 B1 B0 ). Las salidas del circuito serán 4 bits para el resultado (R3 R2 R1 R0 ) y un bit adicional de información extra (EX). Las operaciones que realiza la ALU són configurables, y tiene cuatro posibles modos de funcionamiento, tal como está especificado en la Tabla 1:

| C1 C0  |   Operacion    | Detalles de la implementeación|
|:--------:|:----------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|00|A + B|NO se pueden utilizar componentes de las librerías y se han de implementar SÓLO puertas lógicas y módulos de usuario. La salida R3..0 mostrará el resultado de la suma, y la salida EX valdrá 0 si no hay overflow y 1 si hay.|
|01| abs(A) | Se debe implementar con módulos y circuitos disponibles en las librerías de Proteus y módulos de usuario. La salida R3..0 mostrará en BNSS el valor absoluto de A. La salida EX es indiferente para este caso.|
|10| abs(A) > abs(B)| Se debe implementar con módulos y circuitos disponibles en las librerías de Proteus y módulos de usuario. La salida EX valdrá 1 si el valor absoluto de A (| A |) es mayor que el valor absoluto de B (| B |), y 0 en caso contrario. La salida R3..0 es indiferente para este caso.|
|11 |     A == B     | Se debe implementar sólo con puertas lógicas. La salida EX valdrá 1 si los dos números son iguales, y 0 en caso contrario. La salida R3..0 es indiferente para este caso.|

Esto significa que el circuito tendrá dos entradas de operación ( C1 C0 ), adicionales a las 8 entradas de los operandos, para indicar qué operación se quiere hacer. Los componentes LOGIC PRUEBAS y LOGIC STATES que representan las salidas y entradas del circuito deben estar claramente identificados con los mismos nombres que se indican en este enunciado. Además, es obligatorio incluir dos displays de 7-segmentos para cada valor (o sea, para cada valor un display que muestra el signo y otro que muestra el valor, por lo tanto un total de 6 displays). Puede ver un ejemplo en la Figura 1. Esto supone que también deberá implementar un decodificador C2 - 7segments.

### Pasos para la resolución

- Diseño de cada una de las operaciones individuales.
- Implementación de cada una de las operaciones individuales.
- Juego de pruebas de las diferentes partes.
- Diseño global del conversor.
- Implementación del conversor.
- Juego de pruebas del circuito completo.
