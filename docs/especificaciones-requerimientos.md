## RF-02: Consultar las tutorías disponibles.
    
### Resumen: 
El sistema debe permitir a los estudiantes consultar las tutorías que se encuentran disponibles.

### Entradas:

| Campo               | Tipo de dato |
|---------------------|--------------|
| Fecha de la tutoría | String    |
| Asignatura          | String       |


### Condiciones necesarias:
Deben haber tutorías registradas en el sistema.

### Salidas:

| Campo                                     | Tipo de dato |
|-------------------------------------------|--------------|
| Listado de tutorías disponibles           | String       |
| Identificador único de la tutoría (id)    | String       |
| Tema                                      | String       |
| Profesor                                  | String       |
| Fecha                                     | String       |
| Hora                                      | String       |
| Cantidad de cupos                         | Int          |
| Mensahe de error al no encontrar Tutorías | String       |

### Resultado:
Se espera que el sistema le muestre las tutorías disponibles al estudiante con su respectiva información acorde a la búsqueda previamente realizada.
