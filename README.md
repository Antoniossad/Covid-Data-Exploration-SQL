# Análisis Exploratorio de Datos de COVID-19 con SQL

Este repositorio contiene un proyecto de análisis de datos que explora un conjunto de datos global sobre la pandemia de COVID-19. El objetivo principal es limpiar, transformar y analizar los datos utilizando PostgreSQL para extraer insights significativos sobre el impacto y la progresión de la pandemia.

El proyecto está estructurado en dos scripts de SQL:
* `01_creacion_tablas.sql`: Contiene el código para la creación de las tablas `covid_deaths` y `covid_vaccinations`.
* `02_analisis_covid.sql`: Contiene todas las consultas utilizadas para el análisis exploratorio de datos.

---

## 🛠️ Herramientas y Tecnologías

* **Lenguaje:** PostgreSQL
* **Base de Datos:** PostgreSQL Server
* **Clientes SQL:** VS Code con extensión SQLTools, pgAdmin 4
* **Control de Versiones:** Git y GitHub

---

## 🎯 Habilidades Demostradas

* **Creación de Esquemas:** Diseño y creación de tablas con tipos de datos apropiados.
* **Limpieza de Datos:** Filtrado de registros nulos e irrelevantes para garantizar la integridad del análisis.
* **Funciones de Agregación:** Uso de `SUM()`, `MAX()`, `MIN()` y `AVG()` para generar estadísticas resumidas.
* **Agrupación de Datos:** Implementación de `GROUP BY` para realizar análisis a nivel de país y continente.
* **Unión de Tablas:** Uso de `JOIN` para combinar datos de las tablas de muertes y vacunaciones.
* **SQL Avanzado:**
    * **Expresiones de Tabla Comunes (CTEs):** para organizar y simplificar consultas complejas.
    * **Funciones de Ventana:** para realizar cálculos acumulativos (`SUM() OVER (PARTITION BY ...)`).
    * **Vistas (Views):** para almacenar consultas complejas y simplificar el acceso a los datos para futuras visualizaciones.

---

## 📊 Análisis Realizado

El script de análisis responde a las siguientes preguntas de negocio:

1.  **Tasa de Letalidad Diaria:** ¿Cuál fue la probabilidad de morir por COVID en un país específico a lo largo del tiempo?
2.  **Tasa de Infección Poblacional:** ¿Qué porcentaje de la población de un país se había contagiado en una fecha determinada?
3.  **Ranking de Infección:** ¿Qué países tuvieron el mayor pico de infección en relación con su población total?
4.  **Impacto Absoluto:** ¿Qué países y continentes registraron el mayor número total de muertes?
5.  **Resumen Global:** ¿Cuáles fueron las cifras totales de casos, muertes y el porcentaje de letalidad a nivel mundial durante el periodo analizado?
6.  **Progreso de la Vacunación:** ¿Cómo fue el conteo acumulado de vacunaciones día a día para cada país?
7.  **Porcentaje de Población Vacunada:** ¿Qué porcentaje de la población de cada país había recibido al menos una dosis de la vacuna a lo largo del tiempo?

---

## 📈 Fuente de Datos

Los datos utilizados en este análisis provienen del repositorio de COVID-19 de **Our World in Data**, una de las fuentes más completas y citadas durante la pandemia.

* **Enlace a la Fuente Principal:** [Our World in Data - Coronavirus (COVID-19) Deaths](https://ourworldindata.org/covid-deaths)

---

## 🚀 Cómo Replicar el Proyecto

1.  Descargar los archivos CSV actualizados desde la fuente de datos de Our World in Data.
2.  Configurar una base de datos PostgreSQL.
3.  Ejecutar el script `01_creacion_tablas.sql` para crear la estructura de las tablas.
4.  Utilizar un cliente como pgAdmin para importar los datos de los archivos CSV a las tablas correspondientes.
5.  Ejecutar las consultas del archivo `02_analisis_covid.sql` para replicar el análisis.
