---
title       : Operaciones básicas
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


