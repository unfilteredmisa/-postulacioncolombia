<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Colombia al Consejo de Seguridad</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header class="header">
    <h1 class="title">🇨🇴 Colombia al Consejo de Seguridad</h1>
    <p class="subtitle">Una voz por la paz, el multilateralismo y la democracia en el mundo</p>
  </header>

  <section class="section candidature" id="candidature">
    <h2>🌍 Postulación Oficial</h2>
    <p>Colombia se postula como miembro del Consejo de Seguridad de las Naciones Unidas, impulsando una agenda basada en la diplomacia activa, la prevención de conflictos, la protección de los derechos humanos y la promoción del desarrollo sostenible. Con un firme compromiso con el multilateralismo, Colombia busca ser un actor clave en la construcción de consensos y soluciones duraderas a los desafíos globales.</p>
  </section>

  <section class="section why" id="why">
    <h2>🤝 ¿Por qué Colombia?</h2>
    <ul>
      <li>✔️ Experiencia en construcción de paz y justicia transicional</li>
      <li>✔️ Liderazgo regional y compromiso con el derecho internacional</li>
      <li>✔️ Política exterior centrada en la vida, la equidad y la sostenibilidad</li>
      <li>✔️ Participación activa en organismos multilaterales</li>
    </ul>
    <p>Colombia está lista para aportar su voz, experiencia y liderazgo, representando con dignidad los intereses de América Latina y del mundo en favor de la paz y la seguridad internacional.</p>
  </section>



  <footer class="footer">
    <p>© 2025 Colombia al Consejo de Seguridad | Candidatura oficial | Diplomacia para la vida</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
    font-family: 'Segoe UI', sans-serif;
  }
  
  body {
    background: linear-gradient(to right, #ffd700, #0033a0, #ce1126);
    color: #fff;
  }
  
  .header {
    padding: 3rem;
    text-align: center;
    background-color: rgba(0, 0, 0, 0.3);
    animation: fadeIn 2s ease-in;
  }
  
  .title {
    font-size: 3rem;
    font-weight: bold;
  }
  
  .subtitle {
    font-size: 1.5rem;
    margin-top: 1rem;
  }
  
  .section {
    padding: 3rem 2rem;
    animation: slideUp 1.5s ease forwards;
    opacity: 0;
    transform: translateY(40px);
  }
  
  .candidature, .why, .gallery {
    background-color: rgba(0, 0, 0, 0.2);
    margin: 1rem 0;
    border-radius: 1rem;
  }
  
  .why ul {
    list-style: none;
    padding: 0;
    margin-top: 1rem;
  }
  
  .why li {
    background: rgba(255, 255, 255, 0.1);
    margin-bottom: 0.5rem;
    padding: 0.5rem 1rem;
    border-radius: 8px;
  }
  
  .gallery .images {
    display: flex;
    gap: 1rem;
    justify-content: center;
    flex-wrap: wrap;
    margin-top: 1rem;
  }
  
  .gallery img {
    width: 200px;
    height: auto;
    border-radius: 10px;
    transition: transform 0.3s ease;
  }
  
  .gallery img:hover {
    transform: scale(1.1);
  }
  
  .footer {
    text-align: center;
    padding: 1rem;
    background-color: rgba(0, 0, 0, 0.3);
  }
  
  /* Animaciones */
  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(-20px); }
    to { opacity: 1; transform: translateY(0); }
  }
  
  @keyframes slideUp {
    from { opacity: 0; transform: translateY(40px); }
    to { opacity: 1; transform: translateY(0); }
  }

  document.addEventListener('DOMContentLoaded', () => {
    const sections = document.querySelectorAll('.section');
  
    const revealOnScroll = () => {
      sections.forEach(section => {
        const sectionTop = section.getBoundingClientRect().top;
        if (sectionTop < window.innerHeight - 100) {
          section.style.opacity = 1;
          section.style.transform = 'translateY(0)';
        }
      });
    };
  
    window.addEventListener('scroll', revealOnScroll);
    revealOnScroll(); // Ejecuta al cargar para mostrar la primera sección
  });
  
