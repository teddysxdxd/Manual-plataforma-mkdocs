---
title: Digitalización de Documentos
hide:
  - toc
  - nav
---

# Digitalización de Documentos

Permite realizar la consulta y edición de los documentos digitalizados que tiene registrados una persona (Natural o Jurídica).

Cuando falta digitalizar algún documento, la pestaña de **Digitalización de Documentos** se muestra con un signo de admiración encerrado en un círculo. Al hacer clic en dicho icono, se despliega un mensaje informativo indicando el documento pendiente.

![Aviso documento pendiente](../assets/images/20250729-222530.png)

Al utilizar el botón **Editar**, se habilitan las opciones para gestionar los archivos del documento de identificación. Para guardar los cambios realizados, el sistema solicitará las credenciales que autorizan la modificación de los datos del cliente. 

En el caso de una **persona natural**, generalmente solo se requieren los documentos de identificación. Sin embargo, para una **persona jurídica**, pueden ser necesarios otros documentos específicos según la categoría de negocio registrada y la configuración del sistema.

![Gestión de Digitalización 1](../assets/images/administrar_digitalizacion_1.png)

![Gestión de Digitalización 2](../assets/images/administrar_digitalizacion_2.png)

Al seleccionar el icono en la columna **Documento**, el sistema permite visualizar la imagen cargada del documento de identificación.

#### Mensajes de Error

| Mensaje | Descripción |
| :--- | :--- |
| **El archivo sobrepasa el límite de peso establecido** | El tamaño del archivo es mayor al límite configurado para ese tipo de documento. |
| **Tipo de archivo: application/pdf no está permitido** | Indica que el formato PDF no está habilitado para la digitalización de ese documento específico. |

[← Volver a página anterior](administrar-persona.md)

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