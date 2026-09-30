# Bitacora de tecnicas avanzadas

Laboratorio 07: Tecnicas Avanzadas de Prompting.
Herramienta de IA usada: (Claude)

## Ejercicio 2: Zero-shot, one-shot y few-shot

| Tipo      | Aciertos (de 5) | Formato de la respuesta                                                | Todas con el mismo formato (Si/No) |
| --------- | --------------- | ---------------------------------------------------------------------- | ---------------------------------- |
| Zero-shot | 5 de 5          | Etiqueta de sentimiento por comentario (Positivo / Negativo / Neutral) | Si                                 |
| One-shot  | 5 de 5          | Todas con el mismo formato                                             | Si                                 |
| Few-shot  | 5 de 5          | Todas con el mismo formato                                             | Si                                 |

## Ejercicio 3: Chain of Thought

| Pedido      | Respuesta de la IA                  | Muestra los pasos (Si/No) | Correcta (Si/No) |
| ----------- | ----------------------------------- | ------------------------- | ---------------- |
| Directo     | 318.60                              | No                        | Si               |
| Paso a paso | El cliente paga S/ 318.60 en total. | Si                        | Si               |

## Ejercicio 4: Role prompting

| Version        | Vocabulario (sencillo/tecnico) | Usa ejemplos o codigo | A quien le sirve mas                                                                                           |
| -------------- | ------------------------------ | --------------------- | -------------------------------------------------------------------------------------------------------------- |
| A. Sin rol     | Sencillo                       | Si                    | A principiantes que están empezando a programar, sobre todo en Java                                            |
| B. Rol docente | Sencillo                       | Si                    | A personas que nunca han programado y a quienes recién empiezan con Java                                       |
| C. Rol senior  | Tecnico                        | Si                    | A quien empieza en Java y ya tiene una idea básica de programación, o a un compañero junior que quiere repasar |

## Ejercicio 5: Descomposicion

## Ejercicio 6: Prompt estructurado y autocritica

```text
<rol>Actua como analista de pruebas de software.</rol>
<contexto>Login web con correo y contrasena. La cuenta se bloquea
despues de 3 intentos fallidos.</contexto>
<tarea>Piensa paso a paso que puede fallar y escribe 6 casos de prueba.</tarea>
<formato>Tabla con las columnas: ID, escenario, datos de entrada,
resultado esperado.</formato>
Revisa tu tabla: faltan casos limite como campos vacios, correo sin @
o contrasena con espacios? Agrega los que falten e indica cuales agregaste.
```
