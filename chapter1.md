---
title       : Creación de vectores
description : En esta sección se aprenderá a construir objetos en R.
attachments :
  slides_link : https://s3.amazonaws.com/assets.datacamp.com/course/teach/slides_example.pdf

--- type:MultipleChoiceExercise lang:r xp:50 skills:1 key:80a4fdea25
## A really bad movie

Have a look at the plot that showed up in the viewer to the right. Which type of movie has the worst rating assigned to it?

*** =instructions
- Adventure
- Action
- Animation
- Comedy

*** =hint
Have a look at the plot. Which color does the point with the lowest rating have?

*** =pre_exercise_code
```{r}
# The pre exercise code runs code to initialize the user's workspace.
# You can use it to load packages, initialize datasets and draw a plot in the viewer

movies <- read.csv("http://s3.amazonaws.com/assets.datacamp.com/course/introduction_to_r/movies.csv")

library(ggplot2)

ggplot(movies, aes(x = runtime, y = rating, col = genre)) + geom_point()
```

*** =sct
```{r}
# SCT written with testwhat: https://github.com/datacamp/testwhat/wiki

msg_bad <- "That is not correct!"
msg_success <- "Exactly! There seems to be a very bad action movie in the dataset."
test_mc(correct = 2, feedback_msgs = c(msg_bad, msg_success, msg_bad, msg_bad))
```

--- type:NormalExercise lang:r xp:100 skills:1 key:d9f8a52d8c
## Vector lógico

Para crear un vector lógico se usa la función `c()` y dentro se colocan las respuestras `TRUE` o `FALSE` a la pregunta que se haya realizado.

Ejemplo: a dos personas se les pregunta si fuman, la primera responde que no y la segunda que si. Para construir el vector `fuma` con la información recolectada se usa el siguiente código.

```{r, eval=F}
fuma <- c(FALSE, TRUE)

```

*** =instructions
__Resuelva__
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
# Escriba a continuacion el vector futbol

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
