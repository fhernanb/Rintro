---
title       : Creación de vectores
description : En esta sección se aprenderá a construir vectores en R.

--- type:NormalExercise lang:r xp:100 skills:1 key:d9f8a52d8c
## Vector numérico o cuantitativo

Para crear un vector numérico se usa la función `c()` y dentro se colocan los valores a almacenar y separados por comas.

__Ejemplo:__ A dos personas se les pregunta sus edades, la primera responde que tiene 18 años y la segunda 25 años. Para construir el vector `edad` con la información recolectada se usa el siguiente código `edad <- c(18, 25)`.

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
# Substituya las líneas bajas ___ con el código correcto para completar el ejercicio
nher <- c(___, ___, ___)
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
## Vector con caracteres o cualitativo

Para crear un vector con caracteres se usa la función `c()` y dentro se colocan los valores a almacenar separados por comas, cada elemento del vector debe estar dentro de comillas sencillas `' '` o dobles `" "`.

__Ejemplo:__ A dos personas se les pregunta sus nombres, la primera responde David y la segunda John. Para construir el vector `nombres` con la información recolectada se usa el siguiente código `nombres <- c('David', 'John')`.

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
# Substituya las líneas bajas ___ con el código correcto para completar el ejercicio
pasatiempo <- c(___, ___, ___)
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

__Ejemplo:__ A dos personas se les pregunta si fuman, la primera responde que no y la segunda que si. Para construir el vector `fuma` con la información recolectada se usa el siguiente código `fuma <- c(FALSE, TRUE)`.

__Nota__: cuando el vector es lógico __NO__ se colocan dentro de comillas los valores `TRUE` y `FALSE`.

*** =instructions
Resuelva el siguiente problema:

- A tres personas se les preguntó si gustaban del fútbol, la primera y tercera respondieron que __si__ mientras que la segunda dijo que __no__.
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
# Substituya las líneas bajas ___ con el código correcto para completar el ejercicio
__ <- c(__, __, __)
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

--- type:MultipleChoiceExercise lang:r xp:100 skills:1 key:31831a54be
## Clases de vectores

Elija la respuesta correcta a la siguiente pregunta.

__Pregunta__:
¿Cuáles son los tres tipos de vectores que hemos estudiado aquí?

*** =instructions
- Numéricos, positivos, de nombres.
- Lógicos, de caracteres y numéricos.
- Lógicos, letras y enteros.
- De caracteres, logicos y figuras.

*** =sct
```{r}
msg_bad <- "Incorrecto, revise bien."
msg_success <- "Excelente, muy bien."
test_mc(correct = 2, feedback_msgs = c(msg_bad, msg_success, msg_bad, msg_bad))
```

--- type:MultipleChoiceExercise lang:r xp:10 skills:1 key:4c97d81235
## Para extraer elementos de un vector

Para extraer elementos de un vector se usan corchetes `[]` luego del nombre del vector y dentro de ellos se coloca un vector con las posiciones de interés.

__Ejemplo:__ Supongamos que se tiene construído el vector `personaje` de la siguiente forma.

```{r}
personaje <- c('Marge', 'Homer', 'Lisa', 'Apu', 'Bart')
```
Si queremos extraer los personajes que están en las posiciones 1, 4 y 5 se escribe el siguiente código:

```{r}
personaje[c(1, 4, 5)]
```
__Pregunta__:
¿Cuál de las siguientes instrucciones permite elegir los elementos 2, 3 y 5 del vector `personaje`?

*** =instructions
- `personaje(c(2, 3, 5))`.
- `personaje[c('dos', 'tres', 'cinco')]`.
- `personaje[2, 3, 5]`.
- `personaje[c(2, 3, 5)]`.

*** =hint

*** =pre_exercise_code
```{r}

```

*** =sct
```{r}
msg_bad <- "Incorrecto, revise bien."
msg_success <- "Excelente, muy bien."
test_mc(correct = 4, feedback_msgs = c(msg_bad, msg_bad, msg_bad, msg_success))
```
--- type:MultipleChoiceExercise lang:r xp:10 skills:1 key:7c404128ce
## Para eliminar elementos de un vector

Para eliminar elementos de un vector se debe colocar un signo menos al vector de posiciones.

__Ejemplo:__ Supongamos que se tiene construído el vector `personaje` de la siguiente forma.

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
test_mc(correct = 3, feedback_msgs = c(msg_bad, msg_bad, msg_success, msg_bad))
```
