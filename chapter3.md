---
title       : Creación de matrices
description : En esta sección se aprenderá a construir marcos de datos en R.

--- type:NormalExercise lang:r xp:100 skills:1 key:d9f8a52d8c
## Matriz

Para crear una matriz se usa la función `matrix(data, nrow, ncol, byrow=FALSE)`. En el lugar de `data` se coloca el vector con los datos, en `nrow` y `ncol` se indican el número de filas y columnas de la matriz, y en `byrow` se indica si el vector de datos ingresa por filas o columnas, por defecto es `byrow=FALSE`.

Ejemplo: para construir una matriz llamada `mimat` de 2 filas y 2 columnas y que contenga los números 4, 3, -5, 6 e ingresando la información por filas se usa el siguiente código.

`mimat <- matrix(data=c(4, 3, -5, 6), ncol=2, byrow=TRUE)`

*** =instructions
Resuelva el siguiente problema:

- Construya una matriz llamada `mat1` de 3 filas y 2 columnas con los números 4, 3, 6, 0, 8, 9 e ingresando la información por columnas.

*** =hint
- Coloque los valores 4, 3, 6, 0, 8, 9 dentro de `c()` para crear la matriz.
- Asegúrese de que la matriz se llama `mat1`.
- Verifique que usó el valor correcto para el parámetro `byrow`.


*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Escriba a continuacion matriz mat1 con los valores 4, 3, 6, 0, 8, 9

```

*** =solution
```{r}
mat1 <- matrix(data=c(4, 3, 6, 0, 8, 9), ncol=2, byrow=FALSE)
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