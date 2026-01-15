# **Autorizaciones** {style="text-align: center;"}

En varias opciones del sistema, dependiendo de las operaciones que se estén realizando, puede ser requerida la autorización con credenciales de otro usuario o del mismo para permitir que continue con la operación, siempre que tenga los permisos en Keycloak para aprobar la autorización requerida.

Las autorizaciones pueden ser otorgadas de dos formas, **Locales** cuando en la estación de trabajo del operador se permite el ingreso de usuario y contraseña de la persona que autoriza la operación; **Remotas** cuando desde otro sitio un usuario que está dentro del sistema puede autorizar a distancia la operación.

## **Autorización Local**

Cuando una operación requiere de autorización, muestra el mismo dialogo, en donde se debe seleccionar el tipo de autorización que será realizado, en este caso local.

![Autorizaciones Locales](../../../assets/images/autorizaciones/autorizaciones_locales.png)

Se debe ingresar el usuario y contraseña con el que se autoriza la solicitud.

![Autorizaciones Locales 2](../../../assets/images/autorizaciones/autorizaciones_locales2.png)

Si las credenciales son válidas, muestra el mensaje que la solicitud ha sido aprobada, de lo contrario muestra el mensaje correspondiente indicando que el usuario y la contraseña no son válidos.

![Autorizaciones Locales 3](../../../assets/images/autorizaciones/autorizaciones_locales3.png "Autorizaciones locales")

## **Autorización Remota**

Cuando una operación requiere de autorización, muestra el mismo dialogo, en donde se debe seleccionar el tipo de autorización que será realizado, en este caso remota.

![Autorización Remota](../../../assets/images/autorizaciones/administracion_remota.png)

Se queda a espera de la autorización remota, hasta que sea autorizada o rechazada, el usuario también puede decidir cancelar la solicitud de autorización remota. El sistema envía notificación a los usuarios que estén configurados para que atiendan la solicitud de autorización remota.

![Espera Autorización Remota](../../../assets/images/autorizaciones/captura_de_pantalla_2025-06-18_a_la_s_12.00.55.png)

Si después de un tiempo establecido no se obtiene respuesta será mostrado el mensaje de conexión perdida, el usuario tendrá que confirmar la operación nuevamente, para retornar a la solicitud de autorización y seleccionar la autorización remota.

![Conexión Perdida](../../../assets/images/autorizaciones/captura_de_pantalla_2025-06-18_a_la_s_12.01.23.png)

La persona que realizar la autorización remota, estando dentro de la aplicación, debe ingresar a la opción de Autorizaciones, en donde se puede dar seguimiento a cada solicitud de autorización.

![Portal Autorizaciones](../../../assets/images/autorizaciones/captura_de_pantalla_2025-06-18_a_la_s_12.01.41.png)

En esta opción inicialmente se muestran el listado de autorizaciones pendientes, en donde el usuario puede buscar por orden o por medio de filtros la solicitud y consultar el detalle.

Los filtros pueden ser realizados por fecha (hoy o rango de fechas) y por UUID de solicitud.

![Filtros Autorizaciones](../../../assets/images/autorizaciones/captura_de_pantalla_2025-06-18_a_la_s_12.00.01.png)

La solicitud se puede aceptar o rechazar, dependerá de la persona que analiza la solicitud para decidir qué acción a realizar.

![Detalle Solicitud](../../../assets/images/autorizaciones/captura_de_pantalla_2025-06-18_a_la_s_12.00.11.png)

### **ACEPTAR**

Debe indicar el motivo y seleccionar la opción Autorizar.

![Autorizar Solicitud](../../../assets/images/autorizaciones/captura_de_pantalla_2025-06-18_a_la_s_12.36.53.png)

El usuario solicitante que está a espera de la autorización de la operación, recibe el mensaje correspondiente, indicando que la solicitud ha sido aprobada y se enviaran las notificaciones que la solicitud ya fue aprobada.

![Solicitud Aprobada](../../../assets/images/autorizaciones/autorizar_701.png)

Al seleccionar Continuar, se ejecuta la operación autorizada.

### **RECHAZAR**

Debe indicar el motivo y seleccionar la opción Rechazar.

![Rechazar Autorización](../../../assets/images/autorizaciones/rechazar_autorizacion.png)

El usuario solicitante que está a espera de la autorización de la operación, recibe el mensaje correspondiente, indicando que la solicitud ha sido denegada y se enviaran las notificaciones que la solicitud ya fue denegada.

![Solicitud Denegada](../../../assets/images/autorizaciones/autorizar_702.png)

Al seleccionar Continuar, el sistema lo retorna a la pantalla de operación desde donde se originó la solicitud, sin actualizar los datos de la operación.

### **CANCELAR AUTORIZACIÓN**

Cuando la solicitud se queda a espera de la autorización remota, el usuario puede decidir cancelar la solicitud de autorización remota, al cancelar el sistema muestra el mensaje que la solicitud ha sido cancelada y envía las notificaciones correspondientes para indicar el número de solicitud que fue cancelado.

![Cancelar Autorización](../../../assets/images/autorizaciones/cancelar_autorizacion_703.png)

El portal de autorizaciones separa las peticiones en tres secciones para facilitar la búsqueda al usuario, inicialmente muestra las solicitudes pendientes de ser aprobadas, pero también se puede consultar las solicitudes que fueron autorizadas y las que fueron rechazadas, permitiendo analizar el detalle de los datos, solo las solicitudes canceladas por el usuario no se muestran, porque no tienen ninguna implicación en el sistema.

![Portal Autorizaciones 1](../../../assets/images/autorizaciones/autorizaciones_portal.png)

![Portal Autorizaciones 2](../../../assets/images/autorizaciones/autorizaciones_portal_2.png)

[← Volver a página anterior](../index.md)

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