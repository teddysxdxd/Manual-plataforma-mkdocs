# **Configuraciones** {style="text-align: center;"}

En esta sección se describe las configuraciones importantes que son utilizadas en la funcionalidad de la aplicación.

## **Catálogos**

Los catálogos principales que son utilizados en la aplicación están configurados en el sistema bancario, el cual dispone los datos a través de servicios que son consumidos por la aplicación y almacenados de forma temporal para optimizar el rendimiento, esto es realizado por medio de un proceso calendarizado que se ejecuta cada día de forma automática.

![Configuración Tablas](../../../assets/images/configuraciones/configuracion_tablas.png)

**Homologación de Catálogos a Demanda**

Con esta opción el proceso de homologación de catálogos también puede ser ejecutado a demanda desde la aplicación, al ejecutar el proceso, se recomienda no salir de la opción, sino esperar a que muestre el mensaje de finalización.

![Homologación a Demanda](../../../assets/images/configuraciones/20250731-231907.png)

Durante la ejecución del proceso, las opciones y navegación el menú quedan bloqueadas.

![Proceso en Ejecución](../../../assets/images/configuraciones/20250731-232033.png)

Al finalizar muestra el mensaje indicando que el proceso finalizó correctamente.

![Proceso Finalizado](../../../assets/images/configuraciones/20250731-232107.png)

La aplicación dispone de unos catálogos de configuración propios que complementan la funcionalidad.

**Tipo Rol Persona**

Registro de los roles de persona con los que se configuran los diferentes tipos de documentos de identificación que son requeridos al crear una persona.

![Tipo Rol Persona](../../../assets/images/configuraciones/20250710-230048.png)

| Campo | Descripción | Condición |
|-------|-------------|-----------|
| Aplicación | Nombre de la aplicación con la que se utiliza el rol. | Obligatorio |
| Palabra Clave | Texto que identifica el rol a ser utilizado en la aplicación. | Obligatorio |
| Nombre | Texto descriptivo del rol. | Obligatorio |
| Elemento de Referencia | Texto de referencia relacionado al rol. | Obligatorio |
| Permite Persona Natural | Indica si el rol permite ser utilizado para persona natural, por defecto el valor es "No", se debe seleccionar para indicar que "Si". | Obligatorio |
| Permite Persona Jurídica | Indica si el rol permite ser utilizado para persona jurídica, por defecto el valor es "No", se debe seleccionar para indicar que "Si". | Obligatorio |

![Tipo Rol Persona 2](../../../assets/images/configuraciones/20250710-230152.png)

**Tipos de Documento**

Registro de los tipos de documento que puede presentar una persona para ser creado como cliente.

![Tipos de Documento](../../../assets/images/configuraciones/20250710-230435.png)

| Campo | Descripción | Condición |
|-------|-------------|-----------|
| Código | Código del tipo de documento con el que se identifica en el core. | Obligatorio |
| Etiqueta | Texto con el que se muestra el tipo de documento. | Obligatorio |
| Nombre | Texto descriptivo del tipo de documento. | Obligatorio |
| Máscara | Máscara para el ingreso del número de identificación. | Obligatorio |
| Tipo de Contenido | Tipo de contenido permitido para capturar el documento de identificación. | Obligatorio |
| Tamaño Máximo (bytes) | Tamaño máximo del archivo para capturar el documento de identificación. | Obligatorio |
| Fecha de Emisión | Indica si se muestra la fecha de emisión. | Obligatorio |
| Fecha de Expiración | Indica si se muestra la fecha de expiración o vencimiento. | Obligatorio |
| País de Emisión | | Obligatorio |
| Ver Tipo de Documento | | Obligatorio |
| Encriptar | Indica si se encripta el archivo con el documento de identificación. | Obligatorio |
| Permitir Descarga | Indica si permite descargar el archivo del documento de identificación. | Obligatorio |

![Tipos de Documento 2](../../../assets/images/configuraciones/20250710-230529.png)

**Documentos Persona Rol**

Permite configurar los diferentes tipos de documentos de identificación que son requeridos por tipo de persona y tipo de rol.

![Documentos Persona Rol](../../../assets/images/configuraciones/20250710-230236.png)

| Campo | Descripción | Condición |
|-------|-------------|-----------|
| Tipo Persona | Tipo de persona al que se relaciona el tipo de documento. | Obligatorio |
| Tipo Rol Persona | Tipo de rol al que se relaciona el tipo de documento. | Obligatorio |
| Tipo Documento | Tipo de documento relacionado al rol. | Obligatorio |
| Grupo | Nombre del grupo para combinar condiciones a varios tipos de documentos. | Opcional |
| Requerido | Indica si al crear una persona con este rol, el ingreso del documento de identificación es obligatorio. | Obligatorio |
| Digitalizar | Indica si el documento de identificación permite ser digitalizado. | Obligatorio |
| Validación Grupo | Indica las condiciones de validación ("Y"/"O") entre los documentos que corresponden a un mismo grupo. Cuando la condición es "Y", todos los documentos del grupo son obligatorios, cuando la condición es "O" solo uno de los documentos del grupo es obligatorio. | Obligatorio al indicar un grupo. |

![Documentos Persona Rol 2](../../../assets/images/configuraciones/20250710-230312.png)

**Propiedades**

Registro de las propiedades utilizadas en la aplicación para complementar datos adicionales en la captura de documentos de identificación.

![Propiedades](../../../assets/images/configuraciones/20250710-230652.png)

| Campo | Descripción | Condición |
|-------|-------------|-----------|
| Nombre | Nombre de la propiedad. | Obligatorio |

## **Permisos**

En la aplicación se utiliza la herramienta de Keycloak para configurar y validar los permisos que pueden tener de forma general los usuarios para visualizar o editar datos de clientes, así como utilizar las opciones del menú o la aprobación de solicitudes de autorizaciones locales o remotas.

![Permisos 1](../../../assets/images/configuraciones/permisos_1.png)

![Permisos 2](../../../assets/images/configuraciones/permisos_2.png)

![Permisos 4](../../../assets/images/configuraciones/permisos_4.png)

En Keycloak a nivel de la opción "Clients" opción "Authorization" se utilizan las opciones "Resources" y "Permissions" para configurar los permisos que serán utilizados en la aplicación.

![Keycloak 1](../../../assets/images/configuraciones/keycloak_1.png)

![Keycloak 3](../../../assets/images/configuraciones/keycloak3.png)

Los permisos (Permissions) se asignan en base a los recursos creados (Resources), se identifican con prefijos como "btn" para botón, "web" para opciones de menú o rutas y "authz" para identificar los que corresponde a autorizaciones, al seleccionar cada permiso se muestra el detalle de la configuración, indicando principalmente la acción y los roles que deben tener los usuarios.

![Keycloak 2](../../../assets/images/configuraciones/keycloak2.png)

Algunos permisos están a nivel de campos, como el caso del perfil económico, al utilizar la opción de editar los campos Riesgo Inicial, Riesgo Social Ambiental, Generador de Divisas y CIIU se pueden mostrar protegidos, debido a que el usuario necesita tener los permisos para editar cada campo.

![Permisos Campos](../../../assets/images/configuraciones/20250708-190531.png)

**JSON**

Los mensajes y textos mostrados en la aplicación están configurados en un archivo JSON, dependiendo del idioma en el que se desean los mensajes.

![Keycloak 4](../../../assets/images/configuraciones/keycloak4.png)

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