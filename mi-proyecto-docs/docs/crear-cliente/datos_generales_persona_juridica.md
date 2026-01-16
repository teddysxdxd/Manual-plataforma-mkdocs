---
title: Datos Generales - Persona Jurídica
hide:
  - toc
  - nav
---
# Datos Generales - Persona Jurídica

Este paso permite capturar los datos generales para crear una persona jurídica.

![Formulario Datos Generales](../assets/images/20250901-173554.png)

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Tipo Persona Jurídica** | Indica el tipo de persona jurídica. | Obligatorio |
| **Razón Social** | Texto del nombre de la razón social. | Obligatorio |
| **Nombre Comercial** | Texto del nombre comercial. | Obligatorio |
| **Siglas** | Siglas del nombre de la persona jurídica. | Opcional |
| **País de Origen** | País de origen de la persona jurídica. | Obligatorio |
| **Oficial de Cuentas** | Oficial de cuentas asignado. No es habilitado en este paso. | Protegido |
| **Categoría de Negocio** | Categoría con la que es clasificado el negocio. | Obligatorio |
| **Tipo de Sociedad** | Tipo de sociedad de la persona jurídica. | Obligatorio |
| **En Formación** | Indica si la persona jurídica está en proceso de formación, por defecto es “No”. | Opcional |
| **Fecha de Registro** | Fecha en la que fue registrada la persona jurídica en base a la documentación presentada. Es opcional si está “En Formación”. | Obligatorio |
| **Fecha de Inicio de Operaciones** | Fecha en la que legalmente inicia operaciones la persona jurídica. | Obligatorio |
| **Número** | Número de registro mercantil. | Obligatorio |
| **Tomo** | Número de tomo. | Opcional |
| **Página** | Número de página. | Obligatorio |
| **Patente de Comercio** | Número de patente de comercio. | Obligatorio |
| **No. Escritura / Permiso Operación** | Número de escritura o permiso de operación. | Obligatorio |

Es necesario indicar todos los datos obligatorios para habilitar el botón Siguiente.

### Validación Listas de Cautela

El sistema valida si el documento de identificación o el nombre de la persona se encuentran registrados en alguna lista de cautela, dependiendo del tipo de lista puede ser solo un mensaje informativo o puede requerir credenciales para autorizar la continuidad del flujo o detener la operación y no permitir continuar con el flujo.

![Validación Listas de Cautela](../assets/images/juridica_datos_generales_cautela.png)

[← Volver a página anterior](crear-cliente-juridica.md)

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