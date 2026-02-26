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
