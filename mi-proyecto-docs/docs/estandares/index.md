---
title: Estándares
description: Estándares de navegación y uso de la aplicación - Base conocimiento QA
hide:
  - navigation
  - toc
---

# Estándares

En esta sección se describe de forma general los estándares que son utilizados en la navegación de la aplicación.

<style>
/* ========== ESTILOS PARA ESTÁNDARES ========== */
:root {
  --primary-blue: #2d5490;
  --primary-dark-blue: #1e3a6a;
  --secondary-blue: #4a6fa5;
  --light-blue: #e8eff7;
  --light-green: #e8f7ef;
  --light-red: #f7e8e8;
  --text-dark: #333333;
  --text-light: #666666;
  --white: #ffffff;
  --shadow-light: rgba(0, 0, 0, 0.1);
  --shadow-medium: rgba(0, 0, 0, 0.15);
  --border-color: #ddd;
}

.standard-section {
  margin: 40px 0;
  padding: 30px;
  background: var(--white);
  border-radius: 15px;
  box-shadow: 0 5px 20px var(--shadow-light);
  border-left: 5px solid var(--primary-blue);
  position: relative;
}

.standard-section h2 {
  color: var(--primary-blue);
  border-bottom: 2px solid var(--light-blue);
  padding-bottom: 10px;
  margin-top: 0;
}

.image-container {
  text-align: center;
  margin: 30px 0;
  padding: 20px;
  background: var(--light-blue);
  border-radius: 10px;
}

.image-container img {
  max-width: 100%;
  height: auto;
  border-radius: 8px;
  box-shadow: 0 4px 12px var(--shadow-medium);
  border: 1px solid var(--border-color);
}

.image-caption {
  font-style: italic;
  color: var(--text-light);
  margin-top: 10px;
  font-size: 0.9em;
}

.standard-table {
  width: 100%;
  border-collapse: collapse;
  margin: 25px 0;
  font-size: 0.9em;
  border-radius: 10px;
  overflow: hidden;
  box-shadow: 0 0 20px var(--shadow-light);
}

.standard-table thead tr {
  background: linear-gradient(135deg, var(--primary-blue), var(--secondary-blue));
  color: var(--white);
  text-align: left;
  font-weight: bold;
}

.standard-table th,
.standard-table td {
  padding: 15px 20px;
  border: 1px solid var(--border-color);
}

.standard-table tbody tr {
  border-bottom: 1px solid var(--border-color);
}

.standard-table tbody tr:nth-of-type(even) {
  background-color: var(--light-blue);
}

.standard-table tbody tr:last-of-type {
  border-bottom: 2px solid var(--primary-blue);
}

.standard-table tbody tr:hover {
  background-color: rgba(74, 111, 165, 0.1);
  transform: translateX(5px);
  transition: all 0.3s ease;
}

.table-icon {
  width: 30px;
  height: 30px;
  vertical-align: middle;
  margin-right: 10px;
  border-radius: 5px;
  padding: 3px;
  background: var(--white);
  border: 1px solid var(--border-color);
}

.info-box {
  padding: 20px;
  background: linear-gradient(135deg, var(--light-blue), var(--white));
  border-radius: 10px;
  border-left: 4px solid var(--primary-blue);
  margin: 25px 0;
  box-shadow: 0 4px 12px var(--shadow-light);
}

.info-box.warning {
  background: linear-gradient(135deg, #fff3cd, #ffffff);
  border-left-color: #ffc107;
}

.info-box.danger {
  background: linear-gradient(135deg, #f8d7da, #ffffff);
  border-left-color: #dc3545;
}

.info-box.success {
  background: linear-gradient(135deg, #d4edda, #ffffff);
  border-left-color: #28a745;
}

.steps-container {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin: 30px 0;
  justify-content: center;
}

.step-item {
  flex: 0 0 calc(50% - 20px);
  background: var(--white);
  padding: 25px;
  border-radius: 12px;
  box-shadow: 0 5px 15px var(--shadow-light);
  border: 2px solid transparent;
  transition: all 0.3s ease;
  position: relative;
}

.step-item:hover {
  border-color: var(--primary-blue);
  transform: translateY(-5px);
  box-shadow: 0 10px 25px var(--shadow-medium);
}

.step-item::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 5px;
  height: 100%;
  background: linear-gradient(to bottom, var(--primary-blue), var(--secondary-blue));
  border-radius: 5px 0 0 5px;
}

.navigation-buttons {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 40px 0;
  padding: 25px;
  background: linear-gradient(135deg, var(--white), var(--light-blue));
  border-radius: 15px;
  box-shadow: 0 5px 20px var(--shadow-light);
}

.nav-button {
  display: inline-flex;
  align-items: center;
  padding: 12px 30px;
  background: linear-gradient(135deg, var(--primary-blue), var(--primary-dark-blue));
  color: var(--white);
  text-decoration: none;
  border-radius: 50px;
  font-weight: 600;
  font-size: 1.1em;
  transition: all 0.3s ease;
  box-shadow: 0 4px 15px rgba(45, 84, 144, 0.3);
}

.nav-button:hover {
  transform: translateY(-3px);
  box-shadow: 0 8px 25px rgba(45, 84, 144, 0.4);
  color: var(--white);
}

.nav-button.prev::before {
  content: '←';
  margin-right: 10px;
}

.nav-button.next::after {
  content: '→';
  margin-left: 10px;
}

.back-to-main {
  text-align: center;
  margin: 50px 0 30px 0;
}

.back-to-main .nav-button {
  background: linear-gradient(135deg, var(--secondary-blue), var(--primary-blue));
  font-size: 1.2em;
  padding: 15px 40px;
}

/* ========== RESPONSIVE ========== */
@media (max-width: 768px) {
  .standard-section {
    padding: 20px;
    margin: 25px 0;
  }
  
  .step-item {
    flex: 0 0 100%;
  }
  
  .standard-table {
    display: block;
    overflow-x: auto;
  }
  
  .navigation-buttons {
    flex-direction: column;
    gap: 20px;
  }
  
  .nav-button {
    width: 100%;
    justify-content: center;
  }
}

@media (max-width: 480px) {
  .standard-section {
    padding: 15px;
  }
  
  .standard-table th,
  .standard-table td {
    padding: 10px 15px;
    font-size: 0.85em;
  }
  
  .image-container {
    padding: 15px;
  }
}
</style>

## Pantalla de Acceso

Para ingresar a la aplicación, es requerido el ingreso de credenciales que permiten identificar el usuario y los permisos que este tiene para realizar operaciones en el sistema. El acceso se administra por medio de la aplicación Keycloak, que se encarga de capturar y enviar las credenciales a los servicios de seguridad establecidos, para que sean validadas y determinar si puede ingresar a la aplicación, así como las opciones a las que tiene acceso.

<div class="image-container">
![Pantalla de Login](assets/images/estandares/login.png)
<div class="image-caption">Pantalla de acceso al sistema mediante Keycloak</div>
</div>

## Pantalla de Inicio

Después de ingresar los datos de credenciales para tener acceso a la aplicación, se muestra la pantalla de inicio o principal del sistema.

En la parte superior la pantalla dispone de algunas opciones de acceso rápido que se mantienen siempre visibles en la navegación de la aplicación.

<table class="standard-table">
<thead>
<tr>
<th>Opción</th>
<th>Descripción</th>
<th>Icono</th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Notificaciones</strong></td>
<td>Indica las notificaciones pendientes de leer.</td>
<td><img src="assets/images/estandares/estandares_icono_1.png" class="table-icon" alt="Notificaciones"></td>
</tr>
<tr>
<td><strong>Autorizaciones</strong></td>
<td>Muestra el portal de autorizaciones del usuario.</td>
<td><img src="assets/images/estandares/estandares_icono_2.png" class="table-icon" alt="Autorizaciones"></td>
</tr>
<tr>
<td><strong>Usuario</strong></td>
<td>Usuario con el que se ingresó a la aplicación.</td>
<td>—</td>
</tr>
<tr>
<td><strong>Tema e Idioma</strong></td>
<td>Permite seleccionar el tema e idioma a utilizar.</td>
<td><img src="assets/images/estandares/estandares_icono_3.png" class="table-icon" alt="Tema e Idioma"></td>
</tr>
<tr>
<td><strong>Salir</strong></td>
<td>Salir del sistema.</td>
<td><img src="assets/images/estandares/estandares_icono_4.png" class="table-icon" alt="Salir"></td>
</tr>
</tbody>
</table>

<div class="image-container">
![Pantalla de Inicio](assets/images/estandares/estandares_pantalla_de_inicio_2.png)
<div class="image-caption">Interfaz principal de la plataforma</div>
</div>

El menú de opciones está ubicado al lado izquierdo de la pantalla de inicio de la aplicación, si las opciones principales tienen más opciones, se puede expandir al seleccionar cada opción o se pueden contraer al seleccionar nuevamente la opción.

<div class="image-container">
![Menú Lateral](assets/images/estandares/estandares_pantalla_de_inicio2.png)
<div class="image-caption">Menú lateral expandible de la aplicación</div>
</div>

## Formularios

La aplicación dispone de diferentes tipos de formulario para realizar operaciones con los datos, manteniendo estándares que permitan al usuario navegar de forma fácil.

En los formularios se incluyen campos de texto libre, listas seleccionables, campos tipo fecha, campo de chequeo o verificación y en el caso de los registros, se dispone de botones de acciones para agregar, consultar, modificar o eliminar registros. No todos los formularios permiten todas las acciones, esto depende de los requerimientos establecidos para operar los registros en cada opción.

<div class="image-container">
![Formularios](assets/images/estandares/estandares_formularios.png)
<div class="image-caption">Ejemplo de formulario con diferentes tipos de campos</div>
</div>

En algunas opciones como el flujo de creación de clientes, se dividen en varios pasos, pero algunos pasos tienen inmersos varios pasos que pueden ser obligatorios de completar para continuar con los pasos del flujo general.

<div class="image-container">
![Pasos del Flujo](assets/images/estandares/estandares_pasos.png)
<div class="image-caption">Flujo de pasos para creación de clientes</div>
</div>

### Navegación

<div class="info-box">
En los pasos de cada flujo se puede utilizar el botón para regresar (Anterior), en el caso que el usuario necesite regresar a cambiar algún dato de la información que ingresó en los pasos anteriores, una vez realizado el cambio de datos, debe continuar con el botón Siguiente. Se debe considerar que los datos principales como documentos de identificación, nombres y apellidos, género o tipo de persona, no podrán ser modificados, una vez se haya pasado al siguiente paso.
</div>

<div class="image-container">
![Navegación entre pasos](assets/images/estandares/pasted_20250826-224544.png)
<div class="image-caption">Navegación entre pasos del formulario</div>
</div>

<div class="steps-container">
<div class="step-item">
<h4>Validación de Campos</h4>
<p>Los botones no siempre se muestran habilitados, esto debido a que es necesario completar la información obligatoria.</p>
</div>

<div class="step-item">
<h4>Restricciones de Navegación</h4>
<p>En el primer paso, no se habilita el botón Anterior y en el último paso que corresponde a Finalizar, no se habilita el botón Anterior.</p>
</div>
</div>

## Mensajes Informativos

En esta sección se indican algunos mensajes generales que la aplicación puede mostrar.

### Tiempo Espera Terminado

Este mensaje se muestra cuando los servicios principales no responden al ejecutar una operación y no permite continuar.

<div class="image-container">
![Tiempo de Espera](assets/images/estandares/estandares_tiempo_de_espera.png)
<div class="image-caption">Mensaje de tiempo de espera agotado</div>
</div>

#### No se pudo procesar la solicitud

<div class="info-box warning">
Este mensaje se presenta principalmente porque no hay comunicación al servidor, puede ser por problemas de red o porque el servidor no está disponible.
</div>

<div class="image-container">
![Error de Conexión](assets/images/estandares/estandares_ha_ocurrido_un_error.png)
<div class="image-caption">Mensaje de error de conexión con el servidor</div>
</div>

#### Listas de Cautela

<div class="info-box">
El sistema realiza validaciones en listas de cautela utilizando el documento de identificación y/o el nombre de la persona, dependiendo del tipo de lista en que sea encontrada la persona, puede ser solo un mensaje informativo o puede requerir credenciales para autorizar la continuidad del flujo o detener la operación y no permitir continuar con el flujo. Se debe considerar que la validación de lista de cautela se hace solo cuando se dispone de un documento de identificación de la persona.
</div>

<div class="image-container">
![Lista de Cautela](assets/images/estandares/persona_lista_de_cautela.png)
<div class="image-caption">Alerta de validación en listas de cautela</div>
</div>

<div class="back-to-main">
<a href="../" class="nav-button">← Volver a Menú Plataforma</a>
</div>

<script>
// Añadir funcionalidad interactiva a las tablas
document.addEventListener('DOMContentLoaded', function() {
    // Efecto hover para filas de tabla
    const tableRows = document.querySelectorAll('.standard-table tbody tr');
    tableRows.forEach(row => {
        row.addEventListener('mouseenter', function() {
            this.style.backgroundColor = 'rgba(74, 111, 165, 0.1)';
            this.style.transform = 'translateX(5px)';
        });
        
        row.addEventListener('mouseleave', function() {
            this.style.backgroundColor = '';
            this.style.transform = '';
        });
    });
    
    // Efecto para cajas de información
    const infoBoxes = document.querySelectorAll('.info-box');
    infoBoxes.forEach(box => {
        box.addEventListener('click', function() {
            this.style.transform = 'scale(1.02)';
            setTimeout(() => {
                this.style.transform = '';
            }, 300);
        });
    });
    
    // Smooth scroll para enlaces internos
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
        anchor.addEventListener('click', function(e) {
            e.preventDefault();
            const targetId = this.getAttribute('href');
            if (targetId !== '#') {
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            }
        });
    });
});
</script>