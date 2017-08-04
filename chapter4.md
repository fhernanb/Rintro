---
title       : Creación de matrices
description : En esta sección se aprenderá a construir matrices de datos en R.

--- type:NormalExercise lang:r xp:100 skills:1 key:d9f8a52d8c
## Matriz cuantitativa

Para crear una matriz se usa la función `matrix(data, nrow, ncol, byrow=FALSE)`. En el parámetro `data` se coloca el vector con los datos, en los parámetros `nrow` y `ncol` se indica el número de filas y columnas de la matriz requerida, en `byrow` se indica si el vector de datos ingresa llenando la matriz por filas o columnas, por defecto el parámetro es `byrow=FALSE`.

__Ejemplo:__ Para construir una matriz llamada `mat1` de 2 filas y 2 columnas y que contenga los números 4, 3, -5, 6 e ingresando la información por filas se usa el siguiente código.

```{r}
mat1 <- matrix(data=c(4, 3, -5, 6), ncol=2, byrow=TRUE)
mat1
##      [,1] [,2]
## [1,]    4    3
## [2,]   -5    6
```

*** =instructions
Resuelva el siguiente problema:

- Construya una matriz llamada `mat2` de 3 filas y 2 columnas con los números 4, 3, 6, 0, 8, 9 e ingresando la información por columnas.

*** =hint
- Coloque los valores 4, 3, 6, 0, 8, 9 dentro de `c()` para crear la matriz.
- Asegúrese de que la matriz se llama `mat2`.
- Verifique que usó el valor correcto para el parámetro `byrow`.


*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Escriba a continuacion la matriz mat2 con los valores 4, 3, 6, 0, 8, 9
mat2 <- matrix(___)
```

*** =solution
```{r}
mat2 <- matrix(data=c(4, 3, 6, 0, 8, 9), ncol=2, byrow=FALSE)
```

*** =sct
```{r}
msg_undefined = "Revise si usó el nombre `mat1` para la matriz."
msg_incorrect = "Revise si colocó `FALSE` en el parámetro `byrow`."
test_object("mat2",
            undefined_msg = msg_undefined,
            incorrect_msg = msg_incorrect) 

success_msg("Excelenteee!")
```

--- type:NormalExercise lang:r xp:100 skills:1 key:6d7577ce64
## Matriz con valores lógicos

Para crear una matriz con valores lógicos se usa la misma función `matrix` explicada anteriormente pero ingresando en el parámetro `data` un vector lógico.

__Ejemplo:__ Para construir una matriz llamada `mat3` de 2 filas y 2 columnas tal que los elementos de la primera columna sean `FALSE` y los restantes sean `TRUE` se utiliza el siguiente código.

```{r}
mat3 <- matrix(data=c(FALSE, FALSE, TRUE, TRUE), ncol=2, byrow=FALSE)
mat3
##       [,1] [,2]
## [1,] FALSE TRUE
## [2,] FALSE TRUE
```

*** =instructions
Resuelva el siguiente problema:

- Construya una matriz llamada `mat4` de 2 filas y 2 columnas de tal manera que la primera fila contenga dos valores `TRUE` y la segunda fila contenga dos valores `FALSE`.

*** =hint
- Coloque los valores 4, 3, 6, 0, 8, 9 dentro de `c()` para crear la matriz.
- Asegúrese de que la matriz se llama `mat1`.
- Verifique que usó el valor correcto para el parámetro `byrow`.


*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Escriba a continuacion la matriz mat1 con los valores 4, 3, 6, 0, 8, 9

```

*** =solution
```{r}
mat4 <- matrix(data=c(TRUE, TRUE, FALSE, FALSE), ncol=2, byrow=TRUE)
```

*** =sct
```{r}
msg_undefined = "Revise si usó el nombre `mat4` para la matriz."
msg_incorrect = "Revise si colocó `TRUE` en el parámetro `byrow`."
test_object("mat4",
            undefined_msg = msg_undefined,
            incorrect_msg = msg_incorrect) 

success_msg("Excelenteee!")
```
--- type:MultipleChoiceExercise lang:r xp:10 skills:1 key:7c404128ce
## Para extraer columnas o filas de una matriz

Para extraer ciertas filas o columnas de una matriz llamada `mat` se usa la siguiente estructura: `mat[vector_filas, vector_colum]`.

__Ejemplo:__ Supongamos que se tiene ya construída la matriz `mat` con 6 filas y 7 columnas.

- Para extraer la fila 2 de `mat` se usa: `mat[2, ]`.
- Para extraer la columna 3 de `mat` se usa: `mat[, 3]`.
- Para extraer la fila 2 de `mat` se usa: `mat[2, ]`.
- Para extraer la fila 2 de `mat` se usa: `mat[2, ]`.
- Para extraer la fila 2 de `mat` se usa: `mat[2, ]`.

```{r}
personaje <- c('Marge', 'Homer', 'Lisa', 'Apu', 'Bart')
```
Si queremos eliminar a Homer y Bart del vector entonces se escribe el siguiente código:

```{r}
personaje[-c(2, 5)]
```
__Pregunta__:
¿Cuál de las siguientes instrucciones permite eliminar los elementos 1 y 5 del vector `personaje`?

*** =instructions
- `personaje[-1, -5]`.
- `personaje[-c(1; 5)]`.
- `personaje[-c(1, 5)]`.
- `personaje[+c(1, 5)]`.

*** =hint

*** =pre_exercise_code
```{r}

```

*** =sct
```{r}
msg_bad <- "Incorrecto, revise bien."
msg_success <- "Excelente, muy bien."
test_mc(correct = 3, feedback_msgs = c(msg_bad, msg_success, msg_bad, msg_bad))
```
