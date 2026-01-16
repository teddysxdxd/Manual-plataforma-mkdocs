---
title: Documento de Identificación
hide:
  - toc
  - nav
---
# Documento de Identificación

Permite realizar la búsqueda de una persona indicando los datos de un documento de identificación con el que esté registrado en el sistema. 

!!! abstract "Dato clave"
    Este campo es específico; no se deben indicar más datos de combinación en la búsqueda, porque solo debe existir una persona con un documento de identificación.

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Tipo de documento** | Lista seleccionable de tipos de documentos permitidos para realizar la búsqueda. | Opcional |
| **Identificación** | Permite indicar los datos de la identificación. En base al tipo seleccionado se recupera el formato requerido. | Requerido al seleccionar un Tipo de Documento |

![Búsqueda por tipo de documento](../assets/images/busqueda_por_tipo_de_documento_de_identificacion.png)

---

[← Volver a Búsqueda de clientes](../busqueda-clientes/busqueda-clientes.md)

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