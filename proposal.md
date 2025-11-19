<img width="534" height="437" alt="image" src="https://github.com/user-attachments/assets/fdea1ac4-4a48-41cd-a174-602368122a07" /><img width="534" height="437" alt="image" src="https://github.com/user-attachments/assets/a7543a08-c29c-473a-a5e1-62d923613da9" /># Propuesta TP DSW

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
|CRUD simple|1. CRUD Paciente<br>2. CRUD Profesional<br>3. CRUD Administrador<br>4.CRUD Consultorio<br>5. CRUD Localidad<br>5. CRUD Provincia|
|CRUD dependiente|1. CRUD Sala {depende de} CRUD Consultorio.<br>2.CRUD Horario {depende de} CRUD Profesional y CRUD Sala<br>2. CRUD Turno {depende de} CRUD Horario<br>2. CRUD Diagnóstico {depende de} CRUD Turno|
|Listado<br>+<br>detalle| 1. Listado de profesionales para reservar un turno => detalle CRUD profesionales<br> 2. Listado de turnos disponibles del profesional para reservar turnos => detalle CRUD turnos mostrando tipo de turno, día y horario<br> 3. Listado de turnos para informar al profesional => detalle CRUD turnos mostrando tipo de turno, día, hora y consultorio.<br> 4.Listado de provincias existentes => detalle CRUD provincia mostrando Nombre e ID de provincia. <br> 5. Listado de Localidades existentes => Detalle CRUD Localidades con su nombre, ID y provincia <br> 6. Listado de Consultorios existentes => detalle CRUD consultorios con nombre, localidad, provincia, ID, hora de apertura y hora de cierre del consultorio <br> 7.Listado de salas =>  detalle CRUD salas con nombre e ID de sala, consultorio y localidad a la que pertenece<br> 8. Listado de usuarios => detalle CRUD persona con email, nombre, apellido tipo y nro doc, telefono, tipo de usuario y especialidad si es profesional.|
|CUU/Epic|1. Agendar turnos<br>2. Aceptar turnos<br>3. Cargar horario de profesional<br>4. Crear/modificar/deshabilitar provincia <br> 5. Crear/modificar/deshabilitar Localidad <br>6. Crear/modificar/deshabilitar consultorio <br> 7. Crear/modificar/deshabilitar Sala <br>8. Registrar usuario normal <br>9. Registrar profesional <br> 10. Modificar usuario <br> 11. Cancelar turnos|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Paciente<br>2. CRUD Profesional<br>3. CRUD Administrador<br>4. CRUD Consultorio<br>5. CRUD Horario<br>6. CRUD Turno simple<br>7. CRUD Talleres<br>|
|Listado<br>+<br>detalle| 1. Historia clínica de paciente => detalle CRUD diagnóstico, mostrando todas las observaciones registradas en turnos asistidos por paciente, indicando fecha y hora del turno.<br>2. Listado de consultorios => detalle CRUD Consultorios|
|CUU/Epic|1. Modificar turnos <br> 2. Eliminar un unico paciente de un taller <br> 3. Crear turnos como profesional <br> 4. Añadir paciente a un turno como profesional <br> 5. Cargar/modificar/eliminar diagnóstico de un paciente|


### Alcance Adicional Voluntario

|Req|Detalle|
|:-|:-|
|Otros|* Recordatorio de turnos vía mail<br>* Validación de cuenta vía mail<br>* Notificación de cancelación de turno vía mail<br>* ChatBot con Inteligencia Artificial para agendar turnos|
