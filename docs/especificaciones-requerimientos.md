    # Especificación de Requerimientos

## 1. Descripción del sistema

El sistema organiza la iformación de las tutorías de profesores para los estudiantes de la Universidad. Permite a los 
profesores registrar tutorías (tema, fecha, hora y cupo máximo, validando fecha futura y cupo entre 1 y 10), y a los 
estudiantes buscar tutorías disponibles por fecha y tema, inscribirse validando que estén activos, que haya cupo y que 
no estén ya inscritos, y cancelar su inscripción siempre que la tutoría aún no haya iniciado. 
En cada operación el sistema valida las condiciones necesarias e informa al usuario el resultado.

## 2. Integrantes

- Juan Ángel Tobón Perdomo
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


## RF-02: Consultar las tutorías disponibles.

### Resumen:
El sistema debe permitir a los estudiantes consultar las tutorías que se encuentran disponibles.

### Entradas:

| Campo               | Tipo de dato | Descripción                                            |
|---------------------|--------------|--------------------------------------------------------|
| Fecha de la tutoría | String       | Fecha requerida para filtrar las tutorías disponibles. |
| Asignatura          | String       | Tema o asignatura opcional para filtrar la búsqueda.   |


### Condiciones necesarias:
Deben haber tutorías registradas en el sistema.

### Salidas:

| Campo                                     | Tipo de dato | Descripción                                                   |
|-------------------------------------------|--------------|---------------------------------------------------------------|
| Listado de tutorías disponibles           | String       | Lista con las tutorías encontradas según los filtros.         |
| Identificador único de la tutoría (id)    | String       | Identificador generado por el sistema para cada tutoría.      |
| Tema                                      | String       | Asignatura o tema a tratar en la tutoría.                     |
| Profesor                                  | String       | Código o nombre del docente responsable de la tutoría.        |
| Fecha                                     | String       | Fecha programada para la tutoría.                             |
| Hora                                      | String       | Hora de inicio de la tutoría.                                 |
| Cantidad de cupos                         | Int          | Número de cupos disponibles actualmente.                      |
| Mensaje de error al no encontrar Tutorías | String       | Mensaje de notificación cuando no hay tutorías disponibles.   |

### Resultado:
Se espera que el sistema le muestre las tutorías disponibles al estudiante con su respectiva información acorde a la búsqueda previamente realizada.



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