# Propuesta TP DSW

## Grupo
### Integrantes
* 52688 - Lurati Ignacio
* 52136 - Rodriguez Alan David
* 53404 - Pretelli Rodriguez Mateo Julian
* 53259 - Ortiz Genaro
* 53001 - Olivieri Luca

### Repositorios
* [Full-stack](http://hyperlinkToGihubOrGitlab) *A definir*

## Tema
### Descripción
*La empresa consta de profesionales de la salud. Estos organizan a mano sus pacientes, horarios y realizan las modificaciones a los mismos de manera totalmente autónoma. Se nos solicita realizar un sistema de autogestión para facilitar dicha tarea y a la vez permitir a otros pacientes conocer a sus profesionales vía web.*

### Modelo
![imagen del modelo](DER.png)

* [Draw.io](https://drive.google.com/file/d/1F_wJNXyFcS-_o9hZX_lNe_WDuKzT5CCj/view?usp=sharing)

## Alcance Funcional 

### Alcance Mínimo

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Paciente<br>2. CRUD Profesional<br>3. CRUD Administrador|
|CRUD dependiente|1. CRUD Horario {depende de} CRUD Profesional<br>2. CRUD Turno {depende de} CRUD Horario|
|Listado<br>+<br>detalle| 1. Listado de profesionales para reservar un turno => detalle CRUD profesionales<br> 2. Listado de turnos disponibles del profesional para reservar turnos => detalle CRUD turnos mostrando tipo de turno, día y horario<br> 3. Listado de turnos para informar al profesional => detalle CRUD turnos mostrando tipo de turno, día, hora y consultorio.|
|CUU/Epic|1. Agendar turnos<br>2. Aceptar turnos<br>3. Cambiar horario de profesional<br>4. Cargar horarios de profesional|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Paciente<br>2. CRUD Profesional<br>3. CRUD Administrador<br>4. CRUD Consultorio<br>5. CRUD Horario<br>6. CRUD Turno simple<br>7. CRUD Talleres<br>8. CRUD Pagos|
|Listado<br>+<br>detalle| 1. Historia clínica de paciente => detalle CRUD turno, mostrando todas las observaciones registradas en turnos asistidos por paciente, indicando fecha y hora del turno.<br>2. Listado de pagos => detalle CRUD pagos, pudiendo filtrar por paciente.<br>3. Listado de consultorios => detalle CRUD Consultorios|
|CUU/Epic|*A definir*|


### Alcance Adicional Voluntario

|Req|Detalle|
|:-|:-|
|Otros|* Recordatorio de turnos vía mail<br>* Validación de cuenta vía mail<br>* Notificación de cancelación de turno vía mail|
