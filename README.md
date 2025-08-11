# Proyecto de Ciencia de Datos: Dinámicas Demográficas Globales

Este proyecto tiene como objetivo analizar la evolución histórica y las interrelaciones entre la tasa de fertilidad, la esperanza de vida y el crecimiento poblacional a nivel mundial, regional y nacional. Utiliza un conjunto de datos que abarca más de un siglo de información por país y continente, y se presenta mediante un informe dinámico desarrollado en R con `flexdashboard`.

## Objetivo Principal

Analizar la evolución histórica y las interrelaciones entre la tasa de fertilidad, la esperanza de vida y el crecimiento poblacional a nivel mundial, regional y nacional, con el fin de identificar patrones demográficos y tendencias que puedan informar políticas públicas y estudios socioeconómicos.

## Objetivos Específicos

1. **Estudiar la evolución de la tasa de fertilidad** en los diferentes continentes desde 1900 hasta 2024, identificando periodos de cambio significativo y posibles causas.

2. **Explorar la relación entre la esperanza de vida y la tasa de fertilidad** en distintas regiones, detectando correlaciones y posibles factores comunes entre países con alta esperanza de vida y baja fertilidad.

3. **Identificar los países con las tasas de fertilidad más altas y más bajas** en el año más reciente disponible, y analizar sus características demográficas y socioeconómicas.

4. **Evaluar el crecimiento poblacional por continente**, determinando cuáles han experimentado un crecimiento más acelerado y proyectando posibles escenarios futuros.

5. **Detectar patrones comunes entre países con alta esperanza de vida y baja fertilidad**, considerando variables como el continente, el nivel de desarrollo y el contexto histórico.

6. **Analizar los cambios más drásticos en la esperanza de vida** por país en las últimas décadas, relacionándolos con eventos históricos, avances médicos o políticas públicas.

7. **Comparar los indicadores de países específicos con los promedios regionales y globales**, para evaluar su posición relativa y evolución en el tiempo.

##  Fuentes de Datos

| Dataset | Indicador | Institución | URL |
|--------|-----------|-------------|-----|
| GM-Population - Dataset - v8.xlsx / Hoja: data-for-countries-etc-by-year | Population | Gapminder | http://gapm.io/dpop |
| GM-Population - Dataset - v8.xlsx / Hoja: data-for-regions-by-year | Population | Gapminder | http://gapm.io/dpop |
| GM-Fertility rates - Dataset - v15.xlsx / Hoja: data-for-countries-etc-by-year | Babies per woman, total fertility | Gapminder | [http://gapm.io/dtfr](http://fe Expectancy - Dataset - v14.xlsx / Hoja: data-for-countries-etc-by-year | Life expectancy, at birth | Gapminder | [http//gapm.io/dlex |

##  Tecnologías y Librerías Utilizadas

- **Visualización y dashboard**: `flexdashboard`, `shiny`, `shinyWidgets`, `plotly`, `leaflet`
- **Manipulación de datos**: `tidyverse`, `dplyr`, `readxl`, `scales`, `countrycode`
- **Mapas y geodatos**: `sf`, `rnaturalearth`, `rnaturalearthdata`, `maps`
- **Interactividad y tablas**: `DT`, `htmltools`

## Estructura del Proyecto
```
├── datos
│   ├── \textbf{GM-Fertility_rates_data-for-countries-etc-by-year.xlsx}: Dataset tasa de fertilidad por país y año.
│   ├── `GM-Population_data-for-countries-etc-by-year.xlsx`: Dataset habitantes por país y año.
│   ├── `life.expectancy.at.birth.xlsx`: Dataset tasa de vida por país y año.
│   └── `merged_df_final.xlsx`: Dataset consolidado con datos históricos por continente, país y año.
├── dashboard
│   └── `dashboard_demografico.Rmd`: Código del dashboard interactivo.
├── informes
│   ├── `informe_tecnico.Rmd`: Informe Técnico Demográfico.
│   ├── `informe_demografico.Rnw`: Código del Informe Técnico Demográfico en tinytex/LaTex.
│   └── `eda.Rmd`: Análisis de datos exploratorio (EDA).
└── `README.md`: Documento explicativo del proyecto.
```
---

