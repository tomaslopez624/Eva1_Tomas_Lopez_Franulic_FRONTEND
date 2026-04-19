# Eva1_Tomas_Lopez_Franulic_FRONTEND
Prueba 1 Frontend

A continuación redacto brevemente en HTML semántico partes del codigo del Mockup propuesto en la prueba

//Lo siguiente es solo para la barra superior

<header>
  <a href="/" class="logo">TechConsulting</a> <nav>
    <ul>
      <li><a href="#home">Home</a></li> <li><a href="#servicios">Nuestros Servicios</a></li>
      <li><a href="#nosotros">Nosotros</a></li>
      <li><a href="#contacto">Contáctenos</a></li>
    </ul>
  </nav>
  <button id="theme-toggle"> <span class="icon">৫</span>   //Día&Noche
  </button>
</header>

//Home

<main>
  <section id="home">
    <h1>Soluciones Digitales para tu Empresa</h1> <p>
      Consultoría y desarrollo de software especializado en transformar tu
      negocio mediante soluciones tecnológicas innovadoras e integrales. </p>
    <div class="actions">
      <a href="#servicios" class="btn-primary">Descubre Nuestros Servicios</a> <a href="#contacto" class="btn-secondary">Contáctanos</a> </div>
  </section>

//Servicios
  
  <section id="servicios">
    <h2>Nuestros Servicios</h2> <p>Ofrecemos soluciones integrales de tecnología...</p> <div class="services-grid">
      <article class="service-card">
        <div class="icon">🧠</div> <h3>Consultoría Digital</h3>
        <p>Asesoramiento estratégico para optimizar tus procesos empresariales...</p> </article>

      </div>
  </section>

//Nosotros
  <section id="nosotros">
    <h2>Nosotros</h2> <p>Somos una empresa de consultoría y desarrollo de software...</p> <div class="mission-vision">
      <article>
        <h3>Nuestra Misión</h3> <p>Empoderar a las empresas mediante soluciones tecnológicas...</p> </article>
      <article>
        <h3>Nuestra Visión</h3> <p>Ser el socio tecnológico de referencia en la región...</p> </article>
    </div>
  </section>

//Formulario de contacto
<section id="contacto">
    <h2>Contáctenos</h2> <p>¿Listo para transformar tu empresa? Hablemos de tu proyecto.</p> <form id="contact-form">
      <div class="form-group">
        <label for="nombre">Nombre completo</label> <input type="text" id="nombre" name="nombre" required>
      </div>

      <div class="form-group">
        <label for="email">Email</label> <input type="email" id="email" name="email" required>
      </div>

      <div class="form-group">
        <label for="servicio">Seleccione un servicio</label>
        <select id="servicio" name="servicio">
          <option value="consultoria">Consultoría Digital</option>
          <option value="multiexperiencia">Soluciones Multiexperiencia</option>
          </select>
      </div>

      <div class="form-group">
        <label for="mensaje">Mensaje</label>
        <textarea id="mensaje" name="mensaje" required></textarea>
      </div>

      <button type="submit">Enviar mensaje</button>
    </form>

    <div class="contact-info">
      <p>Email: <strong>contacto@techconsulting.com</strong></p> <p>Teléfono: <strong>+52 (55) 1234-5678</strong></p> </div>
  </section>
</main>

//JS

Podemos activar el boton de NocheDia de la siguiente manera

const botonTema = document.getElementById('theme-toggle'); // theme-toggle es el cambiador de tema
botonTema.addEventListener('click', () => {
    // Efectos de presionar el botón
});

//Finalmente se cambia el BODY completo
document.body.classList.toggle('dark-mode');


