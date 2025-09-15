# Censo de meriendas

Este repositorio contiene un dashboard en Quarto que usamos como ejemplo práctico en el taller **Automatizar la publicación de reportes con Quarto y GitHub Actions**.
La idea es mostrar un flujo completo: render local, control de versiones, reproducibilidad con renv y deploy automático a GitHub Pages mediante un flujo de trabajo de GitHub de Actions.

### Requisitos

- Quarto (>= 1.5)

- R 4.5

- Git


### Cómo clonar el repo 

Elegí uno de estos métodos y asegurate de tener el repo en tu compu al momento del taller:

- Opción 1: Clonar con Git

```bash

git clone https://github.com/JFormoso/censo-meriendas
cd censo-meriendas

```

- Opción 2: Descargar ZIP (si no usás Git)

Ingresá al repositorio en https://github.com/JFormoso/censo-meriendas y en el botón verde **Code** seleccioná **Download ZIP**.
Luego, descomprimí la carpeta en tu equipo.

### Puesta en marcha local

- Opción 1: Con renv (reproducible)

Dentro del proyecto instalá el paquete **renv** y luego utilizá la función **restore** para instalar todos los paquetes utilizados en el proyecto.

```{r}

install.packages("renv")
renv::restore()      # instala paquetes desde renv.lock (si está en el repo)
```

- Opción 2 — Sin renv 

Instalá todos los paquetes que usamos para el proyecto de forma manual con **install.packages()**.

```{r}
install.packages(c("tidyverse","lubridate","janitor","gt","forcats","tidytext","wordcloud2","stopwords","scales"))

```

### Checklist para llegar listxs al taller

- Clonaste o descargaste el repo en tu compu
- Tenés Quarto, R y Git instalados
- Pudiste renderizar index.qmd localmente

### Contacto

Si tenés dudas o sugerencias, abrí un Issue en este repositorio.


