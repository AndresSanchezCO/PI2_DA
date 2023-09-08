# Proyecto Individual Nº2 - Análisis de Siniestros Viales en CABA



## Descripción del Proyecto

Este proyecto tiene como objetivo realizar un análisis detallado de los siniestros viales en la Ciudad Autónoma de Buenos Aires (CABA). Se analizarán datos relacionados con homicidios en siniestros viales durante el período 2016-2021. El análisis se llevará a cabo siguiendo una metodología exhaustiva y utilizando diversas herramientas y técnicas de análisis de datos.

### Contexto y Rol

Los siniestros viales son un problema importante en CABA, con un alto número de víctimas fatales cada año. El Observatorio de Movilidad y Seguridad Vial (OMSV) de la Secretaría de Transporte del Gobierno de la Ciudad de Buenos Aires ha encomendado este proyecto para generar información que permita tomar medidas efectivas para reducir la cantidad de víctimas fatales en siniestros viales.

## Tecnologías y Herramientas Utilizadas

- Python
- Pandas
- Numpy
- Seaborn
- Matplotlib
- Pandas Profiling
- Power BI (para el dashboard)

## Metodología Aplicada

1. **Importación de Librerías**: Se importaron las librerías necesarias para el análisis de datos.

2. **Desactivación de Warnings**: Se desactivaron las advertencias (warnings) para una visualización más limpia.

3. **Importación de Datos**: Se importaron los datos relacionados con homicidios en siniestros viales en CABA.

4. **Primera Inspección de los Datos**: Se realizó una primera inspección de los datos para comprender su estructura y tamaño.

5. **Unión de los Datos**: Se unieron los datos de dos hojas de Excel (HECHOS y VICTIMAS) en un único DataFrame para facilitar el análisis.

6. **Limpieza del Nombre por Join**: Se limpió el nombre de las columnas después de la unión de datos.

7. **Eliminación de Columnas Duplicadas**: Se eliminaron las columnas duplicadas para evitar problemas en el análisis posterior.

8. **Inspección Primer EDA del Dataset**: Se realizó una inspección inicial del dataset.

9. **Tratar Valores Faltantes**: Se identificaron y trataron los valores faltantes en el dataset.

10. **Tratamiento de Outliers**: Se identificaron y trataron los outliers en las variables numéricas.

11. **Tratamiento de Tipos de Datos**: Se corrigieron los tipos de datos de las columnas.

12. **Análisis Exploratorio y Visualización de Datos**: Se realizó un análisis exploratorio y se crearon visualizaciones para comprender mejor los datos.

13. **Creación de KPIs**: Se crearon KPIs relacionados con la seguridad vial en CABA.

14. **Exportación de Datos Limpios**: Se exportaron los datos limpios a un archivo CSV.

## Dashboard

Se creó un dashboard interactivo en Power BI que permite explorar detalladamente los datos y visualizar información relevante sobre los siniestros viales en CABA.

## KPIs

Se definieron y calcularon tres KPIs relacionados con la seguridad vial en CABA:

1. **Tasa de Homicidios en Siniestros Viales**: Se calculó la tasa de homicidios en siniestros viales por cada 100,000 habitantes en CABA para diferentes años.

2. **Evolución de Accidentes Mortales de Motociclistas**: Se calculó la evolución de los accidentes mortales con víctimas en moto en CABA en comparación con el año anterior.

3. *KPI adicional*: Se propuso, calculó y graficó un tercer KPI relevante para la temática.

## Repositorio de GitHub

Se creó un repositorio en GitHub que contiene el código fuente, los datos limpios, el archivo de dashboard en Power BI y el presente archivo README.md con información detallada sobre el proyecto.

### Material de Apoyo

- [Notas para el uso del dataset de homicidios de siniestros viales de la CABA](https://cdn.buenosaires.gob.ar/seguridad-vial/Informe-introduccion-y-notas.pdf)
- [Evolución de la mortalidad en siniestros viales en CABA](https://www.buenosaires.gob.ar/seguridadvial/publicaciones/evolucion-de-la-mortalidad-en-siniestros-viales-en-la-ciudad-de-buenos-aires)

## Autor

- [Andres Sanchez](https://github.com/AndresSanchezCO)

## Agradecimientos

Queremos agradecer al Observatorio de Movilidad y Seguridad Vial (OMSV) de la Secretaría de Transporte del Gobierno de la Ciudad de Buenos Aires por proporcionar los datos necesarios para este proyecto.

---

**Nota**: Este proyecto es un trabajo en curso y se actualizará periódicamente con nuevos análisis y hallazgos.

