# Software Requirements Specification
## For Inscripciones ITAM

#### Prepared by: 
+ Cecilia vásquez
+ Diego Villalvazo 
+ Ana Carolina Sandoval Mejía - 152808
#### DreamTeam
24 de octubre de 2019

# Tabla de contenidos
1. **Introducción**  
   1.  Propósito Convención:
   El propósito de este documento es proporcionar una descripción detallada de los requisitos para el sistema de inscripciones del ITAM. Ilustrará el propósito y la declaración completa para el
desarrollo del sistema. También explicará las limitaciones del sistema y su interfaz. 
   2.  Audiencia: 
   La audiencia para este proyecto es el personal administrativo del ITAM para que puedan dar de alta grupos nuevos, y para los alumnos para que puedan modificar su plan de estudios. 
   3.  Alcance del producto:
  El sistema de inscripciones del ITAM es un software especializado para que alumnos y staff administrativo del ITAM puedan modificar la tira de materias de los alumnos. 
Los alumnos podrán consultar las materias disponibles para su respectivo semestre, podrán seleccionar y dar de alta materias, dar de baja materias desde su tira de materias, podrán ingresar a listas de espera en caso de ser necesario. Con esta información, el alumno podrá diseñar y planificar qué materias cursar en el semestre y obtener su tira de materias.  
El personal administrativo podrá crear los grupos disponibles para el semestre y podrán revisar y administrar las listas de espera, de tal manera, resolviendo los conflictos de los alumnos.  
Sobre todo, esperamos proporcionar una experiencia de usuario cómoda e intuitiva para que los usuarios puedan administrar sus materias de manera rápida y fácil. 

   4.  Referencias:
   -  Clase de Ingeniería de Software - Ing. Paulina Bustos Arellano, 2019.
   -  Software Requirements Specification Template - Karl E. Wiegers, 2019.
2. **Drescripción**  
   1. Perspectiva del producto
   2. Funciones del producto
   3. Clases y caracteristicas
   4. Ambiente de operación
   5. Limitaciones del diseño e implementación
   6. Documentación
   7. Dependencias y supuestos
3. **Requerimientos Externos**
   1. Interfaces de Usuario
   Hay dos interfaces de usuario, una para los alumnos del ITAM y otra para los directores de carrera y jefes de departamento. La interfaz para alumnos sirve de tal manera que el alumno pueda ver inscribirse o dar de baja materias. La primera pantalla de la GUI sirve para iniciar sesión y tiene los campos de usuario y contraseña; si el alumno introduce una combinación inválica de usuario/contraseña aparece un mensaje de error en la pantalla. Después de que el alumno inicia sesión exitosamente aparece una pantalla en donde se muestra un buscador para que el alumno encuentre materias por ID y por departamento, las materias que corresponden al plan de estudios del alumnos están subrayadas y las materias que tienen lista de espera tienen el mensaje "Lista de espera" al lado de ellas. Una vez que las materias son mostradas al alumno, este puede seleccionar una o más materias y seleccionar el botón "Dar de alta" para dar de alta. Si el alumno seleccionó una materia que tiene lista de espera, le aparece un recuadro en donde pone la prioridad de la materia y la justificación para que el jefe de departamento o director de carrera lo acepte. Después de esto, el alumno es llevado a una pantalla donde se muestran sus materias registradas al momento, en forma de lista y también gráfica; sino pudo meter alguna(s) materia(s), al lado de cada materia (en la lista) aparece la razón por la cual no pudo inscribirla, también aparece un mensaje que dice "Alta de materia exitosa" al lado de cada materia que pudo registrar y un mensaje que dice "Lista de espera" para las materias en las cuales está en lista de espera y una opción para editar la prioridad y la justificación.. Desde la pantalla donde aparecen las materias registradas para el alumno hasta el momento, existe una opción de seleccionar las materias registradas y darlas de baja seleccionando el botón "Dar de baja", luego regresa a la misma pantalla en donde aparece la lista de materias con un mensaje que dice "Baja de materia" al lado de cada materia dada de baja.
   La otra interfaz es para los directores de carrera y jefes de departamento. Igual que para los alumnos, la primera pantalla de la GUI sirve para iniciar sesión y tiene los campos de usuario y contraseña; si el usuario introduce una combinación inválica de usuario/contraseña aparece un mensaje de error en la pantalla.
   2. Interfaces de Hardware
   3. Interfaces de Software
   4. Interfaces de comunicación
4. **Funcionalidad del sistema**
   1. Funcionalidad 1
   2. Funcionalidad 2
   3. Funcionalidad 3
5. **Requerimientos no funcionales**
   


