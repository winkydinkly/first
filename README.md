# AVYRA Agenda Virtual
...
## 1. Fundamentos del sistema
Avyra es una agenda virtual que tiene como objetivo proporcionar a estudiantes con herramientas de estudio que estén recogidas en un mismo lugar, y que con sus automatizaciones agilice el uso de estas.

### Funcionamiento

Se basará en la creación de pestañas para cada curso, así como un apartado general donde, si bien existen varios cursos a la vez, se combinarán todos los datos de todos los cursos. Es decir, si existe un calendario para curso A, y otro para curso B, en el general se combinarán los datos de todos los calendarios existentes. De igual manera se combinarán los calendarios de cada asignatura. 

Esto es que cada apartado tendrá sus propias vistas de cada base de datos, y estas, a su vez, se irán acumulando según la siguiente jerarquía:

- asignatura
- curso
- general

### Licencia

Avyra será un software de subscipción que busca poder ser accesible parar la mayor cantidad de estudiantes posible. La mayoría de funciones premium se resumen en personalización: temas, fuentes, tono de notificación para versión móvil...

Tambíen, funciones IA como flashcards o actividades de estudio.

## 2. Análisis y especificación de requisitiso

>### Requisitos Funcionales: 

- El sistema debe seguir una jerarquía modular.
  
- El sistema emitirá una ventana de inicio de sesión/registro.
  
- Emitirá un correo electrónico para verificar la creación de la cuenta o el Inicio de sesión.
  
- El sistema generará las pestañas generales.
  
- El sistema permitirá a los usuarios la creación de nuevas pestañas adicionales fuera del sector de pestañas general.
Al ingresar nuevas pestañas, el sistema debe automatizar la creación de subcategorías (Ciclo → Asignaturas, Calendario, Horario, etc).

- El sistema debe poder reconocer que, de solo existir un ciclo, el horario de dicho ciclo se asigna automáticamente como Horario de la categoría general.
  
- El orden de los elementos de la pestaña general es editable, pero debe permanecer dentro de esa categoría.
De igual manera, el orden de los elementos de cada categoría sólo puede editarse dentro de esa categoría: no puedo sacar la asignatura “Biología” al vacío.

- El sistema debe automatizar los datos y aglomerarlos en la categoría general. Debe ser capaz de comprender que si en Ciclo A tengo 3 horas y en Ciclo 2 tengo 6 horas de distintas asignaturas, en el horario general debe unificar los dos.

- El usuario debe ser capaz de modificar y editar el nombre de las asignaturas, el ciclo, las tareas, las fechas, el calendario, los horarios, entre otras. 

- El sistema debe pedir acceso a documentos para la subida de apuntes.
  
- La aplicación debe poder utilizarse sin necesidad de instalar ningún software adicional además de un navegador web.
  
- El sistema permitirá compartir páginas con otros usuarios parecido a como funciona google docs.
  
- El sistema debe contener gestión de permisos- lector, miembro, administrador.
  
- El sistema debe contener un foro únicamente para los participantes de dicha agenda (no debe actuar como red social. Los foros y los chats son para comunicarse entre compañeros del estudio, para resolver dudas, etc).
  
- El sistema debe cambiar la subida de apuntes, tareas etc en un curso compartido a un estado de pendiente.
  
- El administrador recibirá notificaciones y aceptará la subida de dicho contenido
  
- El sistema deberá encriptar los valores de la nota dentro del campo exámenes y de evaluación
  
- El usuario podrá seleccionar si prefiere adjuntar en privado (para su agenda) o en público para los demás estudiantes.


**Para usuarios que paguen la suscripción:**

- El sistema debe ofrecer varias opciones de suscripción: mensual, anual…
  
- El sistema debe poder realizar transacciones.
  
- El sistema emitirá correos para verificar los pagos.


(El modo estudio, una vez suscrito, se anexará a la categoría general)

- El sistema debe incluir IAs para la elaboración de flashcards y organización automatizada de apuntes.
  
- La última función es completamente opcional: incluso con el plan de suscripción, la función IA debe ser seleccionada manualmente cada vez que se quiera usar, NO automáticamente.

- El sistema debe incluir temporizadores editables por el usuario para el modo estudio.
  
- El sistema debe incluir un horario semanal y diario donde podrá asignar horas por asignatura, y dentro de estas, los temas a cubrir (más opcional y flexible, cada usuario lo modifica a su gusto).
  
- El sistema debe bloquear personalización, aparte de las opciones dentro del plan gratuito (temas claro, oscuro, alto contraste para cada uno de ellos, así como la fuente estándar normal, bold, y la fuente para dislexia), para todos aquellos usuarios que no paguen la suscripción.


> ### Requisitos no funcionales:

- El sistema debe ser intuitivo y en su mayoría visual.
  
- El sistema debe contener un cifrado encriptado para que ciertos apartados como los valores de las notas y las evaluaciones sean sólo accesibles para el usuario en particular. El admin tampoco tiene acceso.
  
- Las páginas de la aplicación deben cargar en un tiempo promedio de menos de 2 segundos, incluso con alta carga de usuarios.
  
- El software podrá ser utilizado en los sistemas operativos Windows, Linux y OSX.
  
- La aplicación debe poder utilizarse con los navegadores web Chrome, Firefox e Internet Explorer.
  
- El sistema debe poder permitir la personalización de los temas y las fuentes fuera de lo predeterminado si tiene el plan de suscripción.
  
- La sincronización de apuntes (u otros) entre usuarios debe ser casi inmediata.
  
- La app debe ser compatible con opciones de accesibilidad como alto contraste y fuentes para dislexia.
  
- La plataforma debe soportar simultáneamente al menos 10.000 usuarios activos
  
- La base de datos debe poder crecer de manera eficiente para cursos, apuntes y notas privadas.
  
- El sistema debe permitir actualizaciones de la app sin pérdida de datos del usuario.
  
- La transición de web a app no debe modificar los ajustes y las preferencias del usuario.

## 3. Diseño

El software se diseñará mediante método scrum, un método ágil que ayudará a compaginar mejor las necesiades del usuario con el funcionamiento del software.

### Historias de usuario

- *Como usuario*, quiero *poder* elegir entre poder subir archivos en privado o en público en una agenda colaborativa *para* poder subir los apuntes/esquemas realizados por mi.

- *Como administrador* de la agenda, *quiero* poder revisar qué apuntes están subiendo los demás miembros de la colaboración para *poder* evitar posibles situaciones feas.

### Diagramas de flujo

![imagen 1](images/image1.png)

![imagen 2](images/image2.png)

![imagen 3](images/image3.png)


## 4. Implementación
Añade aquí aunque no tenga que ver con el proyecto, los ejercicios donde tuviste que corregir el código "feo"

## 5. Plan de pruebas del sistema
Añade aquí lo que hicimos para diseñar las pruebas

### 5.1. Pruebas de aceptación
Nada por aquí 

## 7. Los diccionarios de datos

No hagas nada por aquí
