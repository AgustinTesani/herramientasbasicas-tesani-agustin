# Rendimiento físico: análisis de pruebas y medidas corporales

**Autor:** Agustín Tesani
**Curso:** Curso de herramientas básicas para el análisis de datos
**Cohorte:** [185761](https://cursos.utnba.centrodeelearning.com/course/view.php?id=23711)

## Objetivo
Identificar qué pruebas físicas y medidas corporales se asocian más con un alto nivel de rendimiento (clase A) y cómo cambia esa relación según sexo y edad.

## Dataset
*Body Performance Data* (Kaggle, autor: kukuroo3): 13.393 registros y 12 columnas con edad, sexo, medidas corporales, pruebas físicas (fuerza de agarre, abdominales, salto en largo, flexibilidad) y una clasificación de rendimiento `class`, de A (mejor) a D.
Enlace: [Kaggle](https://www.kaggle.com/datasets/kukuroo3/body-performance-data)

## Pasos realizados
1. **Limpieza (pandas):** eliminé duplicados, convertí ceros imposibles y valores fuera de rango en nulos y los descarté (23 filas, 0,17 %), corregí tipos, estandaricé nombres y creé las columnas `class_num` y `age_group`. Quedaron 13.370 filas y 14 columnas.
2. **EDA (matplotlib y seaborn):** boxplots, mapa de correlaciones, correlaciones por sexo y porcentaje de clase A por grupo de edad y sexo.
3. **Dashboard (Power BI):** KPIs (total de personas, promedio de abdominales, promedio de % de grasa y % de clase A), segmentadores, gráficos y conclusiones.

## Resultados principales
- La flexibilidad y los abdominales son las pruebas que más diferencian las clases (flexibilidad ~21 cm en A vs ~8 cm en D; abdominales ~48 vs ~30).
- El porcentaje de grasa corporal sube de ~20 % (clase A) a ~27 % (clase D).
- En mujeres, el porcentaje de clase A baja con la edad (~39 % a ~20 %); en varones no hay una tendencia clara.

## Limitaciones
Asociación no implica causalidad. Se desconoce cómo se construyó la variable `class`. La muestra se concentra en 21–29 años (~43 %) y es 63 % varones.

## Archivos
- [CSV original](data/raw/bodyPerformance.csv)
- [CSV limpio](data/clean/bodyPerformance_limpio.csv)
- [Notebook de Python](notebooks/Trabajo_final_integrador_Herramientas_b%C3%A1sicas_para_el_an%C3%A1lisis_de_Datos_Tesani_Agustin.ipynb)
- [Dashboard de Power BI (.pbix)](dashboard/dashboard_rendimiento_fisico.pbix)



## Fuentes
- Dataset: [Body Performance Data, Kaggle](https://www.kaggle.com/datasets/kukuroo3/body-performance-data)
- Imagen del dashboard: No se utilizaron imágenes de terceros.
