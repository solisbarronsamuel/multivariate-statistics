# Bitácora de Cómputo — Estadística Multivariada

Este repositorio contiene la bitácora de cómputo desarrollada a lo largo del semestre para el curso de Estadística Multivariada. La bitácora está construida como un libro Quarto y documenta, por tema, el objetivo del análisis, los datos utilizados, el procedimiento comentado, los resultados obtenidos, los problemas encontrados y los aprendizajes derivados.

La versión publicada del libro se encuentra disponible a través de GitHub Pages en la rama `gh-pages`.

---

## Estructura del repositorio

Cada carpeta corresponde a un tema de la bitácora y contiene el archivo `.qmd` con el script comentado y los resultados del análisis correspondiente.

| Carpeta | Contenido |
|---|---|
| `data-frame` | Scripts sobre manejo y manipulación de data frames en R |
| `data-visualization` | Scripts de visualización de datos |
| `manova` | Análisis Multivariado de Varianza (MANOVA) |
| `matrix-algebra` | Operaciones de álgebra matricial aplicadas a estadística multivariada |
| `multivariate-hypotheses` | Pruebas de hipótesis multivariadas |
| `pca` | Análisis de Componentes Principales (PCA) |
| `pcoa` | Análisis de Coordenadas Principales (PCoA) |
| `data` | Archivo CSV con los datos de medidas corporales recolectados al inicio del semestre |
| `_book` | Archivos generados por Quarto al compilar el libro (no editar manualmente) |
| `renv` | Entorno de reproducibilidad de paquetes de R gestionado con `renv` |

---

## Datos

La carpeta `data/` contiene el archivo CSV con las **medidas antropométricas** recolectadas por el grupo al inicio del semestre. Estos datos son la fuente principal utilizada en la mayoría de los análisis de la bitácora. Para los temas en los que los datos propios no resultan adecuados, se utilizaron los conjuntos de datos integrados en R `iris` o `mtcars`, según se especifica en cada capítulo.

---

## Uso de inteligencia artificial

A lo largo del desarrollo de esta bitácora se utilizó **Claude (Anthropic)** como herramienta de apoyo para la corrección de errores en los scripts, la revisión del significado de funciones y argumentos, sugerencias de mejora en el código, y la resolución de problemas relacionados con GitHub. El contenido analítico y los scripts provienen principalmente del material visto en clase, complementado con las siguientes referencias bibliográficas:

- Denis, D. J. (2021). *Univariate, Bivariate, and Multivariate Statistics Using R: Quantitative Tools for Data Analysis and Data Science*. Wiley. — Referencia principal para los temas de MANOVA.
- Field, A. (2012). *Discovering Statistics Using R*. SAGE Publications. — Referencia para los conceptos de varianza, covarianza y PCA.

---

## Requisitos

Para compilar el libro localmente se requiere tener instalados [R](https://cran.r-project.org/), [RStudio](https://posit.co/download/rstudio-desktop/) y [Quarto](https://quarto.org/docs/get-started/). Los paquetes de R necesarios están registrados en el entorno `renv`; para restaurarlos ejecutar `renv::restore()` en la consola de R antes de compilar.
