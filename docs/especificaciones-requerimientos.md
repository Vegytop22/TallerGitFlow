# Especificación de Requerimientos

## 1. Descripción del sistema

El sistema organiza la iformación de las tutorías de profesores para los estudiantes de la Universidad. Permite a los 
profesores registrar tutorías (tema, fecha, hora y cupo máximo, validando fecha futura y cupo entre 1 y 10), y a los 
estudiantes buscar tutorías disponibles por fecha y tema, inscribirse validando que estén activos, que haya cupo y que 
no estén ya inscritos, y cancelar su inscripción siempre que la tutoría aún no haya iniciado. 
En cada operación el sistema valida las condiciones necesarias e informa al usuario el resultado.

## 2. Integrantes

- Juan Ángel Tobón Perdomo
- Mariana Fuertes Campo
- Edisson David Ramirez Guevara
- Linda Isabel Plazas Cortés

## 3. Requerimientos Funcionales

### RF-01 - [Nombre del requerimiento]

#### Resumen

El sistema debe permitir a los profesores registrar sus tutorías para que los estudiantes puedan visualizarlas
fácilmente.

#### Entradas

| Entrada              | Tipo de dato | Descripción                                                       |
|----------------------|--------------|-------------------------------------------------------------------|
| Código de profesor   | String       | Identificador unico de cada profesor                              |
| Tema de la tutoria   | String       | Tema que se tratara en la tutoria                                 |
| Fecha                | String       | Fecha en la que se dara la tutoria                                |
| Hora de inicio       | String       | Hora a la que iniciara la tutoria                                 |
| Maximo de asistencia | Int          | La cantidad maxima de estudiantes que pueden asistir a la tutoria |



#### Reglas o condiciones

La fecha de la tutoría NO puede ser anteriror a la fecha actual. La cantidad maxima de asistencia debe ser un valor entre 1 y 10.

#### Salidas

| Salida | Tipo de dato | Descripción |
|------------------|--------------|------------------------------------------------------------------------------------|
| Mensaje de exito | String       | Mensaje que informa sobre la creación de la tutoria de haber sido creada con exito |


#### Resultado esperado

Internamente, el sistema registrara la tutoria con los datos suministrados, transformando los que necesite (fecha y hora
de inicio a LocalDate y LocalTime respectivamente), asignara un identificador único a la tutoria e imprimira el mensaje
de exito

## RF-02: Consultar las tutorías disponibles.

### Resumen:

### Entradas:

| Campo               | Tipo de dato | Descripción                                            |
|---------------------|--------------|--------------------------------------------------------|

### Condiciones necesarias:

### Salidas:

| Campo                                     | Tipo de dato | Descripción                                                   |
|-------------------------------------------|--------------|---------------------------------------------------------------|

### Resultado:

### RF-03 - Inscripción a tutorías

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

#### Entradas

| Entrada | Tipo de dato | Descripción                  |
|---|---|------------------------------|

#### Reglas o condiciones

#### Salidas

| Salida | Tipo de dato | Descripción                                             |
|---|---|---------------------------------------------------------|

#### Resultado esperado

## 4. Gestión de Versiones

### Ramas utilizadas

### Proceso de integración

### Conflictos encontrados
