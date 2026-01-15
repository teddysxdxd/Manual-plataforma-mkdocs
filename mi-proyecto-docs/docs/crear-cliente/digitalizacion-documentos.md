# Digitalización de documentos – Persona Natural

Registro digitalizado de los documentos de identificación presentados por la persona. En el caso de persona natural solo requiere los documentos de identificación, pero en el caso de persona jurídica, dependiendo de la categoría de negocio registrada, pueden ser requerido algunos otros documentos específicos, dependiendo de la configuración de digitalización de documentos en el sistema.  

El registro de las imágenes es obligatorio, el sistema valida que hayan sido agregadas las imágenes de cada documento de identificación, si falta algún documento de identificación, el sistema muestra un dialogo de solicitud de credenciales, para autorizar la continuidad del flujo. 

![Digitalización de documentos](../assets/images/20250904-184929.png)

Para adjuntar las imágenes de los documentos de identificación, se debe seleccionar el documento en la acción (+), se muestran el campo donde se puede hacer clic para buscar la imagen o arrastrar la imagen al área delimitada por una línea punteada.  

![Carga de archivo](../assets/images/20250904-183411.png)

Al seleccionar el directorio en donde están ubicadas las imágenes, se muestran habilitados los tipos de archivos que el sistema permite adjuntar, los demás archivos se muestran deshabilitados para selección. 

![Explorador de archivos](../assets/images/20250904-183600.png)

Una vez seleccionado el archivo, se muestra el nombre del archivo, se pueden agregar algunas notas relacionadas al documento, al Guardar será realizada la carga de la imagen al sistema.  

![Guardar documento](../assets/images/20250904-183737.png)

En la columna Documento se muestra un icono de archivo, para indicar que el documento ya fue cargado al sistema, con la opción de Editar se puede cambiar los datos e incluso adjuntar nuevamente el archivo. 

![Estado de carga](../assets/images/20250904-184929.png)

Si falta digitalizar algún documento y se utiliza el botón Siguiente, el sistema solicita las credenciales para autorizar continuar con el flujo sin adjuntar las imágenes de los documentos. 

![Solicitud de credenciales](../assets/images/20250904-185226.png)

Si todos los documentos han sido adjuntados, el sistema permite continuar con el flujo de creación de clientes. 

![Flujo completado](../assets/images/20250904-185545.png)

| Mensaje | Descripción |
| :--- | :--- |
| **El archivo sobrepasa el límite de peso establecido** | El tamaño del archivo es mayor al establecido en la configuración de digitalización para el tipo de documento. |
| **Tipo de archivo: application/pdf no está permitido** | Indica que el tipo de archivo (pdf), no esta permitido digitalizar para el tipo de documento. |

[← Volver a página anterior](crear-cliente-natural.md)