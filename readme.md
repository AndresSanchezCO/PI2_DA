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

# Resumen del Notebook de Análisis de Datos de Homicidios en CABA

## Importación de Bibliotecas

En esta sección, se importan las bibliotecas necesarias para el análisis de datos, como Pandas, Numpy, Seaborn, Matplotlib y Pandas Profiling. También se desactivan las advertencias para mantener un entorno limpio.

## Importación de Datos

Se cargan dos hojas de un archivo Excel llamado 'homicidios.xlsx', que contienen datos sobre homicidios relacionados con siniestros viales en CABA.

## Primera Inspección de los Datos

Se realiza una inspección inicial de los datos de ambas hojas. Esto incluye visualizar las primeras filas, obtener la lista de columnas y verificar la forma del DataFrame.

## Unión de los Datos

Dado que se identifica una coincidencia entre las dos hojas de datos mediante una columna llamada 'ID' y la fecha, se procede a unir los datos en un solo DataFrame para facilitar el análisis posterior.

## Limpieza del Nombre por Join

Se realiza una limpieza en los nombres de las columnas después de la unión de datos.

## Eliminación de Columnas Duplicadas

Se identifican y eliminan las columnas duplicadas en el DataFrame resultante de la unión de datos.

## Inspección Inicial del DataFrame Unificado

Se realiza una inspección inicial del DataFrame combinado para comprender mejor su estructura.

## Tratamiento de Valores Faltantes

Se identifican y tratan los valores faltantes en el DataFrame mediante el cálculo del porcentaje de valores faltantes en cada columna.

## Eliminación de Columnas con Valores Faltantes

Debido a la alta proporción de valores faltantes en las columnas 'Altura' y 'Cruce', se toma la decisión de eliminar estas columnas.

## Eliminación de Filas con Valores Faltantes

Se eliminan las filas que contienen valores faltantes en cualquier columna.

## Tratamiento de Valores 'SD'

Se identifica y analiza el porcentaje de valores 'SD' en las columnas del DataFrame. Se decide eliminar las filas que contienen 'SD' en cualquier columna.

## Tratamiento de Duplicados

Se identifican y eliminan las filas duplicadas en el DataFrame.

## Tratamiento de Tipos de Datos

Se corrigen los tipos de datos de ciertas columnas para que sean coherentes con la naturaleza de los datos.

## Análisis de Outliers

Se utilizan gráficos boxplot para identificar outliers en las variables numéricas. Luego, se eliminan los outliers utilizando el método del Rango Intercuartílico (IQR).

## Adición de la Columna de Población

Se agrega una columna que contiene la población correspondiente a cada año en CABA.

## Exportación de Datos Limpios

El DataFrame limpio se exporta a un archivo CSV llamado 'homicidios_limpio.csv'.

## Análisis Exploratorio y Visualización de Datos

Se realiza un análisis exploratorio de los datos, incluyendo estadísticas descriptivas y visualización de datos para comprender mejor la información contenida en el DataFrame.

| Archivo               | Descripción                                         |
|-----------------------|----------------------------------------------------|
| homicidios.xlsx       | Dataset inicial                                    |
| CABA1040.xls          | Origen población CABA                              |
| readme.md             | Archivo describiendo el proyecto                   |
| etl-eda.ipynb         | Archivo donde se realiza el proceso de ETL y EDA   |
| homicidios.html       | Primer reporte hecho con Pandas Profiling a la data sucia |
| homicidios3.html      | Último reporte que se le hace a la data limpia con Pandas Profiling |
| homicidios_limpio.csv | Data limpia                                         |



[Ver el archivo HTML](https://github.com/AndresSanchezCO/PI2_DA/blob/main/homicidios3.html)

Gracias al archivo HTML que se encuentra en la parte superior y donde se encuentra analizadas a detalle todas las variables pude seguir el camino para construir el dashboard y los kpis encontrando las siguientes conclusiones.

Para el KPI 1 por lo menos comparando los últimos 2 semestres de la información disponible, que para mi sería la información más relevante encontramos que si se cumple el kpi ya que la tasa se reduce en un 18%; aunque el dashboard es interactivo y se pueden mostrar semestres dinámicos.

Para el KPI 2 no se cumpliría ya que el porcentaje de variación aumenta en un 95% aproximadamente, sin embargo se puede hacer dinámico de año a año, otra vez comparando la información que para mi sería relevante.

Y para el KPI 3 donde propongo que los siniestros causados por autos se disminuyan en un 10% tampoco se cumple ya que aumenta en un 45%, que igual  forma se puede medir año a año y esto se puede relacionar a que los años coinciden con la pandemia y el reinicio económico, que tambíen está correlacionado con el KPI anterior y sería un sesgo.





## Dashboard

Se creó un dashboard interactivo en Power BI que permite explorar detalladamente los datos y visualizar información relevante sobre los siniestros viales en CABA.

## KPIs

Se definieron y calcularon tres KPIs relacionados con la seguridad vial en CABA:

1. **Tasa de Homicidios en Siniestros Viales**: Se calculó la tasa de homicidios en siniestros viales por cada 100,000 habitantes en CABA para diferentes años.

2. **Evolución de Accidentes Mortales de Motociclistas**: Se calculó la evolución de los accidentes mortales con víctimas en moto en CABA en comparación con el año anterior.

3. **Evolución de Accidentes Mortales en los cuales el acusado es un Autmóvil**: Se calculó la evolución de los accidentes mortales con acusados en Auto en CABA en comparación con el año anterior.

## Repositorio de GitHub

Se creó un repositorio en GitHub que contiene el código fuente, los datos limpios, el archivo de dashboard en Power BI y el presente archivo README.md con información detallada sobre el proyecto.

### Material de Apoyo

- [Fuente de datos adicionales](https://www.estadisticaciudad.gob.ar/eyc/?p=29329)


## Autor

- [Andres Sanchez](https://github.com/AndresSanchezCO)

## Agradecimientos

Queremos agradecer al Observatorio de Movilidad y Seguridad Vial (OMSV) de la Secretaría de Transporte del Gobierno de la Ciudad de Buenos Aires por proporcionar los datos necesarios para este proyecto.

---

**Nota**: Este proyecto es un trabajo en curso y se actualizará periódicamente con nuevos análisis y hallazgos.

