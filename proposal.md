# Propuesta TP DSW

## Grupo
### Integrantes
* 52688 - Lurati Ignacio
* 52136 - Rodriguez Alan David
* 53404 - Pretelli Rodriguez Mateo Julian
* 53259 - Ortiz Genaro
* 53001 - Olivieri Luca

### Repositorios
* [Full-stack](https://github.com/Genchu5/DSW-Autogestora-de-turnos.git) 

## Tema
### Descripción
*La empresa consta de profesionales de la salud. Estos organizan a mano sus pacientes, horarios y realizan las modificaciones a los mismos de manera totalmente autónoma. Se nos solicita realizar un sistema de autogestión para facilitar dicha tarea y a la vez permitir a otros pacientes conocer a sus profesionales vía web.*

### Modelo
![imagen del modelo](https://github.com/user-attachments/assets/ab1d5f90-5379-46fe-ba1a-3f4f918b199f)


* [Draw.io](https://app.diagrams.net/#G1vIZZ-KLhW0B18fT-SZHTOqqv-LPNIAcL#%7B%22pageId%22%3A%22eKS7SbHX9Nti7IfRPMdn%22%7D)

## Alcance Funcional 

### Alcance Mínimo

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Paciente<br>2. CRUD Profesional<br>3. CRUD Administrador<br>4.CRUD Consultorio<br>5. CRUD Localidad|
|CRUD dependiente|1. CRUD Sala {depende de} CRUD Consultorio.<br>2.CRUD Horario {depende de} CRUD Profesional y CRUD Sala<br>2. CRUD Turno {depende de} CRUD Horario|
|Listado<br>+<br>detalle| 1. Listado de profesionales para reservar un turno => detalle CRUD profesionales<br> 2. Listado de turnos disponibles del profesional para reservar turnos => detalle CRUD turnos mostrando tipo de turno, día y horario<br> 3. Listado de turnos para informar al profesional => detalle CRUD turnos mostrando tipo de turno, día, hora y consultorio.|
|CUU/Epic|1. Agendar turnos<br>2. Aceptar turnos<br>3. Cargar horario de profesional|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Paciente<br>2. CRUD Profesional<br>3. CRUD Administrador<br>4. CRUD Consultorio<br>5. CRUD Horario<br>6. CRUD Turno simple<br>7. CRUD Talleres<br>|
|Listado<br>+<br>detalle| 1. Historia clínica de paciente => detalle CRUD turno, mostrando todas las observaciones registradas en turnos asistidos por paciente, indicando fecha y hora del turno.<br><br>2. Listado de consultorios => detalle CRUD Consultorios|
|CUU/Epic|*A definir*|


### Alcance Adicional Voluntario

|Req|Detalle|
|:-|:-|
|Otros|* Recordatorio de turnos vía mail<br>* Validación de cuenta vía mail<br>* Notificación de cancelación de turno vía mail<br>* ChatBot on Inteligencia Artificial para agendar turnos|
