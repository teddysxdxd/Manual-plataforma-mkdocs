---
title: Identificación persona natural
hide:
  - toc
  - nav
---

## Identificación persona natural

Al seleccionar la opción Cliente del botón Agregar en la Búsqueda de Clientes, se muestra el primer paso para la creación de clientes, en donde se solicitan los datos de los documentos de identificación de la persona. 

![Crear cliente persona N o J](../assets/images/crear_cliente_persona_n_o_j.png)

Es necesario indicar el tipo de persona con el que será creado el cliente, dependiendo del tipo de persona seleccionado, será mostrada la lista de tipos de documentos de identificación que puede presentar la persona para identificarse. 

Del listado de tipos de documentos mostrado, hay algunos que son requeridos y otros son opcionales, esto depende de cómo están definidos los parámetros de tipos de documentos por rol de persona “CLIENTE”.  

Es necesario el ingreso de por lo menos un documento de identificación, si no se ingresan los datos de documentos de identificación requeridos, el sistema muestra un dialogo de solicitud de credenciales, para autorizar la continuidad del flujo. 

Los datos requeridos por tipo de documento de identificación pueden ser número de identificación, ubicación y fecha de expiración. 

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Número** | Número de identificación de la persona, el campo valida que sea ingresado en el formato configurado para el tipo de documento. En base a este número de identificación, el sistema puede recuperar datos que son validados en los parámetros de ubicaciones geográficas o validar el año de nacimiento. | Es necesario ingresar al menos un documento de identificación. |
| **Ubicación** | No todos los documentos pueden requerir este dato; solo si el tipo de documento de identificación tiene configurado que requiere ubicación, será mostrado este campo. Permite indicar el lugar en donde fue emitido el documento de identificación, dependiendo de la configuración del tipo de documento, puede recuperar estos datos de forma automática del número de identificación y proteger los datos de este campo para que no sean modificados. | Obligatorio si es ingresado el número de identificación. |
| **Fecha de expiración** | No todos los documentos pueden requerir este dato, solo si el tipo de documento de identificación tiene configurado que requiere fecha de expiración, será mostrado este campo. Permite indicar la fecha en la que expira el documento de identificación; la fecha no puede ser menor a la fecha actual. | Obligatorio si es ingresado el número de identificación. |

El sistema realiza validaciones de lista de cautela por documento de identificación y muestra los mensajes correspondientes si encuentra la identificación en alguna lista de cautela (Notificación, Solicitar Autorización, Detener). 

![Validación cautela](../assets/images/validacion_lista_cautela.png)

Es necesario ingresar por lo menos los datos de un tipo de documento para habilitar el botón Siguiente. 

### Mensajes de error

| Campo | Descripción |
| :--- | :--- |
| **La entrada está incompleta** | No ha sido ingresada la información completamente conforme al formato esperado de la identificación. |
| **Ubicación requerida** | Debe seleccionar de la lista seleccionable, el lugar de emisión del documento de identificación. |
| **Documento de un tercero** | El documento de identificación ya existe relacionado a una persona creada en el sistema. |

#### Documento de identificación existe

El sistema valida cada número de identificación ingresado, para determinar si está relacionado a alguna persona existente, mostrando el mensaje correspondiente. En donde el usuario puede Cancelar y corregir el número de identificación o ir a la opción de administrar persona para consultar la información, saliendo del flujo de creación de cliente. 

![Documento existe](../assets/images/rear_cliente_3.png)

#### Autorización por Documento Requerido

Cuando falta un tipo de documento de identificación que es requerido, muestra un dialogo de solicitud de credenciales, para autorizar la continuidad del flujo sin haber ingresado el tipo de documento requerido. La solicitud puede ser autorizada de forma local o remota, dependiendo del nivel de permisos que tenga asignados el usuario y el que requiere la autorización.  

![Autorización documento](../assets/images/autorizacion_por_documento_requerido.png){ width=100% }


---

[← Volver a página anterior](crear-cliente-natural.md)

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