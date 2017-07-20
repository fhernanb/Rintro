---
title       : Operaciones básicas
description : En esta sección usted aprenderá a realizar operaciones aritméticas con R.

--- type:NormalExercise lang:r xp:100 skills:1 key:d9f8a52d8c
## Suma, resta, multiplicación y división

Para realizar las operaciones de suma, resta, multiplicación y división se usan los siguientes operadores respectivamente: `+ - * /`.

Ejemplo: para sumar los números 8 y 4 se usa el código `8 + 4` y para dividir 10 entre 2 se usa el código `10 / 2`.

*** =instructions
Resuelva el siguiente problema:

- Al número 12.56 réstele 10.
- Multiplique los números 10 y 8.5

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
12.56 - 10
10 * 8.5
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


--- type:MultipleChoiceExercise lang:r xp:100 skills:1 key:31831a54be
## Suma, resta, multiplicación y división

Para realizar las operaciones de suma, resta, multiplicación y división se usan los siguientes operadores respectivamente: `+ - * /`.

Ejemplo: para sumar los números 8 y 4 se usa el código `8 + 4` y para dividir 10 entre 2 se usa el código `10 / 2`.

El código correcto para restarle 10 al número 12.56 y para multiplicar los números 10 y 8.5 es:

*** =instructions
- Numéricos, positivos, de nombres.
- Lógicos, de caracteres y numéricos.
- `12.56 - 10` y `10 * 8.5`.
- De caracteres, logicos y figuras.

*** =sct
```{r}
# SCT written with testwhat: https://github.com/datacamp/testwhat/wiki

msg_bad <- "Incorrecto, revise bien."
msg_success <- "Excelente, muy bien."
test_mc(correct = 2, feedback_msgs = c(msg_bad, msg_success, msg_bad, msg_bad))
```


