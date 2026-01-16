---
title: Perfil Económico - Persona Natural
hide:
  - toc
  - nav
---
# Perfil Económico – Persona Natural

Registro de los datos que permite clasificar a la persona con un perfil económico.  

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Afecto ISR** | Indica si la persona es afecta a ISR, el sistema valida que tenga ingresado el documento de identificación. Si no es afecto a ISR será requerida una autorización. | Obligatorio |
| **Actividad Económica** | Actividad económica a la que se dedica la persona. | Obligatorio |
| **Fecha Actividad Económica** | Fecha de inicio de la actividad económica. Se muestra solo cuando la actividad económica tiene configurado que requiere fecha. | Obligatorio |
| **Sector Económico** | Sector económico al que pertenece la persona. | Obligatorio |
| **Clase de Cliente** | Clase de cliente con el que es clasificada la persona. | Obligatorio |
| **Situación Laboral** | Situación laboral de la persona. En base a este dato, el sistema va a solicitar datos adicionales, como referencia laborales o datos de negocio cuando es comerciante. | Obligatorio |

![Perfil Económico General](../assets/images/20250903-181650.png)

### Otros ingresos
La sección de Otros ingresos permite indicar el detalle de los ingresos adicionales que recibe la persona. Esta sección es opcional. 

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Ingresos** | Indica el rango de los montos de ingresos que recibe la persona. | Obligatorio |
| **Observaciones** | Texto descriptivo del origen de los ingresos. | Obligatorio |

![Detalle Otros Ingresos](../assets/images/20250903-181525.png)

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