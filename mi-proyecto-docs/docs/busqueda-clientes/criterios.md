---
title: Criterios
hide:
  - toc
  - nav
---
# Criterios

El gestor dispone de criterios de inclusión o exclusión de personas, estos pueden ser combinado con los criterios de búsqueda. Si no es seleccionado ninguno, se incluyen todos los registros, los criterios deben ser seleccionados antes de ejecutar la búsqueda. 

| Campo | Descripción |
| :--- | :--- |
| **Natural** | La búsqueda recupera solo las personas naturales que coincidan con los criterios de búsqueda indicados |
| **Jurídico** | La búsqueda recupera solo las personas jurídicas que coincidan con los criterios de búsqueda indicados. |
| **Jurídico** | La búsqueda recupera solo las personas que tienen un código de cliente asignado y que coincidan con los criterios de búsqueda indicados. |

Este campo permite realizar un filtro rápido de los registros mostrados en el grid por medio de la columna Nombre. Es habilitado solo cuando la búsqueda retorna registros. 

![Criterios 1](../assets/images/criterios_1.png)

![Criterios 2](../assets/images/criterios_2.png)

Cuando la búsqueda retorna registros, se puede seleccionar uno de los registros para consultar los datos con los que ha sido grabado el cliente o para continuar el flujo de creación de cliente, si aún no se ha completado como cliente. La información que se muestre depende del estado del flujo de creación de cliente, si está completado, muestra la pantalla de Administrar persona; si está incompleto, muestra la pantalla para completar el flujo de creación de cliente. 

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