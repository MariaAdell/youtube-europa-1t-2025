
# Proyecto: Dashboard y Análisis de Datos de YouTube – Europa 1T 2025

## 1. Fuente de datos utilizada

**URL**: https://www.kaggle.com/datasets/asaniczka/trending-youtube-videos-113-countries

Este dataset incluye los 50 videos más populares de YouTube en 113 países, con actualizaciones diarias. Contiene información detallada sobre visualizaciones, likes, comentarios, clasificaciones diarias, tendencias de movimiento y más.

---

## 2. Transformación y limpieza de los datos

El dataset original en formato CSV contiene más de 3 millones de registros (3.188.956), lo que excede las capacidades prácticas de Excel/Google Sheets. Por ello, el tratamiento inicial se realizó en Power BI para hacer el filtrado inicial, ya que es una herramienta mas ágil que con Excel.

### En Power BI:
- Se cargó el CSV completo.
- Se añadió una columna de "continente" cruzando los códigos de país ISO con Excel (listado_paises_con_continente.csv).
- Se filtraron los datos por continente “Europa” y por fecha de snapshot dentro del 1er trimestre de 2025.
- Se limpiaron los títulos de video eliminando emojis.
- Se añadió la columna 'DescriptionCountry' con el nombre completo del país.

### En Excel:
- Las columnas 'snapshot_date' y 'publish_date' se formatearon como fechas.
- Las columnas 'view_count' y 'like_count' se formatearon con separadores de miles.
- Se añadió la columna “Semana de publicación”, calculada desde 'publish_date'.

---

## 3. Análisis descriptivo de los datos

Se realizó un análisis exploratorio para identificar tendencias y patrones en los datos filtrados.

### Principales indicadores:
- **Visualizaciones totales**: más de 3,2 billones
- **Likes totales**: cerca de 99 mil millones
- **Videos únicos analizados**: 16.282

### Gráficos incluidos:
- Evolución de videos publicados por mes
- Top 10 videos más vistos
- Top 5 videos con más likes
- Top 5 canales con más visualizaciones
- Videos publicados por país

---

## 4. Dashboard en Excel

Se desarrolló un dashboard interactivo con los siguientes elementos:

- Segmentadores por **país** y **fecha**
- KPIs visuales
- Gráficos dinámicos que permiten analizar la distribución por país, canal y popularidad de los contenidos

---

## 5. Informe explicativo del análisis

> **Nota**: El análisis se basa en la columna 'snapshot_date', que refleja el momento en que un video estuvo en tendencia en un país durante el primer trimestre de 2025. La columna 'publish_date' puede ser anterior, por lo que se incluyen videos que fueron publicados en fechas previas, pero que siguen acumulando visualizaciones o relevancia durante este período.

### Conclusiones principales:

- **Concentración de visualizaciones en pocos canales**  
  Aunque el dataset contiene una amplia variedad de videos, un número reducido de canales concentra la mayor parte de las visualizaciones, indicando un comportamiento de consumo centralizado.

- **Diferencias entre países productores y consumidores de contenido**  
  Algunos países generan muchos videos, pero no necesariamente concentran las visualizaciones. Otros, con menor volumen de publicación, tienen una mayor audiencia. Esto puede estar influenciado por el idioma, el tamaño poblacional o las preferencias culturales.

- **Relevancia sostenida de ciertos canales**  
  Los rankings muestran que algunos canales aparecen repetidamente en las primeras posiciones de visualizaciones, lo que indica una fidelidad de audiencia o una buena optimización para los algoritmos de visibilidad de YouTube.

- **Presencia continuada de videos previamente publicados**  
  Se observa que muchos de los videos que aparecen en el ranking semanal tienen fechas de publicación anteriores al trimestre analizado. Esto indica que el contenido exitoso tiende a mantener su relevancia a lo largo del tiempo, reapareciendo durante varias semanas posteriores a su publicación inicial.

---

## 6. Autor y herramientas

- **Autor**: [Tu nombre aquí]
- **Herramientas utilizadas**:
  - Power BI (filtrado)
  - Microsoft Excel (transformación, limpieza, análisis y dashboard)

---

## 📦 Entregables del Proyecto

El proyecto incluye los siguientes archivos:

- 🗂️ archive.zip: Archivo original con el dataset descargado.
- 🗺️ listado_paises_con_continente.csv: Archivo auxiliar con la relación entre código ISO del país, nombre del país y continente.
- 📊 youtube.zip: No se puede subir el Zip con el archivo de Power BI con las transformaciones y filtrado. Si es necesario vemos otras vías para enviarlo.
- 📈 VisualizacionesYoutube_1ertrimestre2025.xlsx: Archivo Excel que incluye:
  - **Hoja Datos**: Dataset limpio y filtrado (solo países europeos, Q1 2025).
  - **Hoja Análisis**: KPIs y tablas dinámicas.
  - **Hoja Dashboard**: Dashboard interactivo con segmentadores y visualizaciones.
- 📄 README.md: Este archivo explicativo del proyecto, con metodología, análisis, herramientas utilizadas y conclusiones.
