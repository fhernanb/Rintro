---
title       : Creación de vectores
description : En esta sección se aprenderá a construir vectores en R.

--- type:NormalExercise lang:r xp:100 skills:1 key:d9f8a52d8c
## Vector numérico

Para crear un vector numérico se usa la función `c()` y dentro se colocan los valores a almacenar y separados por comas.

Ejemplo: a dos personas se les pregunta sus edades, la primera responde que tiene 18 años y la segunda 25 años. Para construir el vector `edad` con la información recolectada se usa el siguiente código `edad <- c(18, 25)`.

*** =instructions
Resuelva el siguiente problema:

- A tres personas A, B y C se les preguntó por el número de hermanos que tienen y las respuestas fueron: 2, 0 y 3 respectivamente.
- Construya un vector llamado `nherm` que contenga las tres respuestas cuantitativas.

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

--- type:NormalExercise lang:r xp:100 skills:1 key:13c7057274
## Vector con caracteres

Para crear un vector con caracteres se usa la función `c()` y dentro se colocan los valores a almacenar separados por comas, cada elemento del vector debe estar dentro de comillas sencillas `' '` o dobles `" "`.

Ejemplo: a dos personas se les pregunta sus nombres, la primera responde David y la segunda John. Para construir el vector `nombres` con la información recolectada se usa el siguiente código `nombres <- c('David', 'John')`.

*** =instructions
Resuelva el siguiente problema:

- A tres personas A, B y C se les preguntó por pasatiempo preferido y las respuestas fueron Leer, Caminar y Dormir.
- Construya un vector llamado `pasatiempo` que contenga las tres respuestas tal y como están escritas.

*** =hint
- Use `c()` para crear el vector.
- Nombre al vector con `pasatiempo`.
- Coloque dentro las respuestas cada una dentro de comillas `' '`.


*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Escriba a continuacion el vector pasatiempo con las respuestas

```

*** =solution
```{r}
pasatiempo <- c('Leer', 'Caminar', 'Dormir')
```

*** =sct
```{r}
msg_undefined = "Revise si usó el nombre `pasatiempo` para el vector."
msg_incorrect = "Revise si ingresó bien los datos usando comillas `' '`."
test_object("pasatiempo",
            undefined_msg = msg_undefined,
            incorrect_msg = msg_incorrect) 

success_msg("Excelenteee!")
```

--- type:NormalExercise lang:r xp:100 skills:1 key:eea6792263
## Vector lógico

Para crear un vector lógico se usa la función `c()` y dentro se colocan las respuestras `TRUE` o `FALSE` a la pregunta que se haya realizado.

Ejemplo: a dos personas se les pregunta si fuman, la primera responde que no y la segunda que si. Para construir el vector `fuma` con la información recolectada se usa el siguiente código `fuma <- c(FALSE, TRUE)`.

__Nota__: cuando el vector es lógico __NO__ se colocan dentro de comillas los valores `TRUE` y `FALSE`.

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