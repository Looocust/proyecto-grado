# proyecto-grado
Proyecto de grado
# Etapa 1 - Limpieza de Base de Datos de Noticias Financieras

Este notebook forma parte de un proyecto de análisis de series de tiempo y análisis de sentimiento para modelar el tipo de cambio EUR/USD. En esta primera etapa se realiza la limpieza y transformación de un conjunto de noticias financieras extraídas de diferentes fuentes.

## Objetivo

Realizar la limpieza preliminar de la base de datos de noticias financieras (`financial_news_sentiment.csv`) para su posterior análisis de sentimiento y modelado predictivo. Esta etapa se enfoca en:

- Cargar la base de datos original.
- Analizar su estructura y contenido.
- Eliminar columnas innecesarias.
- Corregir formatos de fecha.
- Eliminar valores nulos y duplicados.
- Guardar la base de datos limpia para siguientes etapas.

## Estructura del Notebook

1. **Importación de librerías**
   - `pandas`, `numpy`, `matplotlib`, `seaborn`, entre otras.

2. **Carga de la base de datos**
   - Archivo utilizado: `financial_news_sentiment.csv`.

3. **Análisis exploratorio inicial**
   - Vista general con `head()`, `info()`, `describe()`.
   - Conteo de valores nulos por columna.

4. **Transformaciones aplicadas**
   - Eliminación de columnas irrelevantes: `source`, `tickers`, `uuid`, `url`, etc.
   - Conversión de la columna `published_utc` al formato `datetime`.
   - Extracción de la fecha (`date`) desde el timestamp completo.
   - Eliminación de registros nulos y duplicados.
   - Reset del índice del DataFrame.

5. **Exportación del dataset limpio**
   - Se guarda como `financial_news_clean.csv`.

## Requisitos del Entorno

- Python 3.8+
- Paquetes utilizados:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - warnings

Puedes instalar los requerimientos con:

```bash
pip install pandas numpy matplotlib seaborn
