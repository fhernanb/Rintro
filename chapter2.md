---
title       : Creación de marco de datos
description : En esta sección se aprenderá a construir marcos de datos en R.

--- type:NormalExercise lang:r xp:100 skills:1 key:d9f8a52d8c
## Marco de datos

Para crear un marco de datos se usa la función `data.frame()` y dentro se colocan los vectores de la misma longitud con la información a almacenar.

Ejemplo: a dos personas se les pregunta sus edades y nombres, la primera responde que tiene 18 años con nombre David, y la segunda 25 años con nombre John. Para construir el marco de datos de nombre `datos` y con las variables `edad` y `nombre` se usa el siguiente código:

```{r, eval=F}
datos <- data.frame(edad=c(18, 25),
                    nombre=c('David', 'John'))
```

*** =instructions
Resuelva el siguiente problema:

- A dos personas A y B se les preguntó por el número de hermanos que tienen y si les gusta el fútbol, las respuestas fueron: 3 hermanos y FALSE para A, 1 hermano y TRUE para B.
- Construya un marco de datos llamado `misdatos` que contenga las variables `nherm` y `futbol`.

*** =hint
- Use `data.frame()` para crear el marco de datos.
- Colóquele al marco de datos el nombre `misdatos`.
- Coloque dentro los valores llamando las variables `nherm` y `futbol`.


*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Escriba a continuacion el vector nherm con las respuestas

```

*** =solution
```{r}
misdatos <- data.frame(nherm=c(3, 1),
                       futbol=c(FALSE, TRUE))
```

*** =sct
```{r}
msg_undefined = "Revise si usó el nombre `misdatos` para el marco de datos."
msg_incorrect = "Revise si ingresó bien los datos usando nombrando las variables `nherm` y `futbol`."
test_object("misdatos",
            undefined_msg = msg_undefined,
            incorrect_msg = msg_incorrect) 

success_msg("Excelenteee!")
```
