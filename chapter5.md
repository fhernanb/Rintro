---
title       : Creación de arreglos
description : Insert the chapter description here

--- type:VideoExercise lang:r xp:50 skills:1 key:2732a01bb6
## ¿Qué es un arreglo?

*** =video_link
//player.vimeo.com/video/228519938

--- type:MultipleChoiceExercise lang:r xp:100 skills:1 key:31831a54be
## Creación de arreglos

Elija la respuesta correcta a la siguiente pregunta.

__Pregunta__:
¿Cuál es la función de R que se utiliza para crear un arreglo?

*** =instructions
- `arreglo`.
- `matrix`.
- `argl`.
- `array`.

*** =sct
```{r}
msg_bad <- "Incorrecto, revise bien."
msg_success <- "Excelente, muy bien."
test_mc(correct = 4, feedback_msgs = c(msg_bad, msg_bad, msg_bad, msg_success))
```