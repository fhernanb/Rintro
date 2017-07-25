---
title       : Operaciones básicas y asignación
description : En esta sección usted aprenderá a realizar operaciones aritméticas con R.

--- type:MultipleChoiceExercise lang:r xp:100 skills:1 key:31831a54be
## Suma, resta, multiplicación y división

Para realizar las operaciones de suma, resta, multiplicación y división se usan los siguientes operadores respectivamente: `+`,  `-`, `*`, y `/`.

Ejemplo: para sumar los números 8 y 4 se usa el código `8 + 4` y para dividir 10 entre 2 se usa el código `10 / 2`.


__Pregunta__: El código correcto para restarle 10 al número 12.56 y para multiplicar los números 10 y 8.5 es:

*** =instructions
- `12.56 + 10` y `10 + 8.5`.
- `12.56 * 10` y `10 - 8.5`.
- `12.56 - 10` y `10 * 8.5`.
- `12.56 / 10` y `10 / 8.5`.

*** =sct
```{r}
# SCT written with testwhat: https://github.com/datacamp/testwhat/wiki

msg_bad <- "Incorrecto, revise bien."
msg_success <- "Excelente, muy bien."
test_mc(correct = 3, feedback_msgs = c(msg_bad, msg_success, msg_bad, msg_bad))
```

--- type:NormalExercise lang:r xp:100 skills:1 key:d9f8a52d8c
## Símbolo de asignación y creación de variables

Para asignar el valor a una variable se usa el símbolo `<-`.

__Ejemplo:__ Para almacenar el valor 2300 en la variable `preciodolar` se usa el siguiente código `preciodolar <- 2300`.

*** =instructions
Resuelva el siguiente problema:

- Construya la variable `precioeuro` y asígnele el valor de 2500.

*** =hint
- Use `c()` para crear el vector.
- Nombre al vector con `nherm`.
- Coloque dentro los valores.

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Substituya las líneas bajas _____ con el valor a almacenar
precioeuro <- _____
```

*** =solution
```{r}
precioeuro <- 2500
```

*** =sct
```{r}
msg_undefined = "Revise si usó el nombre `precioeuro` para el vector."
msg_incorrect = "Revise si ingresó el número 2500."
test_object("precioeuro",
            undefined_msg = msg_undefined,
            incorrect_msg = msg_incorrect) 

success_msg("Excelenteee!")
```

--- type:NormalExercise lang:r xp:100 skills:1 key:ddd977c426
## Operaciones con variables parte 1

Para realizar las operaciones de suma, resta, multiplicación y división entre variables se usan los siguientes operadores respectivamente: `+`,  `-`, `*`, y `/`.

__Ejemplo:__ Crear la variable `pasaje` y almacenar allí el valor 2000, crear la variable `num_pasajes` y almacenar el valor de 5, después crear la variable `total` y que contenga el resultado de multiplicar `pasaje` por `num_pasajes`, por último imprimir por pantalla el resultado almacenado en `total`. El código necesario para realizar lo solicitado es:

```{r}
pasaje <- 2000
num_pasajes <- 5
total <- pasaje * num_pasajes
total
10000
```


*** =instructions
Resuelva el siguiente problema:

- Construya la variable `nhombre` con un valor de 6 y la variable `nmujer` con valor de 4. Construya la variable `nper` como la suma de `nhombre` y `nmujer`.

*** =hint
- Nombre los objetos con `nhombre`, `nmujer` y `nper`.
- Coloque dentro los valores.

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Complete el código para realizar lo solicitado
nhombre <- ____
nmujer <- ____
____ <- ____ + ____
```

*** =solution
```{r}
nhombre <- 6
nmujer <- 4
nper <- nhombre + nmujer
```

*** =sct
```{r}
msg_undefined = "Debe crear tres objetos."
msg_incorrect = "El objeto nper es la suma de los otros dos objetos."
test_object("nper",
            undefined_msg = msg_undefined,
            incorrect_msg = msg_incorrect) 

success_msg("Excelenteee!")
```

--- type:NormalExercise lang:r xp:100 skills:1 key:79fb1c8c8a
## Operaciones con variables parte 2

__Ejemplo:__ Una hamburguesa cuesta 5 dólares y un refresco cuesta 2 dólares. Construya la variable `nhamb` con el valor de 4 y la variable `nrefre` con el valor de 6, luego construya la variable `total` que contenga el costo total de las hamburguesas y refrescos. El código necesario para realizar lo solicitado es:

```{r}
nhamb <- 4
nrefre <- 6
total <- nhamb * 5 + nrefre * 2
total
32
```


*** =instructions
Resuelva el siguiente problema:

- Cada pasaje de adulto cuesta 0.5 dólares y cada pasaje de niño cuesta 0.15 dólares. Construya las variables `nadul <- 10` y `nnino <- 5`, luego construya la variable `total` de manera que corresponda al valor total de los pasajes. 

*** =hint
- Nombre los objetos con `nadul`, `nnino` y `total`.
- Coloque dentro los valores.

*** =pre_exercise_code
```{r}

```

*** =sample_code
```{r}
# Complete el código para realizar lo solicitado
nadul <- ____
nnino <- ____
tot__ <- ____ + ____
```

*** =solution
```{r}
nadul <- 10
nnino <- 5
total <- 0.5 * nadul + 0.15 * nnino
```

*** =sct
```{r}
msg_undefined = "Debe crear tres objetos."
msg_incorrect = "El objeto total es la suma de los otros dos objetos."
test_object("total",
            undefined_msg = msg_undefined,
            incorrect_msg = msg_incorrect) 

success_msg("Excelenteee!")
```
