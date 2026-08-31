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

### RF-01 - Registrar información de tutorias

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

#### Salidas

| Salida           | Tipo de dato | Descripción |
|------------------|--------------|---|
| Mensaje de exito | String       |	Mensaje que informa sobre la creación de la tutoria de haber sido creada con exito|

#### Resultado esperado

Internamente, el sistema registrara la tutoria con los datos suministrados, transformando los que necesite (fecha y hora
de inicio a LocalDate y LocalTime respectivamente), asignara un identificador único a la tutoria e imprimira el mensaje
de exito

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

-main
-develop
-feature/rf01-registro-tutoria
-feature/rf02-consulta-tutorias
-feature/rf03-incripcion-tutoria
-feature/rf04-cancelacion-inscripcion
-revert-5-feature/rf02-consulta-tutorias


### Proceso de integración

A partir de la linea base, creamos una rama develop desde donde creamos cada rama de las features, en las cuales cada uno
detallo los requerimientos funcionales por separado para despues unirlos en develop y finalmente enviarlos a main.

main<br>
↓<br>
develop<br>
↓<br>
[feature/rf01-registro-tutoria, feature/rf02-consulta-tutorias, feature/rf03-incripcion-tutoria, 
-feature/rf04-cancelacion-inscripcion, revert-5-feature/rf02-consulta-tutorias]<br>
↓<br>
develop<br>
↓<br>
main

### Conflictos encontrados
Varios de los commits afectaban lineas más arriba o abajo de su sección, por lo que al hacer merge en develop, se 
presentaba un conflicto ya sea con titulos o algunas secciones de los requisitos. Nuestra solución fue editarlo
manualmente en las pull requests de github asegurandonos de no borrar información importante.<br>
Un problema mayor que tuvimos fue que aveces, por usar la interfaz de github, en vez de mergear las features con develop, 
lo haciamos directamente con main. Para arreglar esto, usamos el comando de revert para devolver las ramas afectadas a
los commits anteriores y, en el caso de main, al primer commit de creación del repositorio, que funcionaba como nuestra 
linea base.