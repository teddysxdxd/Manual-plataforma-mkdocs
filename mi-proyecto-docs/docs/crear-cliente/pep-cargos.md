---
title: PEP Cargos - Persona natural
hide:
  - toc
  - nav
---
# PEP Cargos - Persona natural

Este paso permite capturar los datos relacionados a personas expuestas políticamente (PEP). El ingreso de datos es opcional, pero una vez creado un registro de cargos ocupados, la persona se clasifica como PEP. Serán habilitados otros pasos del flujo relacionados a personas naturales clasificadas como PEP, como la participación en empresas, parentescos y todos los datos relacionados con el cónyuge. 

![Formulario PEP Cargos](../assets/images/pep_cargos_1.png)

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Institución** | Nombre de la institución en donde la persona PEP ocupó un cargo público. Al ingresar algún texto, el sistema sugiere el listado de instituciones existentes con ese nombre. | Obligatorio si es una persona PEP. |
| **Cargo Ocupado** | Cargo que fue ocupado por la persona PEP en esa institución. Al ingresar algún texto, el sistema sugiere el listado de cargos existentes con ese nombre. | Obligatorio al ingresar la institución. |
| **País donde ocupó el cargo** | País en donde la persona PEP ocupó el cargo en la institución. | Obligatorio al ingresar la institución. |
| **Período en que ocupó el cargo** | Permite seleccionar el período de gobierno en el que la persona PEP ocupo el cargo. | Obligatorio al ingresar la institución. |

En este paso es realizada la creación del cliente y se asigna el estado correspondiente, dependiendo si es una persona PEP se asigna el estado pendiente de aprobación y cuando no es PEP se asigna el estado de prospección.

Después de agregar los registros de cargos ocupados por la persona PEP, se debe utilizar el botón Siguiente para continuar con el próximo paso y capturar datos relacionados a PEP. 

Al agregar el primer cargo público durante el flujo de creación de clientes, el sistema realiza la creación de cliente y asigna el estado del cliente para identificar que esta pendiente de aprobación por ser PEP.

Si no es creado ningún cargo público a la persona, al utilizar el botón Siguiente el sistema crea el cliente con estado de prospección para que pueda continuar con los demás pasos.

---

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