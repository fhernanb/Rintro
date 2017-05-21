---
title       : Creación de marco de datos
description : En esta sección se aprenderá a construir marcos de datos en R.

--- type:NormalExercise lang:r xp:100 skills:1 key:d9f8a52d8c
## Marco de datos

Para crear un marco de datos se usa la función `data.frame()` y dentro se colocan los vectores de la misma longitud con la información a almacenar.

Ejemplo: a dos personas se les pregunta sus edades y nombres, la primera responde que tiene 18 años con nombre David, y la segunda 25 años con nombre John. Para construir el marco de datos de nombre `datos` se usa el siguiente código:

```{r, eval=F}
datos <- data.frame(edades=c(18, 25),
                    nombres=c('David', 'John')
```

