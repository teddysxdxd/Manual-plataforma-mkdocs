# Datos de Negocio – Persona Natural

Registro de los datos de negocios que posee la persona natural. 

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Estado** | Indica el estado del negocio. Al agregar se muestra como Activo, al eliminar se muestra como Inactivo. | Protegido |
| **Nombre de la Empresa** | Nombre de la empresa. | Obligatorio |
| **Fecha de Inscripción** | Fecha de inscripción o inicio de operación del negocio. | Obligatorio |
| **Años de Operación** | Muestra los años de operación en base a la fecha de inscripción. | Protegido |
| **Giro del Negocio** | Texto que describe el giro del negocio. | Obligatorio |
| **Ingresos Mensuales** | Monto de los ingresos mensuales que genera el negocio | Obligatorio |
| **Categoría de Negocio** | Texto que describe la categoría en la que se clasifica el negocio. | Obligatorio |

![Formulario Datos de Negocio](../assets/images/20250728-223338.png)

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Correlativo** | Correlativo de la dirección. | Protegido |
| **País** | País al que corresponde la dirección. | Obligatorio |
| **Tipo de Dirección** | Tipo de dirección registrada, en base a la cual se determina lo datos que se deben ingresar al registrar la dirección. | Protegido |
| **Buscar** | Buscador de distribución geográfica configurada para el país, se debe ingresar el texto a buscar, el sistema muestra una lista de registros coincidentes. Al seleccionar el registro, muestra los datos recuperados en el campo ubicación, agencia, información dirección y dirección referencia de búsqueda. | Obligatorio |
| **Ubicación** | Muestra los niveles geográficos recuperados en base al registro seleccionado en campo Buscar. | Protegido |
| **Agencia más Cercana** | Muestra la agencia más cercana recuperada en base al registro seleccionado en campo Buscar. | Protegido |
| **Información Dirección** | Información detallada de la dirección. | Obligatorio |
| **Especificaciones** | Información de referencias para ubicar la dirección. | Opcional |
| **Dirección Referencia Búsqueda** | Información detallada de la dirección que se puede utilizar para realizar la búsqueda de geoposición con el servicio de mapas utilizando el botón Buscar, para recuperar la latitud y longitud de la dirección. | Opcional |
| **Latitud** | Datos de latitud en donde se ubica la dirección. | Opcional |
| **Longitud** | Datos de longitud en donde se ubica la dirección. | Opcional |

![Detalle Dirección Negocio](../assets/images/20250728-223416.png)

[← Volver a página anterior](crear-cliente-natural.md)