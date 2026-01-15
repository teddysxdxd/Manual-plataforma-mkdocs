# **Estándares** {style="text-align: center;"}


En esta sección se describe de forma general los estándares que son utilizados en la navegación de la aplicación.

## **Pantalla de Acceso**

Para ingresar a la aplicación, es requerido el ingreso de credenciales que permiten identificar el usuario y los permisos que este tiene para realizar operaciones en el sistema. El acceso se administra por medio de la aplicación Keycloak, que se encarga de capturar y enviar las credenciales a los servicios de seguridad establecidos, para que sean validadas y determinar si puede ingresar a la aplicación, así como las opciones a las que tiene acceso.

![Pantalla de Acceso](../../assets/images/estandares/login.png)

## **Pantalla de Inicio**

Después de ingresar los datos de credenciales para tener acceso a la aplicación, se muestra la pantalla de inicio o principal del sistema.

En la parte superior la pantalla dispone de algunas opciones de acceso rápido que se mantienen siempre visibles en la navegación de la aplicación.

| Opción | Descripción | Icono |
|--------|-------------|-------|
| Notificaciones | Indica las notificaciones pendientes de leer. | ![Icono Notificaciones](../../../assets/images/estandares/estandares_icono_1.png) |
| Autorizaciones | Muestra el portal de autorizaciones del usuario. | ![Icono Autorizaciones](../../assets/images/estandares/estandares_icono_2.png) |
| Usuario | Usuario con el que se ingresó a la aplicación. | |
| Tema e Idioma | Permite seleccionar el tema e idioma a utilizar. | ![Icono Tema](../../assets/images/estandares/estandares_icono_3.png) |
| Salir | Salir del sistema. | ![Icono Salir](../../assets/images/estandares/estandares_icono_4.png) |

![Pantalla de Inicio 1](../../assets/images/estandares/estandares_pantalla_de_inicio_2.png)

El menú de opciones está ubicado al lado izquierdo de la pantalla de inicio de la aplicación, si las opciones principales tienen más opciones, se puede expandir al seleccionar cada opción o se pueden contraer al seleccionar nuevamente la opción.

![Pantalla de Inicio 2](../../assets/images/estandares/estandares_pantalla_de_inicio2.png)

## **Formularios**

La aplicación dispone de diferentes tipos de formulario para realizar operaciones con los datos, manteniendo estándares que permitan al usuario navegar de forma fácil.

En los formularios se incluyen campos de texto libre, listas seleccionables, campos tipo fecha, campo de chequeo o verificación y en el caso de los registros, se dispone de botones de acciones para agregar, consultar, modificar o eliminar registros. No todos los formularios permiten todas las acciones, esto depende de los requerimientos establecidos para operar los registros en cada opción.

![Formularios](../../assets/images/estandares/estandares_formularios.png)

En algunas opciones como el flujo de creación de clientes, se dividen en varios pasos, pero algunos pasos tienen inmersos varios pasos que pueden ser obligatorios de completar para continuar con los pasos del flujo general.

![Pasos del Formulario](../../assets/images/estandares/estandares_pasos.png)

## **Navegación**

En los pasos de cada flujo se puede utilizar el botón para regresar (Anterior), en el caso que el usuario necesite regresar a cambiar algún dato de la información que ingresó en los pasos anteriores, una vez realizado el cambio de datos, debe continuar con el botón Siguiente. Se debe considerar que los datos principales como documentos de identificación, nombres y apellidos, género o tipo de persona, no podrán ser modificados, una vez se haya pasado al siguiente paso.

![Navegación](../../assets/images/estandares/navegacion.png)

Los botones no siempre se muestran habilitados, esto debido a que es necesario completar la información obligatoria.

En el primer paso, no se habilita el botón Anterior y en el en último paso que corresponde a Finalizar, no se habilita el botón Anterior.

## **Mensajes Informativos**

En esta sección se indican algunos mensajes generales que la aplicación puede mostrar.

## **Tiempo Espera Terminado**

Este mensaje se muestra cuando los servicios principales no responden al ejecutar una operación y no permite continuar.

![Tiempo de Espera](../../assets/images/estandares/estandares_tiempo_de_espera.png)

## **No se pudo procesar la solicitud**

Este mensaje se presenta principalmente porque no hay comunicación al servidor, puede ser por problemas de red o porque el servidor no está disponible.

![Error en solicitud](../../assets/images/estandares/estandares_ha_ocurrido_un_error.png)

## **Listas de Cautela**

El sistema realiza validaciones en listas de cautela utilizando el documento de identificación y/o el nombre de la persona, dependiendo del tipo de lista en que sea encontrada la persona, puede ser solo un mensaje informativo o puede requerir credenciales para autorizar la continuidad del flujo o detener la operación y no permitir continuar con el flujo. Se debe considerar que la validación de lista de cautela se hace solo cuando se dispone de un documento de identificación de la persona.

![Listas de Cautela](../../assets/images/estandares/persona_lista_de_cautela.png)

[← Volver a Menú plataforma](../index.md)

<style>
  /* Estilos específicos para Autorizaciones */
  .md-typeset h1 {
    color: #2d5490;
    border-bottom: 3px solid #2d5490;
    padding-bottom: 0.5rem;
  }
  
  .md-typeset h2 {
    color: #3a6bc0;
    margin-top: 2.5rem;
    padding-top: 1rem;
    border-top: 2px solid #eee;
  }
  
  .md-typeset h3 {
    color: #4a7cd0;
    margin-top: 1.8rem;
    padding-left: 1rem;
    border-left: 4px solid #2d5490;
  }
  
  .md-typeset img {
    display: block;
    margin: 2em auto;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.15);
    max-width: 100%;
    height: auto;
    border: 1px solid #ddd;
  }
  
  .md-typeset strong {
    color: #2d5490;
    font-size: 1.1em;
    background-color: #f0f7ff;
    padding: 2px 6px;
    border-radius: 4px;
    display: inline-block;
    margin: 0.5em 0;
  }
  
  /* Estilo para secciones ACEPTAR/RECHAZAR/CANCELAR */
  .md-typeset h3 + p + strong {
    font-size: 1.2em;
    padding: 8px 15px;
    margin: 1.5em 0 1em 0;
    border-left: 5px solid #2d5490;
  }
  
  /* Mejorar legibilidad de párrafos */
  .md-typeset p {
    line-height: 1.6;
    text-align: justify;
    margin-bottom: 1.2em;
  }
  
  /* Estilo para imágenes con ancho específico */
  .md-typeset img[width="400"] {
    max-width: 400px;
    width: 100%;
  }
</style>