---
title: Referencias Comerciales
hide:
  - toc
  - nav
---
# Referencias Comerciales

Registro de las referencias comerciales de la persona. 

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Buscar/Nombre** | Nombre de la empresa al que corresponde la referencia comercial. El sistema hace una búsqueda del nombre ingresado y muestra una lista seleccionable de los registros de personas jurídicas encontradas, al seleccionar uno de los registros recupera de forma protegida, los datos que tiene grabados la persona jurídica en los campos correspondientes. (Identificación, dirección, correo, teléfono). Los datos que no existen, se muestra el campo habilitado para que complete la información. | Obligatorio |
| **Tipo de Documento** | Tipo de documento de identificación de la referencia comercial. | Opcional |
| **Identificación** | Número de identificación de la referencia comercial. | Obligatorio al seleccionar Tipo de Documento |
| **Dirección** | Dirección de la referencia comercial. | Opcional |

Registro de datos de contacto de la referencia comercial de la persona. Es obligatorio registrar como mínimo un correo y un teléfono. 

Es importante considerar que los datos de contacto tanto correos electrónicos como teléfonos, no deben existir registrados con otra persona. 

## Correo Electrónico

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Tipo de Correo** | Tipo de correo para contactar a la persona. | Obligatorio |
| **Correo** | Dirección de correo electrónico de la persona. El correo no debe existir registrado con otra persona. | Obligatorio |

## Teléfono

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Tipo de Teléfono** | Tipo de teléfono para contactar a la persona. | Obligatorio |
| **Teléfono** | Teléfono de la persona. El sistema sugiere el área de marcación correspondiente al país local, el cual se puede modificar. El teléfono no debe existir registrado con otra persona. | Obligatorio |
| **Ubicación** | Dirección relacionada al teléfono de la persona. Muestra un listado de direcciones registradas a la persona. | Opcional |

![Referencias Comerciales](../assets/images/refrencias_comerciales_14.2.png)

[← Volver a página anterior](referencias.md)

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