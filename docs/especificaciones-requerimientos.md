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
