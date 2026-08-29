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


### RF-03 - [Nombre del requerimiento]

#### Resumen

#### Entradas

| Entrada | Tipo de dato | Descripción |
|---|---|---|

#### Reglas o condiciones

#### Salidas

| Salida | Tipo de dato | Descripción |
|---|---|---|

#### Resultado esperado



### RF-04 - Cancelar participación en la tutoría

#### Resumen
El sistema debe permitir a un estudiante que esté inscrito en una tutoría cancelar su participación en ella.
#### Entradas

| Entrada | Tipo de dato | Descripción                  |
|---|---|------------------------------|
|Código estudiantil|String| Código del estudiante activo |
|Identificador único de la tutoría|String| Id de la tutoría             |

#### Reglas o condiciones
* El estudiante debe estar inscrito previamente en la tutoría.
* La tutoría no ha dado inicio.

#### Salidas

| Salida | Tipo de dato | Descripción                                             |
|---|---|---------------------------------------------------------|
|Mensaje de información de la operación|String| Mensaje informativo de la cancelación de la inscripción |
|Eliminar la inscripción|Boolean| Eliminar la inscripción del sistema                     |
|Cupo liberado|Boolean| Libera el cupo en el sistema                            |
#### Resultado esperado
Se espera que el sistema elimine la inscripción del estudiante, se libere el cupo y se envié el mensaje informativo de la operación realizada.
## 4. Gestión de Versiones

### Ramas utilizadas

### Proceso de integración

### Conflictos encontrados