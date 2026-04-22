# Proyecto Final: Buscaminas en MARIE.js

Este proyecto implementa una versión funcional del juego **Buscaminas** utilizando el simulador **MARIE.js** y su display gráfico de **16 × 16 celdas**.

La lógica del juego fue diseñada respetando las limitaciones de la arquitectura MARIE, por lo que la interacción con el usuario se realiza mediante entradas numéricas secuenciales a través de la instrucción `INPUT`.

## Descripción general

En cada turno, el usuario ingresa tres valores:

1. Fila
2. Columna
3. Acción

Como MARIE no cuenta con herramientas prácticas para generar aleatoriedad ni para construir tableros complejos de manera cómoda, el tablero inicial se genera externamente mediante un script en Python. Ese script produce la información necesaria para inicializar la memoria en MARIE y también permite visualizar el tablero completo para verificar el comportamiento del juego.

## Objetivo

El objetivo principal del proyecto es desarrollar la lógica de Buscaminas en lenguaje ensamblador de MARIE, usando el display 16 × 16 como interfaz gráfica y adaptando la experiencia del juego a las capacidades reales del simulador.

## Flujo de interacción

- El tablero se prepara fuera de MARIE con un script en Python.
- MARIE carga el contenido inicial en memoria.
- En cada jugada, el usuario ingresa fila, columna y acción.
- El programa procesa la jugada y actualiza el estado del tablero.

## Cuaderno de Colab

El cuaderno de Colab del proyecto está disponible aquí:

[Abrir cuaderno de Colab](https://drive.google.com/file/d/1hsW-7F1Q17yOyQrvXEAbdosAzxwlS1hE/view?usp=sharing)

## Documentación complementaria

Para entender con más detalle la estructura del algoritmo y la presentación del proyecto, se incluyen los siguientes documentos:

- [Reporte del proyecto](reporte-org-comp.pdf)
- [Póster del proyecto](poster-org-compus.pdf)