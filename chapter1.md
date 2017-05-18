---
title       : Creación de vectores
description : En esta sección se aprenderá a construir vectores en R.
attachments :
  slides_link : https://s3.amazonaws.com/assets.datacamp.com/course/teach/slides_example.pdf

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

--- type:NormalExercise lang:r xp:100 skills:1 key:eea6792263
## Vector lógico

Para crear un vector lógico se usa la función `c()` y dentro se colocan las respuestras `TRUE` o `FALSE` a la pregunta que se haya realizado.

Ejemplo: a dos personas se les pregunta si fuman, la primera responde que no y la segunda que si. Para construir el vector `fuma` con la información recolectada se usa el siguiente código `fuma <- c(FALSE, TRUE)`.

*** =instructions
Resuelva el siguiente problema:

- A tres personas se les preguntó si gustaban del fútbol, la primera y tercera respondieron que si mientras que la segunda dijo que no.
- Construya un vector llamado `futbol` que contenga las tres respuestas.

*** =hint
- Use `c()` para crear el vector.
- Nombre al vector con `futbol`.
- Use `TRUE` o `FALSE`.


*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Escriba a continuacion el vector futbol con las respuestas

```

*** =solution
```{r}
futbol <- c(TRUE, FALSE, TRUE)
```

*** =sct
```{r}
msg_undefined = "Revise si usó el nombre `futbol` para el vector."
msg_incorrect = "Revise si ingresó bien los datos usando `TRUE` o `FALSE`."
test_object("futbol",
            undefined_msg = msg_undefined,
            incorrect_msg = msg_incorrect) 

success_msg("Excelenteee!")
```
