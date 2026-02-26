# Movilidad urbana y productividad económica en ciudades de LATAM

#### Debemos entregar un reporte para entender cómo la movilidad urbana (niveles de congestión, tiempos de viaje, retrasos) se relaciona con la productividad económica (PIB per cápita, desempleo) en las principales ciudades latinoamericanas.

- El objetivo del banco es identificar en qué ciudades invertir en infraestructura de transporte para aumentar la productividad y el bienestar de la población.

Para ello, se usaron dos fuentes reales de datos:

- Movilidad urbana: TomTom Traffic Index (datos de tráfico en tiempo real).
- Economía urbana: OECD Cities (PIB per cápita, desempleo y población).

💡 Preguntas del negocio:

- ¿Qué ciudades de América Latina presentan alta congestión y baja productividad económica?
- ¿Cuáles muestran los mejores indicadores combinados (movilidad eficiente y economía fuerte)?
- ¿Qué variables parecen tener una relación más fuerte con el desarrollo urbano?


#### 🎯 Procesos:
- Crear un dataset único y limpio a partir de dos fuentes diferentes.
- Aplicar limpieza, estandarización y validación de tipos de datos.
- Filtrar y enfocar el análisis en ciudades latinoamericanas.
- Calcular indicadores agregados (por ciudad–año).
- Realizar análisis exploratorios y visuales.
- Documentar todos los pasos en Jupyter Notebook, exportar un dataset final y listo para análisis.

🛠️ Herramientas de la lección
- Jupyter Notebook
- Python: pandas, numpy, seaborn, matplotlib

#### Dataset del proyecto
- tomtom_traffic.csv : Datos sobre congestión vehicular y condiciones de tráfico en ciudades del mundo. Puedes descargarlo aquí.
- oecd_city_economy.csv : Indicadores económicos y ambientales por ciudad, recopilados por la OECD (Organización para la Cooperación y el Desarrollo Económico). Puedes descargarlo aquí.
#### Ambas tablas se complementan para entender cómo la eficiencia del tráfico urbano se relaciona con el desempeño económico en ciudades latinoamericanas.

## Visualización y Análisis de relaciones
<img width="575" height="424" alt="image" src="https://github.com/user-attachments/assets/ee11774a-9c99-4611-af6f-17c7c46fdea9" />

<img width="826" height="442" alt="image" src="https://github.com/user-attachments/assets/5a864fe3-056b-44ee-8fef-4a1a7d1598b6" />

<img width="576" height="514" alt="image" src="https://github.com/user-attachments/assets/fcfa1fe1-7a50-4f9b-9927-fe0352f272ba" />

## Resumen Ejecutivo
### Contexto & objetivo:
- El presente análisis evalúa la relación entre la movilidad urbana y la productividad económica en las principales ciudades de Latinoamérica durante 2024. El objetivo central fue determinar si un mayor PIB per cápita correlaciona directamente con mayores niveles de congestión (Jams Delay), permitiendo identificar cuellos de botella que afectan la competitividad regional y priorizar inversiones en infraestructura de transporte.

### Cobertura de datos:
- El estudio abarcó el año 2024, integrando datos de tráfico de TomTom y métricas económicas de la OCDE para ciudades clave en Argentina, Brasil, Colombia, México y Perú. El dataset consolidado permitió comparar métricas de tiempo perdido y riqueza en un entorno urbano estandarizado.

### Metodología:
- Se estandarizaron los nombres de columnas a formato snake_case y se transformaron variables críticas (PIB, desempleo y población) de formato texto a numérico para permitir cálculos. Los datos de tráfico se promediaron anualmente para eliminar la volatilidad diaria. Finalmente, se utilizó una unión de tipo INNER para asegurar que solo se analizaran ciudades con información completa en ambas dimensiones (movilidad y economía), validando los resultados mediante histogramas y diagramas de caja para detectar valores atípicos.

### Hallazgos iniciales:
- Ausencia de correlación lineal: Los datos demuestran que una economía fuerte no implica necesariamente colapso vial. Buenos Aires, con uno de los PIB per cápita más altos de la muestra ($18,117.00), mantiene una demora promedio por congestión de 571.09 min, nivel significativamente menor al de otras capitales.
- Liderazgo en congestión: Ciudad de México se posiciona como el outlier más crítico de la región, liderando el ranking con un jams_delay promedio de 2,833.06 min, superando incluso a potencias globales como Tokio o Nueva York en tiempo perdido.
- Eficiencia relativa: Ciudades como Brasilia muestran una gestión de movilidad superior, con apenas 101.58 min de demora, a pesar de tener un PIB per cápita competitivo de $16,251.00.

### Recomendaciones
- Basado en la disparidad entre tiempos de viaje y productividad, Bogotá se perfila como la ciudad prioritaria para inversión urgente. Con una demora por congestión de 1,141.55 min (la segunda más alta de la muestra analizada) y un PIB per cápita de $11,442.00, el costo de oportunidad del tiempo perdido es desproporcionado respecto a su generación de riqueza. Se recomienda priorizar proyectos de transporte masivo en el eje Bogotá-Ciudad de México para mitigar el freno económico que representa la movilidad ineficiente.

