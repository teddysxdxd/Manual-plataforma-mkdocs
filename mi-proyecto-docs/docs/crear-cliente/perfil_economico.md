---
title: Perfil Económico - Persona Jurídica
hide:
  - toc
  - nav
---
# Perfil Económico - Persona Jurídica

Registro de los datos que permite clasificar a la persona jurídica con un perfil económico. El ingreso de datos en esta sección es obligatorio para continuar con el flujo de creación de cliente.

El perfil económico de una persona jurídica está dividido en cuatro secciones, información general y financiera, información de donde opera la institución, relaciones con grupos económicos o financieros y registro de proveedores principales.

### Información General y Financiera – Perfil Económico

La información general corresponde a los datos que permiten identificar el perfil económico general de la persona jurídica.

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Afecto ISR** | Indica si la persona es afecta a ISR, el sistema valida que tenga ingresado el documento de identificación. Si no es afecto a ISR será requerida una autorización. | Obligatorio |
| **Actividad Económica** | Actividad económica a la que se dedica la persona jurídica. | Obligatorio |
| **Fecha Actividad Económica** | Fecha de inicio de la actividad económica. Se muestra solo cuando la actividad económica tiene configurado que requiere fecha. | Obligatorio |
| **Sector Económico** | Sector económico al que pertenece la persona jurídica. | Obligatorio |
| **Clase de Cliente** | Clase de cliente con el que es clasificada la persona jurídica. | Obligatorio |

La sección de información financiera corresponde al total de activos y ventas anuales que percibe la institución. Es obligatorio el ingreso de un registro en la moneda local para continuar con el flujo. (Siguiente)

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Moneda** | Indica la moneda en la que están expresados los valores | Obligatorio |
| **Monto Aproximado de Total de Activos** | Valor del total de activos expresados en la moneda seleccionada. | Obligatorio |
| **Nivel de Ventas Anuales** | Valor de ventas anuales en la moneda seleccionada. | Obligatorio |
| **Observaciones** | Observaciones relacionadas a la información financiera. | Opcional |

![Perfil Económico](../assets/images/20250901-185321.png)

### Información Donde Opera

Registro de los países o distribución geográfica local en donde tiene operaciones la institución, el registro de datos es opcional, se puede continuar con el flujo sin ingresar estos datos. (Siguiente)

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **País** | Indica el país en donde tiene operaciones. | Obligatorio |
| **Región** | Región del país local en donde tiene operaciones. Este campo se habilita cuando el país es local. | Opcional |
| **Departamento** | Departamento del país local en donde tiene operaciones. | Opcional |
| **Municipio** | Municipio del país local en donde tiene operaciones. | Opcional |

![Información de Operación](../assets/images/20250901-185509.png)

### Relaciones Grupos Económicos / Financieros

Registro del grupo económico y/o financiero con los que tiene relación la institución, el registro de datos es opcional, se puede continuar con el flujo sin ingresar estos datos. (Siguiente)

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Relación con Grupo Económico** | Grupo económico con el que tiene relación la institución. | Opcional |
| **Relación con Grupo Financiero** | Grupo financiero con el que tiene relación la institución. | Opcional |

![Relaciones de Grupo](../assets/images/20250901-185612.png)

### Principales Proveedores

Registro de los principales proveedores de la institución, el registro de datos es obligatorio, no se puede continuar con el flujo sin agregar proveedores. (Finalizar)

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Proveedor** | Proveedor con el que tiene relación la institución. Al ingresar el nombre del proveedor el sistema realiza una búsqueda de las personas existentes y muestra una lista seleccionable de las personas que coinciden con el texto. | Obligatorio |

![Principales Proveedores](../assets/images/20250901-185718.png)

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