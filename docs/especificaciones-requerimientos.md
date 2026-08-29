    # Especificación de Requerimientos

## 1. Descripción del sistema

## 2. Integrantes

- Nombre:
- Nombre:
- Nombre:
- Nombre:
- Nombre:

## 3. Requerimientos Funcionales

### RF-01 - [Nombre del requerimiento]

#### Resumen

#### Entradas

| Entrada | Tipo de dato | Descripción |
|---|---|---|

#### Reglas o condiciones

#### Salidas

| Salida | Tipo de dato | Descripción |
|---|---|---|

#### Resultado esperado


### RF-02 - [Nombre del requerimiento]

#### Resumen

#### Entradas

| Entrada | Tipo de dato | Descripción |
|---|---|---|

#### Reglas o condiciones

#### Salidas

| Salida | Tipo de dato | Descripción |
|---|---|---|

#### Resultado esperado



        ### RF-03 - Inscripción a tutorías

#### Resumen
Permitir que un estudiante se inscriba a una tutoría disponible utilizando su código estudiantil y el identificador de la tutoría.

#### Entradas

| Entrada | Tipo de dato | Descripción |
|---|---|---|
| codigoEstudiante | String | Código único del estudiante |
| idTutoria | Integer | Identificador de la tutoría |

#### Reglas o condiciones

- El estudiante debe estar activo en la Universidad.
- La tutoría debe existir en el sistema.
- La tutoría debe tener al menos un cupo disponible.
- El estudiante no puede estar previamente inscrito en la tutoría.
#### Salidas

| Salida | Tipo de dato | Descripción |
|---|---|---|
| mensaje | String | Confirmación o error de la inscripción |
| cuposActualizados | Integer | Cantidad de cupos restantes después de la inscripción |

#### Resultado esperado

Si todas las condiciones se cumplen, el estudiante queda inscrito en la tutoría, se actualiza la cantidad de cupos disponibles y se muestra un mensaje de confirmación. Si alguna condición no se cumple, la inscripción no se realiza y se muestra un mensaje indicando el problema.               
### RF-04 - [Nombre del requerimiento]

#### Resumen

#### Entradas

| Entrada | Tipo de dato | Descripción |
|---|---|---|

#### Reglas o condiciones

#### Salidas

| Salida | Tipo de dato | Descripción |
|---|---|---|

#### Resultado esperado


## 4. Gestión de Versiones

### Ramas utilizadas

### Proceso de integración

### Conflictos encontrados