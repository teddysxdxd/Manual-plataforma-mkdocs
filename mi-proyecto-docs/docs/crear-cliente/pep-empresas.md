---
title: PEP Empresas - Persona natural
hide:
  - toc
  - nav
---
# PEP Empresas - Persona natural

Permite registrar la información de las empresas en las cuales la persona PEP tiene alguna participación como accionista, un puesto significante en la dirección de una empresa o posee afiliación en empresas no lucrativas. Se debe ingresar información solo en las secciones en donde la persona PEP tiene relación con alguna empresa. 

La creación de registros en estas secciones no es obligatoria, es permitido utilizar el botón **Siguiente** para continuar con el próximo paso. 

## Empresas

Sección para agregar las empresas en las que la persona PEP tiene algún porcentaje de participación como accionista. 

![Sección Empresas](../assets/images/pep_empresas_accionista.png)

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Empresa** | Nombre de la empresa en donde la persona PEP posee un porcentaje de participación como accionista. Al ingresar el nombre, el sistema sugiere el listado de empresas (persona jurídica) que ya están registradas en el sistema con ese nombre, para que pueda ser seleccionado, de lo contrario se puede crear una nueva. | Opcional. |
| **Tipo de Documento** | Tipo de documento con el que se identifica la empresa. El campo muestra una lista desplegable de tipos de documento. | Obligatorio al ingresar empresa. |
| **Identificación** | Número con el que se identifica la empresa, relacionado al tipo de documento seleccionado. | Obligatorio al ingresar empresa. |
| **Actividad Económica** | Actividad económica a la que se dedica la empresa. El campo muestra una lista desplegable de actividades. | Obligatorio al ingresar empresa. |
| **Fecha Actividad Económica** | Fecha de inicio de actividad económica. Este campo es mostrado solo si la actividad económica tiene configurado que requiere fecha. | Obligatorio |
| **% de Participación** | Porcentaje de participación que la persona tiene como accionista en la empresa. | Obligatorio al ingresar empresa. |

---

## Organización/Dirección de Empresas

Sección para agregar las empresas en las que la persona PEP ocupa un puesto significativo de control, gerencia, dirección o firmante dentro de la empresa. 

![Sección Dirección](../assets/images/pep_empresas_direccion.png)

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Empresa** | Nombre de la empresa en donde la persona PEP posee un puesto significativo en la organización o dirección. Al ingresar el nombre, el sistema sugiere el listado de empresas (persona jurídica) que ya están registradas en el sistema con ese nombre, para que pueda ser seleccionado, de lo contrario se puede crear una nueva. | Opcional. |
| **Tipo de Documento** | Tipo de documento con el que se identifica la empresa. El campo muestra una lista desplegable de tipos de documento. | Obligatorio al ingresar empresa. |
| **Identificación** | Número con el que se identifica la empresa, relacionado al tipo de documento seleccionado. | Obligatorio al ingresar empresa. |
| **Fecha Inicial** | Fecha a partir de la cual ocupa el puesto en la empresa. | Obligatorio al ingresar empresa. |
| **Fecha Final** | Fecha de finalización del puesto en la empresa. | Opcional |
| **Actividad Económica** | Actividad económica a la que se dedica la empresa. El campo muestra una lista desplegable de actividades. | Obligatorio al ingresar empresa. |
| **Fecha Actividad Económica** | Fecha de inicio de actividad económica. Este campo es mostrado solo si la actividad económica tiene configurado que requiere fecha. | Obligatorio |
| **Puesto** | Puesto que ocupa dentro de la organización o dirección de la empresa. | Obligatorio al ingresar empresa. |

---

## ONG’s

Sección para agregar las empresas sin fines de lucro en las que la persona PEP posee alguna afiliación. 

![Sección ONGs](../assets/images/pep_empresas_ongs.png)

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Empresa** | Nombre de la empresa en donde la persona PEP posee afiliación. Al ingresar el nombre, el sistema sugiere el listado de empresas (persona jurídica) que ya están registradas en el sistema con ese nombre, para que pueda ser seleccionado, de lo contrario se puede crear una nueva. | Opcional. |
| **Tipo de Documento** | Tipo de documento con el que se identifica la empresa. El campo muestra una lista desplegable de tipos de documento. | Obligatorio al ingresar empresa. |
| **Identificación** | Número con el que se identifica la empresa, relacionado al tipo de documento seleccionado. | Obligatorio al ingresar empresa. |
| **Fecha Inicial** | Fecha a partir de la cual ocupa el puesto en la empresa. | Obligatorio al ingresar empresa. |
| **Fecha Final** | Fecha de finalización del puesto en la empresa. | Opcional |
| **Actividad Económica** | Actividad económica a la que se dedica la empresa. El campo muestra una lista desplegable de actividades. | Obligatorio al ingresar empresa. |
| **Fecha Actividad Económica** | Fecha de inicio de actividad económica. Este campo es mostrado solo si la actividad económica tiene configurado que requiere fecha. | Obligatorio |
| **Puesto** | Puesto que ocupa dentro de la organización o dirección de la empresa. | Obligatorio al ingresar empresa. |

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