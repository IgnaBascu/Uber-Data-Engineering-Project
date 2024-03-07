# Uber-Data-Engineering-Project
Proyecto de ingeniería de datos ETL, a partir de una muestra de datos de Uber NYC, desde el Data Modelling, procesamiento y transformación hasta la visualización de estos usando las tecnologías y servicios de Google Cloud Platform, Python y Mage Data Pipeline Tool.

> [!Note]
> Proyecto basado en el tutorial de Darshil Parmar : https://www.youtube.com/watch?v=WpQECq5Hx9g&t=155s

![NYC Taxis](https://www.nuevayork.net/f/estados-unidos/nueva-york/guia/taxi.jpg)

## Setup

La arquitectura de la solución se basa en las tecnologías de Google Cloud Platform (GCP) junto con la herramienta open-source de pipelines Mage, todo esto bajo lenguaje SQL y Python.

<p align="center">
  <img src="https://github.com/IgnaBascu/Uber-Data-Engineering-Project/blob/main/assets/DiagramaETL.png?raw=true">
</p>

## Resumen de herramientas

*  **Cloud Storage**: Almacenamiento de datos no estructurados, se ocupó para guardar el dataset a trabajar.


*  **MAGE AI**: Framework open-source ETL para construir, correr y manejar pipelines de data para su integración y transformación.

Código de transformaciones acá:

*  **Compute Engine**: Instancia de Máquina virtual donde se instaló Mage


*  **BigQuery**: Servicio de Google para análisis y almacen de datos mediante el uso de queries SQL

*  **Locker**: Servicio de Google para visualización de datos tipo dashboard interactivos.

## Dataset usado

Es una muestra de 100K datos sobre viajes en Nueva York de la "*NYC Taxi and Limousine Commission*" que muestra diversas features tales como tarifas, códigos de tarifa, métodos de pago, coordenadas de pickup y dropoff de viajes, etc.

- Dataset (Muestra): https://github.com/darshilparmar/uber-etl-pipeline-data-engineering-project/blob/main/data/uber_data.csv
- Diccionario de datos: https://www.nyc.gov/assets/tlc/downloads/pdf/data_dictionary_trip_records_yellow.pdf

## Modelado de datos

Al intentar recrear un modelo real de negocios para DataWarehouse, se realizó un modelado tipo estrella (Star Model) con una tabla de hechos (fact_table) y varias tablas de dimensiones rodeandola. Se hizo con la herramienta draw.io

 *Modelo puede mejorar, solo es con proposito de aprendizaje*
