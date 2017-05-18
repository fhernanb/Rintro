---
title       : Creación de listas
description : En esta sección se aprenderá a construir listas en R.

--- type:NormalExercise lang:r xp:100 skills:1 key:d9f8a52d8c
## Vector numérico

Para crear un vector numérico se usa la función `c()` y dentro se colocan los valores a almacenar.

Ejemplo: a dos personas se les pregunta sus edades, la primera responde que tiene 18 años y la segunda 25 años. Para construir el vector `edad` con la información recolectada se usa el siguiente código `edad <- c(18, 25)`.

*** =instructions
Resuelva el siguiente problema:

- A tres personas A, B y C se les preguntó por el número de hermanos que tienen y las respuestas fueron: dos, ninguno y 3 respectivamente.
- Construya un vector llamado `nherm` que contenga las tres respuestas.

*** =hint
- Use `c()` para crear el vector.
- Nombre al vector con `nherm`.
- Coloque dentro los valores.


*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Escriba a continuacion el vector nherm con las respuestas

```

*** =solution
```{r}
nherm <- c(2, 0, 3)
```

*** =sct
```{r}
msg_undefined = "Revise si usó el nombre `futbol` para el vector."
msg_incorrect = "Revise si ingresó bien los datos usando `TRUE` o `FALSE`."
test_object("nherm",
            undefined_msg = msg_undefined,
            incorrect_msg = msg_incorrect) 

success_msg("Excelenteee!")
```