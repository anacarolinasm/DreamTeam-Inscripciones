# Software Requirements Specification
## For Inscripciones ITAM

#### Prepared by: 
+ Cecilia Vásquez Perez- 150482 
+ Diego Villalvazo Sulzer - 155844 
+ Ana Carolina Sandoval Mejía - 152808
+ Stephanie
#### DreamTeam
24 de octubre de 2019
# Tabla de contenidos
1. **Introducción**  
   1.  Propósito Convención.
   2.  Audiencia. 
   3.  Alcance del producto.
   4.  Referencias. 
2. **Drescripción**  
   1. Perspectiva del producto
   2. Funciones del producto
   3. Clases y caracteristicas
   4. Ambiente de operación
   5. Limitaciones del diseño e implementación
   6. Documentación
   7. Dependencias y supuestos
3. **Requerimientos Externos**
   1. Interfaces de Usuario.
   2. Interfaces de Hardware. 
   3. Interfaces de Software.
   4. Interfaces de comunicación
4. **Funcionalidad del sistema**
   1. Funcionalidad 1
   2. Funcionalidad 2
   3. Funcionalidad 3
5. **Requerimientos no funcionales**
   
   # 1. Introducción
   ## 1.1 Propósito Convención.
    El propósito de este documento es proporcionar una descripción detallada de los requisitos para el sistema de inscripciones del ITAM. 
    Ilustrará el propósito y la declaración completa para el desarrollo del sistema. También explicará las limitaciones del sistema y su interfaz.
   
      ## 1.2 Audiencia
      La audiencia para este proyecto es el personal administrativo del ITAM para que puedan dar de alta grupos nuevos y para los alumnos para que puedan modificar su plan de estudios.

      ## 1.3 Alcance del producto
      El sistema de inscripciones del ITAM es un software especializado para que alumnos y staff administrativo del ITAM puedan modificar la tira de materias de los alumnos. 
      Los alumnos podrán consultar las materias disponibles para su respectivo semestre, podrán seleccionar y dar de alta materias, dar de baja materias desde su tira de materias, podrán ingresar a listas de espera en caso de ser necesario. Con esta información, el alumno podrá diseñar y planificar qué materias cursar en el semestre y obtener su tira de materias.  
      El personal administrativo podrá crear los grupos disponibles para el semestre y podrán revisar y administrar las listas de espera, de tal manera, resolviendo los conflictos de los alumnos.  
      Sobre todo, esperamos proporcionar una experiencia de usuario cómoda e intuitiva para que los usuarios puedan administrar sus materias de manera rápida y fácil. 
   
   ## 1.4 Referencias
      -  Clase de Ingeniería de Software - Ing. Paulina Bustos Arellano, 2019.
      -  Software Requirements Specification Template - Karl E. Wiegers, 2019.

   # 2. Descripción  
   ## 2.1 Perspectiva del producto
   El producto surge como una necesidad para mejorar el sistema de inscripciones actual del ITAM, debido a su falta de actualización y su falta de una interfaz amigable con el usuario provocando que cada semestre se encuentren con problemas al momento de las inscripciones.

   Esta pensado para mejorar la experiencia de los usuarios que serán los alumnos y personal administrativo del ITAM.
   ## 2.2 Funciones del producto
   Esta mejora del producto debe de tener las siguientes caracteristicas como minimo: 
 
   - Alta de materias.
   - Baja de materias
   - Modificación de Horario.


   Para que esos requerimientos minimos funciones se debe considerar tambien lo siguiente:
      
   - Inicio de sesión
   - Recuperar contraseña
   - Listas de espera.
   - Prerrequisitos de materias.
      
   ## 2.3 Usuarios y caracteristicas
   Los usuarios principales de este producto serán los alumnos,ya que en sí el producto esta diseñado para que puedan inscribirse y modificar horarios. Estos usuarios deben de contar con su clave unica y contraseña para poder realizar estos tramites, tambien deben de tener noción de los prerrequisitos de las materias que desean ingresar.

   Otros usuarios son los administrativos. Ellos ingresarán al sistema para revisar solicitudes de casos especiales,ingresar grupos y salones, checar listas de espera, entre otros.

   ## 2.4 Ambiente de operación
   El producto debe de ser visualizado en cualquier navegador tanto de una computadora de escritorio / laptop, dispositivo móvil o tableta.
   ## 2.5 Limitaciones del diseño e implementación
   Algunas limitaciones que se encuentran para este producto son:
    - Los protocolos de seguridad que se tienen como estándar.
    - Utilizar la base de datos ya existente con los datos de los alumnos.
    - Tiempo de desarrollo del producto, ya que debe de estar listo para las proximas inscripciones.

   ## 2.6 Documentación
   Para que el usuario pueda tener una mejor experiencia al utilizar este sistema se le proporcionarán erramientas para ayudarlo en el uso de la nueva aplicación. Para esto se considero que la mejor manera de hacer es a través de un chatbot para dudas en la página y también la creación de un manual para llevarlo paso a paso sobre como realizar los procesos.

   ## 2.7 Dependencias y supuestos
   Se asume que los usuarios cuentan con una computadora en condiciones optimas con los funcionamientos básicos y acceso a internet a través de algun explorador como edge, google chrome, etc.
   
   Por parte de las personas encargadas de este proyecto se asume que se tendrá un servidor web en buenas condiciones y con el funcionamiento adecuado para que el sistema funcione, que la base de datos este actualizada y bien implementada.

   # 3. Requerimientos Externos
   ## 3.1. Interfaces de Usuario.
   Hay dos interfaces de usuario, una para los alumnos del ITAM y otra para los directores de carrera y jefes de departamento. 

   La interfaz para alumnos sirve de tal manera que el alumno pueda ver inscribirse o dar de baja materias. La primera pantalla de la GUI sirve para iniciar sesión y tiene los campos de usuario y contraseña; si el alumno introduce una combinación inválica de usuario/contraseña aparece un mensaje de error en la pantalla. Después de que el alumno inicia sesión            aparece una pantalla en donde se muestra un buscador para que el alumno encuentre materias por ID y por departamento, las materias que corresponden al plan de estudios del alumnos están subrayadas y las materias que tienen lista de espera tienen el  mensaje "Lista de espera" al lado de ellas. 
   Una vez que las materias son mostradas al alumno, este puede seleccionar una o más materias y seleccionar el botón "Dar de alta" para dar de alta. 
   Si el alumno seleccionó una materia que tiene lista de espera, le aparece un recuadro en donde pone la prioridad de la materia y la justificación para que el jefe de departamento o director de carrera lo acepte. Después de esto, el alumno es llevado a una pantalla donde se muestran sus materias registradas al momento, en forma de lista y también gráfica; sino pudo meter  alguna(s) materia(s), al lado de cada materia (en la lista) aparece la razón por la cual no pudo inscribirla. 
   También aparece un mensaje que dice "Alta de materia exitosa" al lado de cada materia que pudo registrar y un mensaje que dice  "Lista de espera" para las materias en las cuales está en lista de espera y una opción para editar la prioridad y la  justificación. Desde la pantalla donde aparecen las materias registradas para el alumno hasta el momento, existe una opción de seleccionar las materias registradas y darlas de baja seleccionando el botón "Dar de baja", luego regresa a la misma pantalla             en donde aparece la lista de materias con un mensaje que dice "Baja de materia" al lado de cada materia dada de baja.

   La otra interfaz es para los directores de carrera y jefes de departamento. 
   Al igual que para los alumnos, la primera pantalla de la GUI sirve para iniciar sesión y tiene los campos de usuario y contraseña; si el usuario introduce una combinación inválica de usuario/contraseña aparece un mensaje de error en la pantalla. 
   Luego de iniciar sesión, el usuario es llevado a una pantalla en donde aparecen las materias que tienen lista de espera. 
   El usuario puede seleccionar cada materia para entrar a ver qué alumnos han inscrito lista de espera para esa materia y sus prioridades y justificaciones. El usuario selecciona una cantidad limitada (indicada en el sistema) de alumnos que aceptará en la lista de espera y oprime el botón "Aceptar lista de espera". 
   Finalmente es llevado a la pantalla donde aparecen las materias que tienen lista de espera, donde las materias que ya aceptó están subrayadas en verde y las que faltan de aceptar están subrayadas en rojo.
   Ambos usuarios tienen la opción de cerrar sesión oprimiendo el botón "Cerrar sesión", que aparece en todas las pantallas, en la esquina superior derecha.

      ## 3.2 Interfaces de Hardware
   Esta plataforma es una página web a la que se puede acceder desde navegadores de internet, tanto en computadoras, como en smartphones y tabletas que tengan acceso a internet y que soporten la página.
   Los datos utilizados, que están guardados en una base de datos, son tanto categóricos, como numéricos. Los datos categóricos son nombre del alumno, plan de estudios, nombre de las materias, estatus de la materia en general (abierto, cerrado o lista de espera), estatus de la materia para cada alumno (alta, baja y lista de espera), todos estos son nominales. Los datos numéricos son ID del alumno y ID de la materia, los cuales son datos discretos.

      ## 3.3 Interfaces de software
   Este software se conecta con el software local del ITAM en donde el personal administrativo introduce las materias y sus horarios que estarán disponibles durante el semestre actual, de este software local obtiene los datos de las materias, alumnos y planes de estudio. 
   A la vez, la página de Internet envía las peticiones al software local para que éste se actualice y actualice la base de datos (alumnos inscritos en las materias, materias cerradas, etcétera). 
   El software local tiene una conexión vía la Intranet del ITAM a la base de datos que contiene la información pertinente para el semestre actual, esta información es guardada en servidores locales dentro del ITAM.
      
      ## 3.4 Interfaces de comunicación
      El software local se comunica con la página de internet de registro de materias y viceversa mediante el protocolo de comunicación HTTP.
      A le vez, este se comunica mediante el protocolo SMTP para enviar correos a los alumnos con su tira de materias al fin del periodo de inscripciones.
      A la vez, el software local se comunica con la base de datos almacenada en los servidores locales por medio de la Intranet del ITAM (protocolo TCP/IP). 
      Los datos solamente pueden ser accesados si el alumno o usuario introduce introduce las credenciales correctas para así garantizar la seguridad del sistema. Además, los datos enviados mediante los protocolos de Internet son todos encriptados para evitar robo de información. Finalmente, el sistema es resistente a ataques DoS.
      
      # 4. **Funcionalidad del sistema**
      ## 4.1 Funcionalidad 1
      ## 4.2 Funcionalidad 2
      ## 4.3 Funcionalidad 3


      # 5. Requerimientos no funcionales
      ## 5.1 Requerimientos de rendimiento
      El sistema debe garantizar el dar respuesta a las consultas en menos de 5 segundos. En especial en el día de inscripciones.
      ## 5.2 Requerimientos de seguridad
      - El sistema debe ser resistente a ataques, por ejemplo, D-DOS. Para así garantizar fiabilidad y rendimiento al usuario.
      - El sistema debe cuidar la confidencialidad de los usuarios y la integridad de los datos, esto se puede hacer mediante la encriptación de los datos enviados y recibidos por el sistema.
      ## 5.3 Requerimientos de fiabilidad
      - El sistema debe garantizar tener pocos incidentes de alta prioridad, por ejemplo, teniendo un sistema alterno que sirve como DR (Disaster Recovery) en caso de algún problema
      - El sistema debe garantizar ser resistente a un fuerte uso del sistema, por ejemplo, en día de inscripciones.
