<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mis Proyectos</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f9f9f9;
      margin: 0;
      padding: 0;
    }
    header {
      background-color: #333;
      color: white;
      padding: 1rem;
      text-align: center;
    }
    section {
      max-width: 800px;
      margin: 2rem auto;
      padding: 1rem;
    }
    .proyecto {
      background: white;
      border-radius: 8px;
      padding: 1rem;
      margin-bottom: 1rem;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    }
    footer {
      background-color: #333;
      color: white;
      text-align: center;
      padding: 1rem;
      position: fixed;
      bottom: 0;
      width: 100%;
    }
    nav {
      text-align: center;
      margin-top: 1rem;
    }
    nav a {
      margin: 0 1rem;
      color: #333;
      text-decoration: none;
    }
    nav a:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body>
  <header>
    <h1>Mis Proyectos</h1>
    <nav>
      <a href="#proyectos">Proyectos</a>
      <a href="#sobre-mi">Sobre mí</a>
      <a href="#contacto">Contacto</a>
    </nav>
  </header>

  <section id="proyectos">
    <h2>Lista de Proyectos</h2>
    <div id="lista-proyectos"></div>
  </section>

  <section id="sobre-mi">
    <h2>Sobre mí</h2>
    <p>Soy un entusiasta de la tecnología, desarrollador de proyectos relacionados con CNC, impresión 3D, y automatización mediante inteligencia artificial. Me apasiona construir cosas útiles y aprender constantemente.</p>
  </section>

  <section id="contacto">
    <h2>Contacto</h2>
    <p>Puedes encontrarme en:</p>
    <ul>
      <li>Email: tuskarch94@gmail.com</li>
      <li><a href="https://github.com/Tuskarch94" target="_blank">GitHub</a></li>
      <li><a href="https://linkedin.com/in/tuskarch94" target="_blank">LinkedIn</a></li>
    </ul>
  </section>

  <footer>
    <p>&copy; 2025 Tuskarch94. Todos los derechos reservados.</p>
  </footer>

  <script>
    const proyectos = [
      { nombre: "CNC Homemade", descripcion: "Proyecto de máquina CNC casera con control GRBL y Mach3." },
      { nombre: "Recicladora PET", descripcion: "Sistema para reciclar PET y fabricar filamento 3D." },
      { nombre: "Controlador AI", descripcion: "IA para controlar hardware de impresión 3D y CNC." }
    ];

    const contenedor = document.getElementById('lista-proyectos');
    proyectos.forEach(p => {
      const div = document.createElement('div');
      div.className = 'proyecto';
      div.innerHTML = `<h3>${p.nombre}</h3><p>${p.descripcion}</p>`;
      contenedor.appendChild(div);
    });
  </script>
</body>
</html>
