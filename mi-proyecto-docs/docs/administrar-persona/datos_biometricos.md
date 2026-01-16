---
title: Datos Biométricos
hide:
  - toc
  - nav
---

# Datos Biométricos

Permite gestionar los datos biométricos de una persona, permitiendo capturar las huellas en forma digital. Esta sección depende de los parámetros recuperados del core, en donde se indica si es permitido realizar la captura de huellas (capturaHuella). Esta opción esta disponible solo para personas naturales.

Dependiendo de la configuración de parámetros para captura de huella en el core, será necesario la captura de determinados dedos tanto de la mano derecha como la izquierda.

**Requerimientos**

* Dispositivo de lector de huella instalado con sus drivers correspondientes.
* Agente de captura de huella (applet)

---

## Agregar Huella

![Estado inicial sin huella](../assets/images/20251120-184959.png)

Cuando las huellas no han sido capturadas, se muestra al imagen de huella en rojo con el texto “Sin Huella” y un texto informativo en el tab de Datos Biométricos “Datos Biométricos sin registrar ”. Para realizar la captura de huellas se debe utilizar el botón “Capturar Huella”.

![Proceso de captura](../assets/images/20251120-190917.png)

Al seleccionar “Capturar Huella” se activa el applet mostrando una pequeña ventana con la imagen de las manos, resaltando de color verde los dedos a los cuales corresponden las huellas que serán capturadas y un contador numeral de las veces que debe ser capturada la huella de cada dedo (1 2 3 4). 

En el campo “Status” se debe mostrar el texto “Lector Conectado…” el cual indica que el applet a detectado el dispositivo para capturar las huellas.

![Applet de captura](../assets/images/20251215-204625.png)

Al capturar cada huella de forma satisfactoria, en el campo “Status” será mostrado el texto “Huella capturada correctamente…” y al finalizar de capturar la huellas requeridas, se muestra el texto “Captura Finalizada correctamente”, se debe utilizar el botón Guardar para almacenar las huellas capturadas.

![Captura finalizada](../assets/images/20251215-211439.png)

---

## Huella Registrada / Actualizar Huella

Cuando las huellas ya han sido capturadas, se muestra la imagen de huella en verde con el texto “Tiene Huella”.

![Estado con huella registrada](../assets/images/20251215-211704.png)

Si fuera necesario cambiar o volver a capturar las huellas de una persona, se puede utilizar el botón “Actualizar Huella”. Para realizar la actualización de huellas, es mostrado el dialogo de autorizaciones, para que sea realizada la operación es necesario ingresar de forma local las credenciales del usuario que tiene permisos o hacer la solicitud de forma remota. Después que sea autorizado, se muestra la ventana pequeña del applet para captura de huellas, como se hace al agregar huellas.

![Autorización para actualización](../assets/images/20251215-212301.png)

---

### Mensajes de error

| Mensaje | Descripción |
| :--- | :--- |
| **Timeout - No se registro en lector** | Cuando el applet de captura de huella no esta listo para capturar huellas. |
| **Huella digital cancelada** | Cuando en la captura de huellas se utiliza el botón “Cancelar” |

[← Volver a página anterior](administrar-persona.md)

<style>
  /* Estilos específicos para Datos Biométricos */
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
  
  .md-typeset p {
    line-height: 1.6;
    text-align: justify;
    margin-bottom: 1.2em;
  }
</style>