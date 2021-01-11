# Quiniela
Modelo para predecir el resultado de un partido de fútbol desde el punto de vista del equipo local (Ganar, Empatar, Perder)
El repositorio se divide en tres partes:
## 1. Extracción de datos
Extrae los datos desde la página https://resultados-futbol.com, la cual contiene datos de posiciones a lo largo de las jornadas así como los datos de los partidos jugados en dichas jornadas.
Una vez terminado el webscraping, los datos son almacenados en dos hojas de cálculo, una con las posiciones de cada equipo en cada jornada, y otra con los resultados de los partidos. 
Los nombres de estas hojas de cálculo siguen el siguiente patrón: 
* Tabla Posiciones: 
DDBB_Tabla\_{Primer Año}\_{Segundo Año}\_{Liga}.xlsx
* Tabla Partidos: 
DDBB_Resultados\_{Primer Año}\_{Segundo Año}\_{Liga}.xlsx
## 2. Transformación y limpieza de datos
Los datos extraídos en la parte anterior son tratados para eliminar valores nulos, normalizarlos, y crear keys que servirán de unión entre las dos tablas creadas.
Finalmente se eligen las columnas que pasarán a ser features del modelo predictivo.
## 3. Modelo predictivo
Los datos son introducidos a un modelo de clasificación, que predecirá si un partido es Ganado, Empatado, o Perdido por el equipo local.

TODO: Rellenar Sección 2. y 3. con más información a medida que vayan saliendo los resultados
