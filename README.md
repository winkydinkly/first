# AVYRA Agenda Virtual

---

<img src = "https://github.com/user-attachments/assets/9d9effff-1fe6-4f77-8637-c5a3d44ba30b" width = "250"/>

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

###### *He intentado incluirlos pero no he podido porque las imagenes son capturas de pantalla.*

## 4. Implementación

     /**
     * Clase Hola
     *
     * Muestra por pantalla si la condición se cumple
     *
     * @author pipilla
     * 
     * @version 1.0
     */
    public class Hola
    {

        public static void main(String args[])
        {

            System.out.println("Hola mundo");
            
            if(true)
            {
                
                System.out.println("Condición verdadera");
                
            } else
                {
                    
                    System.out.println("Condición falsa");
                    
                }
            
        }
        
    }

---

     /**
     * Clase Area
     *
     * Calcula el area
     *
     * @author Yo
     * 
     * @version 1.0
     */

    public class Area
    {

        public static void main(String[] args)
        {
            
            double r = 5;
            
            double pi = 3.14159;
            
            double area = pi * r * r;

            System.out.println("el area es "+ area);
            
        }
        
    }

---

    /**
     * Clase Hola
     *
     * Recopila una serie de operaciones matemáticas
     *
     * @param num1 primer número
     * 
     * @param num2 segundo número
     * 
     * @author Yo 
     * 
     * @version 1.0
     */
    
    public class OperacionesMatematicas {

     
        public static int sumar(int num1, int num2)
        {
            
            return num1 + num2;
            
        }
        
        public static int restar(int num1, int num2)
        {
            
            return num2 - num1;
            
        }
        
        public static int mult(int num1,int num2)
        {
            
            return num1 * num2;
            
        }
        
        public static int div(int num1, int num2)
        {

            return num1 / num2;
            
        }
        
        public static void main(String[] args)
        {
            
            System.out.println(sumar(3,4));
            
            System.out.println(restar(5,2));
            
            System.out.println(mult(2,6));
            
            System.out.println(div(8,2));

        }
        
    }


---


    /**
     * Clase Calculadora
     *
     * Esta clase calcula operaciones
     *
     * @author Yo
     * 
     * @version 1.0
     */

    
        public class Calculadora 
        {
            
    /** Este método suma dos números */
    
        public int sumar(int x, int y)
        {
            
            return x + y;   
            
        }
        
    /** Este método resta dos números */
    
        public int restar(int x, int y)
        {
            
            return x - y;
            
        }
        
    /** Este método multiplica dos números */
        public int multiplicar(int x, int y)
        {
    
            return x * y;
            
        }
    
    /** Este método divide dos números */
    
        public int dividir(int x, int y)
        {
    
            return x / y; 
            
        }
    
        public static void main(String[] args)
        {
        
            Calculadora c = new Calculadora();
            
            System.out.println("resultado: " + c.sumar (5,3));
       }
            
     }


---

    /**
     * Clase Alumno
     *
     * Esta clase recoge los datos del alumno
     *
     * @author Yo
     * 
     * @version 1.0
     */

    public class Alumno
    {
        private String NOMBRE;
    
        private int edad;
        
        private double notaFinal;

        public alumno(String n,int e,double nf)
        {

           NOMBRE = n;
          
           edad = e; 

           notaFinal = nf;
         
        }
        
        public void Mostrardatos()
        {
            System.out.println("Alumno: "+ NOMBRE +", Edad:" + edad + ", Nota Final:" + NotaFinal);
            
        }
        
        public boolean aprobado()
        {
            if(NotaFinal>=5.0)
            {
                return true;
                
            }else{
                
                return false;
                
            }
            
        }
        
        
    /**
     * Muestra por pantalla si ha aprobado o no
     *
     */

        public void mensajeFinal()
        {
            if(aprobado())
            {
                System.out.println("felicidades " + NOMBRE + " aprobaste!");
                
            }else{
                
                System.out.println("Lo siento " + NOMBRE + " no aprobaste");
                
            }
            
        }
    }


    /**
     * Clase Curso
     *
     * Esta clase recoge los datos del curso
     *
     * @author Yo
     * 
     * @version 1.0
     */
    public class Curso
    {
        private String NOMBRE_CURSO;
        
        private alumno[] lista;

        public curso(String n, alumno[]1) 
        {
        
           NOMBRE_CURSO = n;

           lista = l;

        }

        public void mostrarTodo()
        {
            System.out.println("curso: "+ NOMBRE_CURSO);
            
            for(alumno a:lista)
            {
                a.Mostrardatos();
                
                a.mensajeFinal();
                
            }
            
        }

        /**
         * Recopila todos los datos para crear un curso específico
         *
         */
        public static void main(String[] args)
        {
            
            Alumno a1 = new Alumno("ana",18,6.5);
    
            Alumno a2 = new Alumno("PEDRO",19,4.3);
            
            Alumno a3 = new Alumno("Lucia",17,8.7);
    
            Alumno[] lista = {a1,a2,a3};
            
            Curso c1 = new Curso("programacion",lista);
            
            c1.mostrarTodo();
            
        }
        
    }




## 5. Plan de pruebas del sistema


**Caso de uso 1: Registrar usuario**

Requisito funcional: El sistema debe permitir a un nuevo usuario crear una cuenta, validando que el correo no exista y enviando un correo de verificación para activar el perfil.

| Tipo de prueba | Entrada / acción | Resultado |
| :---- | :---- | :---- |
| Funcional | Usuario introduce un correo nuevo y datos válidos | El sistema registra al usuario y envía correo de verificación |
| Funcional / Negativa | Usuario introduce un correo ya registrado | El sistema muestra un mensaje de error indicando que el correo ya existe |



**Caso de uso 2: Iniciar sesión con autenticación segura**

Requisito funcional: El sistema debe autenticar a los usuarios mediante correo y contraseña cifrada, y ofrecer la opción de inicio de sesión con Google o Microsoft.

| Tipo de prueba | Entrada / acción | Resultado |
| :---- | :---- | :---- |
| Funcional | El usuario introduce el correcto y la contraseña. | El sistema envía correo de verificación y una vez verificado accede a su cuenta |
| Funcional | El usuario inicia sesión a través de Google o Microsoft | El sistema realiza todo lo necesario para automatizar el proceso (esto es, si se usa verificación doble notificar al dispositivo de acceso) y una vez verificado, el usuario accede a su cuenta |
| Funcional / Negativa | Usuario no tiene una cuenta | El sistema muestra un mensaje de error indicando que aún no está registrado y le pregunta si quiere registrarse ahora |
| Funcional / Negativa | El usuario no tiene ninguna cuenta vinculada a las opciones de Google/Microsoft | El sistema notifica al usuario y le pregunta si quiere crear una cuenta o vincular una existente a Google o Microsoft |
| Rendimiento | El usuario inicia sesión y.. | ..en menos de 10 segundos el resultado debe haberse mostrado por pantalla |



**Caso de uso 3: Cerrar sesión en todos los dispositivos**

Requisito funcional: El sistema debe permitir al usuario cerrar su sesión activa en todos los dispositivos desde el panel de seguridad.

| Tipo de prueba | Entrada / acción | Resultado |
| :---- | :---- | :---- |
| Funcional | Usuario cierra sesión en todos los dispositivos | Todas las sesiones de todos los dispositivos vinculados se cierran simultáneamente. |



**Caso de uso 4: Recuperar contraseña mediante enlace temporal**

Requisito funcional: El sistema debe permitir restablecer la contraseña enviando un enlace temporal al correo del usuario, con caducidad de 15 minutos.

| Tipo de prueba | Entrada / acción | Resultado |
| :---- | :---- | :---- |
| Funcional | Usuario solicita un enlace a cambio de contraseña | El sistema envía un enlace temporal que caduca en 15 minutos. |
| Funcional / Negativa | Usuario solicita un enlace a cambio de contraseña pero tarda más de 15 minutos. | El sistema muestra un mensaje de error indicando que el enlace ha caducado y reenvía al usuario para que solicite otro si lo necesita. |



**Caso de uso 5: Actualizar perfil profesional**

Requisito funcional: El sistema debe permitir editar los datos personales y profesionales (nombre, foto, puesto, redes sociales), guardando cambios en tiempo real.

| Tipo de prueba | Entrada / acción | Resultado |
| :---- | :---- | :---- |
| Funcional | El usuario edita datos personales | El sistema los guarda |
| Funcional / Negativa | El usuario edita datos personales a algún formato no valido  | El sistema notifica del error y solicita un reintento. |
| Rendimiento | El usuario edita los datos personales | Y estos se guardan a tiempo real. |



**Caso de uso 6: Subir archivos y documentos al proyecto**

Requisito funcional: El sistema debe permitir al usuario subir archivos (PDF, imágenes o CSV) de hasta 10 MB, validando el formato y guardándolos en la nube con versión automática.

| Tipo de prueba | Entrada / acción | Resultado |
| :---- | :---- | :---- |
| Funcional | Usuario sube archivo | El sistema valida el formato y lo guarda en la nube  |
| Funcional / Negativa | Usuario sube archivo sobrepasando límite de tamaño o de formato inválido | Sistema muestra error indicando cuál de los dos ha sido |



**Caso de uso 7: Buscar oportunidades o proyectos activos**

Requisito funcional: El sistema debe permitir realizar búsquedas filtradas por palabra clave, cliente o estado del proyecto, mostrando resultados relevantes en menos de 2 segundos.

| Tipo de prueba | Entrada / acción | Resultado |
| :---- | :---- | :---- |
| Funcional | Usuario introduce filtro en la búsqueda | El sistema muestra los resultados relevantes |
| Funcional / Negativa | Usuario introduce un filtro para el cual no hay resultado | El sistema muestra que no hay resultados coincidentes. |
| Rendimiento | El usuario realiza una búsqueda con filtro | El filtro se aplica y muestra resultados en menos de 2 segundos |



**Caso de uso 8: Generar informe de rendimiento mensual**

Requisito funcional: El sistema debe permitir generar informes en PDF o Excel con métricas actualizadas (usuarios activos, ventas, incidencias), y ofrecer la descarga inmediata.

| Tipo de prueba | Entrada / acción | Resultado |
| :---- | :---- | :---- |
| Funcional | Usuario genera un informe en PDF o Excel | El sistema lo muestra con métricas actualizadas y ofrece la descarga  |
| Funcional | El usuario solicita la descarga | El sistema descarga el documento |



**Caso de uso 9: Enviar notificaciones automáticas de eventos**

Requisito funcional: El sistema debe enviar notificaciones por correo o dentro de la aplicación cuando ocurran eventos relevantes (nuevo comentario, tarea asignada, renovación próxima).

| Tipo de prueba | Entrada / acción | Resultado |
| :---- | :---- | :---- |
| Funcional | Ocurre un evento relevante | Se notifica al usuario por correo o dentro de la app |
| Funcional | Ocurre un evento relevante pero el usuario tiene las notificaciones desactivadas | No se notifica al usuario |



**Caso de uso 10: Gestionar roles y permisos de usuario (rol administrador)**

Requisito funcional: El sistema debe permitir al administrador asignar, modificar o revocar roles y permisos, registrando todas las acciones en el log de auditoría.

| Tipo de prueba | Entrada / acción | Resultado |
| :---- | :---- | :---- |
| Funcional | El usuario modifica algún permiso | El sistema lo registra en el log a tiempo real |



**Caso de uso 11: Validar métricas financieras (caso tipo SaaS empresarial)**

Requisito funcional: El sistema debe comparar los ingresos mensuales actuales con los históricos (MRR, ARR) y marcar automáticamente anomalías o diferencias significativas.

| Tipo de prueba | Entrada / acción | Resultado |
| :---- | :---- | :---- |
| Funcional | El sistema compara ingresos mensuales con históricos | Marca anomalías o diferencias significativas |
| Funcional  | El sistema compara ingresos mensuales con históricos pero no se da ninguna anomalía | El sistema no marca nada. |



**Caso de uso 12: Eliminar cuenta y todos los datos personales**

Requisito funcional: El sistema debe permitir al usuario eliminar su cuenta de forma permanente, asegurando la eliminación completa de los datos conforme al RGPD.

| Tipo de prueba | Entrada / acción | Resultado |
| :---- | :---- | :---- |
| Funcional | El usuario elimina su cuenta de forma permanente | Se manda un correo de verificación y se elimina  |
| Funcional / Negativa | El usuario elimina su cuenta de forma permanente | El sistema trata de verificar y si falla no permite que se elimine |
| Rendimiento | El usuario elimina su cuenta | Todos los datos se eliminan cumpliendo el RGPD. |


### 5.1. Pruebas de aceptación

<img src = "https://media.tenor.com/zquJuMNTpdQAAAAM/dog-wave-h2di.gif" width = "200" />

## 7. Los diccionarios de datos

<img src = "https://gifdb.com/images/high/golden-retriever-puppy-cute-animal-zu8hkoirl1sx4de1.webp" width = "200" />
