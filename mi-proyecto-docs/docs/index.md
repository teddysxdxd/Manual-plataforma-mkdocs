---
title: Plataforma – Base conocimiento QA
hide:
  - navigation
  - toc
---

<style>
/* Container for the grid of features */
.features-grid {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
  padding: 20px;
  max-width: 1200px;
  margin: 0 auto;
}

/* Styling for each individual feature item */
.feature-item {
  flex: 0 0 calc(33.33% - 40px);
  max-width: 300px;
  position: relative;
  overflow: hidden;
  background-color: #fff;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  padding-bottom: 15px;
  transition: transform 0.3s ease;
  text-align: center;
  cursor: pointer;
  border: 1px solid #e0e0e0;
}

/* Scale up item slightly on hover */
.feature-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
}

/* Adjust z-index of figure to be above other content within the item */
.feature-item figure {
  position: relative;
  z-index: 1;
  margin: 0;
  padding: 15px 10px 10px 10px;
}

/* Styling for the image within the item */
.feature-item img {
  display: block;
  width: 120px;
  height: auto;
  margin: 15px auto 10px auto;
  border-radius: 5px;
}

/* Styling for the image caption */
.feature-item figcaption {
  font-size: 1.1em;
  color: #333;
  padding: 0 10px;
  font-weight: 500;
}

/* Styling for the overlay */
.overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background-color: rgba(0, 30, 118, 0.8);
  overflow: hidden;
  width: 100%;
  height: 0;
  transition: height 0.5s ease;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 0 0 10px 10px;
  z-index: 2;
}

/* Expand the overlay to full height on hover */
.feature-item:hover .overlay {
  height: 100%;
}

/* Styling for the text inside the overlay */
.overlay-text {
  color: white;
  font-size: 1.1em;
  text-align: center;
  padding: 20px;
  white-space: normal;
  font-weight: bold;
}

/* Header styling */
.header-title {
  text-align: center;
  margin: 30px 0;
  padding: 0 20px;
}

.header-title h1 {
  font-size: 2.5em;
  color: #2d5490;
  margin-bottom: 10px;
}

.header-title p {
  color: #666;
  font-size: 1.1em;
  max-width: 800px;
  margin: 0 auto;
}

/* Logo section */
.logo-section {
  text-align: center;
  margin: 20px 0 40px 0;
}

.logo-section img {
  max-width: 250px;
  height: auto;
}

/* Back link */
.back-link {
  text-align: center;
  margin: 40px 0;
  padding: 20px;
}

.back-link a {
  display: inline-block;
  padding: 10px 20px;
  background-color: #2d5490;
  color: white;
  text-decoration: none;
  border-radius: 5px;
  transition: background-color 0.3s ease;
}

.back-link a:hover {
  background-color: #1e3a6a;
}

/* Responsive Adjustments */
@media (max-width: 768px) {
  .feature-item {
    flex: 0 0 calc(50% - 40px);
  }
  
  .header-title h1 {
    font-size: 2em;
  }
}

@media (max-width: 480px) {
  .feature-item {
    flex: 0 0 calc(100% - 40px);
  }
  
  .header-title h1 {
    font-size: 1.8em;
  }
}
</style>

<div class="logo-section">
![plataforma](assets/images/titulo-plataforma.png)
</div>

<div class="header-title">
<h1>Base conocimiento QA</h1>
<p>Documentación completa de la plataforma para el equipo de Quality Assurance</p>
</div>

<div class="features-grid">

<div class="feature-item" onclick="window.location.href='estandares/'">
  <figure>
    <img src="assets/images/plataforma_estandar.png" alt="Icono para Estandares">
    <figcaption>Estándares</figcaption>
  </figure>
  <div class="overlay">
    <div class="overlay-text">Guías y estándares de calidad para el desarrollo y testing</div>
  </div>
</div>

<div class="feature-item" onclick="window.location.href='configuraciones/'">
  <figure>
    <img src="assets/images/plataforma_configuraciones.png" alt="Icono para Configuraciones">
    <figcaption>Configuraciones</figcaption>
  </figure>
  <div class="overlay">
    <div class="overlay-text">Configuración del sistema y parámetros de la plataforma</div>
  </div>
</div>

<div class="feature-item" onclick="window.location.href='autorizaciones/'">
  <figure>
    <img src="assets/images/plataforma_autorizaciones.png" alt="Icono para Autorizaciones">
    <figcaption>Autorizaciones</figcaption>
  </figure>
  <div class="overlay">
    <div class="overlay-text">Sistema de permisos y autorizaciones de usuarios</div>
  </div>
</div>

<div class="feature-item" onclick="window.location.href='busqueda-clientes/busqueda-clientes/'">
  <figure>
    <img src="assets/images/buscar_cliente-platatorma4.png" alt="Icono para Búsqueda de Cliente">
    <figcaption>Búsqueda de Cliente</figcaption>
  </figure>
  <div class="overlay">
    <div class="overlay-text">Procedimientos para búsqueda y consulta de clientes</div>
  </div>
</div>

<div class="feature-item" onclick="window.location.href='crear-cliente/crear-cliente/'">
  <figure>
    <img src="assets/images/crear_cliente-platatorma5.png" alt="Icono para Crear Cliente">
    <figcaption>Crear Cliente</figcaption>
  </figure>
  <div class="overlay">
    <div class="overlay-text">Flujos para creación de nuevos clientes en el sistema</div>
  </div>
</div>

<div class="feature-item" onclick="window.location.href='administrar-persona/'">
  <figure>
    <img src="assets/images/administrar_persona.png" alt="Icono para Administrar Persona">
    <figcaption>Administrar Persona</figcaption>
  </figure>
  <div class="overlay">
    <div class="overlay-text">Gestión de información personal en la plataforma</div>
  </div>
</div>

</div>

<div class="back-link">
<a href="#" onclick="history.back(); return false;">← Volver a Página Anterior</a>
</div>

<script>
// Añadir funcionalidad de clic a todos los feature items
document.querySelectorAll('.feature-item').forEach(item => {
  item.style.cursor = 'pointer';
  item.addEventListener('click', function(e) {
    if (!e.target.closest('a')) {
      const link = this.getAttribute('onclick');
      if (link) {
        const url = link.match(/window\.location\.href='([^']+)'/)[1];
        window.location.href = url;
      }
    }
  });
});
</script>