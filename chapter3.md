---
title       : Creación de matrices
description : En esta sección se aprenderá a construir marcos de datos en R.

--- type:NormalExercise lang:r xp:100 skills:1 key:d9f8a52d8c
## Matriz

Para crear una matriz se usa la función `matrix(data, nrow, ncol, byrow = FALSE)`. En el lugar de `data` se coloca el vector con los datos, en `nrow` y `ncol` se indican el número de filas y columnas de la matriz, y en `byrow` se indica si el vector de datos ingresa por filas o columnas, por defecto es `byrow=FALSE`.

Ejemplo: para construir una matriz llamada `mimat` de 4 filas y 3 columnas y que contenga los primeros 12 números enteros positivos se usa el siguiente código.

`mimat <- matrix(data=1:12, ncol=4, nrow=3)`.

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