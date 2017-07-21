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
## Símbolos de asignación

Para asignar el valor a una variable se usa el símbolo `<-`.

Ejemplo: para almacenar el valor 2300 en la variable `preciodolar` se usa el siguiente código `preciodolar <- 2300`.

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
# Substituya los _____ con el valor a almacenar en precioeuro
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

