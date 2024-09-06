# Buscaminas Solver con OCR y Algoritmos de Búsqueda
![Uso del programa](https://github.com/user-attachments/assets/b79fbc4b-5bff-4b91-9402-9ab4bfb0afb3)

Este proyecto implementa un **solver de Buscaminas** utilizando técnicas de **Reconocimiento Óptico de Caracteres (OCR)** y algoritmos avanzados de búsqueda para determinar el siguiente movimiento en el tablero. La interfaz interactiva fue desarrollada en un cuaderno de **Jupyter Notebook** utilizando **ipywidgets**, lo que permite al usuario generar el tablero, resolverlo, y visualizar el siguiente movimiento de forma dinámica.

## Características Principales

- **OCR con EasyOCR**: Se utiliza EasyOCR para leer los números en las casillas del tablero y detectar minas adyacentes.
- **Algoritmo de Búsqueda**: Implementación de un algoritmo que calcula las probabilidades de que cada casilla tenga una mina, basado en el número de minas adyacentes y las casillas abiertas.
- **Interfaz Interactiva**: Creada con `ipywidgets`, permite al usuario seleccionar el tamaño del tablero, capturar el estado actual y mostrar el próximo movimiento.
- **Detección Automática del Tablero**: Se captura la mitad izquierda de la pantalla y se recorta automáticamente el tablero de Buscaminas.
- **Visualización de Resultados**: Los resultados se muestran gráficamente, resaltando las casillas seguras y las casillas con minas con diferentes colores.

## Tecnologías Utilizadas

- **Python 3**
- **OpenCV**: Procesamiento de imágenes para detectar bordes y recortar el tablero.
- **EasyOCR**: Reconocimiento de caracteres en las casillas del tablero.
- **Matplotlib**: Visualización gráfica de los resultados.
- **ipywidgets**: Interactividad en el cuaderno de Jupyter.

## Estructura del Proyecto

1. **Captura del Tablero**: El tablero de Buscaminas se captura desde la pantalla y se recorta automáticamente utilizando técnicas de procesamiento de imágenes.
2. **Detección de Casillas**: Se detectan las casillas abiertas y cerradas mediante contornos y análisis de bordes.
3. **Lectura de Valores con OCR**: Se aplica OCR a cada casilla para leer los números y determinar cuántas minas están adyacentes.
4. **Cálculo del Siguiente Movimiento**: El algoritmo calcula la probabilidad de cada casilla para determinar el siguiente movimiento seguro.
5. **Visualización**: Se muestra el tablero con el siguiente movimiento resaltado y las probabilidades de las casillas.

## Ejemplo de Uso

1. Especifica el número de filas y columnas del tablero.
2. Haz clic en **"Resolver"** para capturar el tablero y calcular el siguiente movimiento.
3. El tablero actualizado se mostrará con el siguiente movimiento resaltado en rojo.

## Requisitos

- Python 3.7+
- Dependencias principales:
  - `easyocr`
  - `opencv-python`
  - `ipywidgets`
  - `matplotlib`
