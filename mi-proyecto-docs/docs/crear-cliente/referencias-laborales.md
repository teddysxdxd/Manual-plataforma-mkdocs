---
title: Referencias Laborales -  Persona Natural
hide:
  - toc
  - nav
---
# Referencias Laborales – Persona Natural

Registro de referencias laborales de la persona, las referencias pueden ser de una persona natural o una persona jurídica. 

![Referencias Laborales](../assets/images/20250903-220723.png)

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Tipo de Persona** | Indica si la referencia laboral corresponde a una persona natural o persona jurídica. | Obligatorio |

En base a este campo se determinan los datos que serán requeridos para crear la referencia laboral. 

Para crear una referencia laboral es requerido indicar los datos generales, dirección y datos de contacto. 

**Natural - Datos Generales – Referencia Laboral**

Los datos generales para crear una referencia laboral de persona natural se muestran en una sola pantalla, en este documento se muestran separados para describir la funcionalidad. 

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Conoce el Número de Identificación** | Indica si la persona conoce el número de identificación de la referencia laboral. Al seleccionar, es desplegada la lista de tipos de documentos de identificación correspondientes al tipo de persona. | Opcional |

Los datos requeridos por tipo de documento de identificación pueden ser número de identificación, ubicación y fecha de expiración. 

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Número** | Número de identificación del documento de la persona, el campo valida que sea ingresado en el formato configurado para el tipo de documento. | Requerido al seleccionar el campo “Conoce el número de identificación.” |
| **Ubicación** | No todos los documentos pueden requerir este dato, solo si el tipo de documento de identificación tiene configurado que requiere ubicación, será mostrado este campo. Permite indicar el lugar en donde fue emitido el documento de identificación, dependiendo de la configuración del tipo de documento puede recuperar estos datos de forma automática del número de identificación y proteger los datos de este campo para que no sean modificados. | Obligatorio al ingresar el número de identificación. |
| **Fecha de Expiración** | No todos los documentos pueden requerir este dato, es mostrado solo si el tipo de documento de identificación tiene configurado que requiere fecha de expiración. Permite indicar la fecha en la que expira el documento de identificación, la fecha no puede ser menor a la fecha actual. | Obligatorio al ingresar el número de identificación. |

El sistema realiza validaciones de lista de cautela por documento de identificación y muestra los mensajes correspondientes si encuentra la identificación en alguna lista de cautela (Notificación, Solicitar Autorización, Detener). 

Si el número de documento de identificación ingresado existe registrado en el sistema, serán recuperados los datos de la persona con campos protegidos (Datos generales, Dirección, Contacto), serán habilitados solo los campos que no poseen información. 

Del listado de tipos de documentos mostrado, hay algunos que son requeridos y otros son opcionales, esto depende como están definidos los parámetros de tipos de documentos por rol de persona, en este caso los roles “CLIENTE” para persona natural o “EMPRESA” para para persona jurídica. Si falta un tipo de documento de identificación que es requerido en esta sección, muestra un dialogo de solicitud de credenciales, para autorizar la continuidad del flujo, sin haber ingresado el tipo de documento requerido. 

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Género** | Indica si la persona es de género masculino o femenino. | Obligatorio |
| **Primer Apellido** | Primer apellido de la persona. | Obligatorio |
| **Segundo Apellido** | Segundo apellido de la persona. | Opcional |
| **Primer Nombre** | Primer nombre de la persona. | Obligatorio |
| **Segundo Nombre** | Segundo nombre de la persona. | Opcional |
| **Otros Nombres** | Otros nombres de la persona. | Opcional |
| **Fecha Ingreso** | Fecha que inició a trabajar la persona. | Obligatorio |
| **Fecha Egreso** | Fecha que finalizó de trabajar la persona. | Opcional |
| **Años de Laborar** | Muestra los años laborados por la persona en base a la fecha de ingreso y egreso o fecha actual. | Protegido |
| **Puesto** | Puesto que ocupa la persona en este trabajo. | Obligatorio |
| **Salario** | Salario devengado por la persona en este trabajo. | Obligatorio |

![Detalle Natural](../assets/images/20250903-221538.png)

**Jurídica - Datos Generales – Referencia Laboral**

Los datos generales para crear una referencia laboral de persona jurídica se muestran en una sola pantalla, en este documento se muestran separados para describir la funcionalidad. 

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Conoce el Número de Identificación** | Indica si la persona conoce el número de identificación de la referencia laboral. Al seleccionar, es desplegada la lista de tipos de documentos de identificación correspondientes al tipo de persona. | Opcional |

![Detalle Jurídica](../assets/images/20250903-221352.png)

Los datos requeridos por tipo de documento de identificación pueden ser número de identificación, ubicación y fecha de expiración. 

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Número** | Número de identificación del documento de la persona, el campo valida que sea ingresado en el formato configurado para el tipo de documento. | Requerido al seleccionar el campo “Conoce el número de identificación.” |
| **Ubicación** | No todos los documentos pueden requerir este dato, solo si el tipo de documento de identificación tiene configurado que requiere ubicación, será mostrado este campo. Permite indicar el lugar en donde fue emitido el documento, recuperándolo automáticamente si aplica. | Obligatorio al ingresar el número de identificación. |
| **Fecha de Expiración** | No todos los documentos pueden requerir este dato, es mostrado solo si el tipo de documento de identificación tiene configurado que requiere fecha de expiración. Permite indicar la fecha de expiración, la cual no puede ser menor a la actual. | Obligatorio al ingresar el número de identificación. |

El sistema realiza validaciones de lista de cautela por documento de identificación y muestra los mensajes correspondientes si encuentra la identificación en alguna lista de cautela (Notificación, Solicitar Autorización, Detener). 

Si el número de documento de identificación ingresado existe registrado en el sistema, serán recuperados los datos de la persona con campos protegidos (Datos generales, Dirección, Contacto), serán habilitados solo los campos que no poseen información. 

Del listado de tipos de documentos mostrado, hay algunos que son requeridos y otros son opcionales, esto depende como están definidos los parámetros de tipos de documentos por rol de persona, en este caso el rol de “CLIENTE”. Si falta un tipo de documento de identificación que es requerido en esta sección, muestra un dialogo de solicitud de credenciales, para autorizar la continuidad del flujo, sin haber ingresado el tipo de documento requerido. 

![Formulario Jurídico](../assets/images/20250903-221352.png)

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Nombre de la Empresa** | Nombre de la empresa. | Obligatorio |
| **Fecha Ingreso** | Fecha que inició a trabajar la persona. | Obligatorio |
| **Fecha Egreso** | Fecha que finalizó de trabajar la persona. | Opcional |
| **Años de Laborar** | Muestra los años laborados por la persona en base a la fecha de ingreso y egreso o fecha actual. | Protegido |
| **Puesto** | Puesto que ocupa la persona en este trabajo. | Obligatorio |
| **Salario** | Salario devengado por la persona en este trabajo. | Obligatorio |

**Capturar Dirección – Referencia Laboral**

Sección para ingresar los datos de dirección de la referencia laboral. 

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Correlativo** | Correlativo de la dirección creada. | Protegido |
| **País** | País al que corresponde la dirección. | Obligatorio |
| **Tipo de Dirección** | Tipo de dirección registrada, en base a la cual se determina los datos que se deben ingresar al registrar la dirección. | Protegido |
| **Buscar** | Buscador de distribución geográfica configurada para el país, se debe ingresar el texto a buscar, el sistema muestra una lista de registros coincidentes. Al seleccionar el registro, muestra los datos recuperados en el campo ubicación, agencia, información dirección y dirección referencia de búsqueda. | Obligatorio |
| **Ubicación** | Muestra los niveles geográficos recuperados en base al registro seleccionado en campo Buscar. | Protegido |
| **Agencia más Cercana** | Muestra la agencia más cercana recuperada en base al registro seleccionado en campo Buscar. | Protegido |
| **Información Dirección** | Información detallada de la dirección. | Obligatorio |
| **Especificaciones** | Información de referencias para ubicar la dirección. | Opcional |
| **Dirección Referencia Búsqueda** | Información detallada de la dirección que se puede utilizar para realizar la búsqueda de geoposición con el servicio de mapas utilizando el botón Buscar, para recuperar la latitud y longitud de la dirección. | Opcional |
| **Latitud** | Datos de latitud en donde se ubica la dirección. | Opcional |
| **Longitud** | Datos de longitud en donde se ubica la dirección. | Opcional |

![Mapa Dirección](../assets/images/referencia_laboral_10.png)

| Botón | Descripción |
| :--- | :--- |
| **Buscar** | Recupera las coordenadas en las que está localizada la dirección por medio del servicio de mapas. |
| **Encuéntrame** | Recupera en el mapa la ubicación más cercana a donde se encuentra ubicado el equipo de donde se invoque el servicio y actualiza los datos de coordenadas. |

**Capturar Contacto – Referencia Laboral**

Registro de datos de contacto de la referencia laboral de la persona. Es obligatorio registrar como mínimo un correo y un teléfono. 

Es importante considerar que los datos de contacto tanto correos electrónicos como teléfonos, no deben existir registrados con otra persona. 

## Correo

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Tipo de Correo** | Tipo de correo para contactar a la persona. | Obligatorio |
| **Correo** | Dirección de correo electrónico de la persona. El correo no debe existir registrado con otra persona. | Obligatorio |

## Teléfono

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Tipo de Teléfono** | Tipo de teléfono para contactar a la persona. | Obligatorio |
| **Teléfono** | Teléfono de la persona. El sistema sugiere el área de marcación correspondiente al país local, modificable. | Obligatorio |
| **Ubicación** | Dirección relacionada al teléfono de la persona. Muestra un listado de direcciones registradas a la persona. | Opcional |

![Contacto Teléfono](../assets/images/20250903-224002.png)

Después de ingresar los datos de contacto, se utiliza el botón Agregar para crear el registro.

![Agregar Contacto](../assets/images/20250903-224101.png)

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