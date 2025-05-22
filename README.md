# PORTFOLIO - LISTA DE PROYECTOS:

# Proy_01 – Gráfico de ciclos (Liq_divisas_por_exp_de_oleaginosas_y_cereales)

## Introducción
El gráfico de ciclos es una herramienta elegante que me permitió explorar, al mismo tiempo, la tendencia general de una variable en el tiempo y sus ciclos estacionales. Lo usé para analizar mes a mes el comportamiento de ciertas métricas a lo largo de varios años.

Con este enfoque, busqué:

- **Detectar patrones estacionales** repetitivos (por ejemplo, en qué meses suele subir o bajar el valor).
- **Comparar cada año** frente a los anteriores, para identificar anomalías o quiebres de tendencia.
- **Hacer más intuitivo** el análisis de series temporales, ya que los gráficos de líneas convencionales enmascaran su componente cíclico.

Cada línea corresponde a un año, el eje X muestra los meses y el eje Y el valor mensual de la variable, lo que facilita visualizar si un comportamiento se repite de un año a otro.

## Datos
Fuente: datos oficiales de la Secretaría de Gobierno de Energía de Argentina  
[sspm-liquidacion-divisas-por-exportaciones-oleaginosas-cereales](https://datos.gob.ar/dataset/sspm-liquidacion-divisas-por-exportaciones-oleaginosas-cereales/archivo/sspm_349.2)

## Limpieza de datos
- Utilicé Python y pandas para ajustar el formato de fechas.
- Reemplacé puntos por comas en los decimales.
- Cambié el separador de columnas de punto y coma a coma.
- El notebook con todo el proceso está disponible en el repositorio.

## Modelo
**Modelo híbrido (semi-dimensional):** una única tabla de hechos relacionada con una tabla calendario (dimensional).

## Demo
Puedes ver el proyecto en Power BI:  
https://app.powerbi.com/view?r=eyJrIjoiOWVlNWY0NDAtNmQyZS00Y2Y2LWI5MzEtZmQzOTliYTVmNzk0IiwidCI6IjkxZjVjYjg5LTUyZmUtNDdhYi05MDVmLTRlMzU4ODZmNWE1NyIsImMiOjR9





# Proy_02 – Dashboard Análisis de maíz

## Introducción
Desarrollé este tablero con el objetivo de **controlar el flujo de entrega de materia prima**.  
La idea central fue crear una herramienta que me permita:

- Ver **cómo estoy en un período** determinado.
- **Comparar ese desempeño** con otro período anterior o posterior.

Esto facilita el seguimiento de tendencias, cuellos de botella y oportunidades de mejora en la gestión de entregas.

## Datos
Para mantener la confidencialidad se trabajó con **datos sintéticos**, y se codificaron los nombres de los proveedores.  
Aunque son datos ficticios, se generaron sobre la base de datos reales, con una variación aproximada del **±25%**.

## Limpieza de datos
El procesamiento y la transformación de los datos se realizaron completamente en **Power Query**.

## Modelo
**Modelo en estrella:** la estructura del modelo se basa en una **tabla de hechos** y varias **dimensiones** (como proveedor, producto, fechas), permitiendo una navegación eficiente y flexible en los análisis.

## Demo
Puedes ver el proyecto en Power BI:  
https://app.powerbi.com/view?r=eyJrIjoiYWRmZDFhNjQtMjIwZS00YzY2LWExZWItMjBlMGUyZTdmYWI3IiwidCI6IjkxZjVjYjg5LTUyZmUtNDdhYi05MDVmLTRlMzU4ODZmNWE1NyIsImMiOjR9

