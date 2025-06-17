<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Veterinaria Mi Mascota</title>
  <style>
    :root {
      --primary: #4caf50;
      --secondary: #ffffff;
      --background: #f9f9f9;
      --dark: #333;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', sans-serif;
    }

    body {
      background-color: var(--background);
      color: var(--dark);
    }

    header {
      background-color: var(--primary);
      color: var(--secondary);
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
    }

    header h1 {
      font-size: 1.8rem;
    }

    nav ul {
      list-style: none;
      display: flex;
      gap: 1rem;
    }

    nav a {
      color: var(--secondary);
      text-decoration: none;
      font-weight: bold;
    }

    .hero {
      background: url('https://images.unsplash.com/photo-1558788353-f76d92427f16') no-repeat center/cover;
      color: white;
      text-align: center;
      padding: 4rem 2rem;
    }

    .hero h2 {
      font-size: 2.5rem;
    }

    .section {
      padding: 3rem 2rem;
    }

    .section.light {
      background-color: #e8f5e9;
    }

    .cards {
      display: flex;
      flex-wrap: wrap;
      gap: 1.5rem;
      justify-content: center;
    }

    .card {
      background: white;
      border-radius: 8px;
      padding: 1.5rem;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
      flex: 1 1 250px;
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 1rem;
      max-width: 400px;
      margin: auto;
    }

    form input,
    form textarea {
      padding: 0.8rem;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    form button {
      background-color: var(--primary);
      color: white;
      border: none;
      padding: 1rem;
      border-radius: 5px;
      cursor: pointer;
    }

    form button:hover {
      background-color: #388e3c;
    }

    footer {
      background-color: var(--primary);
      color: var(--secondary);
      text-align: center;
      padding: 1rem;
      margin-top: 2rem;
    }
  </style>
</head>
<body>
  <header>
    <h1>Veterinaria Mi Mascota</h1>
    <nav>
      <ul>
        <li><a href="#servicios">Servicios</a></li>
        <li><a href="#nosotros">Nosotros</a></li>
        <li><a href="#contacto">Contacto</a></li>
      </ul>
    </nav>
  </header>

  <section class="hero">
    <h2>¡Cuidamos a tu mejor amigo!</h2>
    <p>Atención profesional y cariñosa para tu mascota.</p>
  </section>

  <section id="servicios" class="section">
    <h2>Servicios</h2>
    <div class="cards">
      <div class="card">
        <h3>Consultas</h3>
        <p>Revisión general, diagnósticos y tratamientos.</p>
      </div>
      <div class="card">
        <h3>Vacunas</h3>
        <p>Protégete y protege a tu mascota con nuestras vacunas.</p>
      </div>
      <div class="card">
        <h3>Estética</h3>
        <p>Baños, cortes y limpieza para que luzca genial.</p>
      </div>
    </div>
  </section>

  <section id="nosotros" class="section light">
    <h2>Sobre Nosotros</h2>
    <p>Somos una clínica con más de 10 años de experiencia cuidando a los animales con amor y profesionalismo.</p>
  </section>

  <section id="contacto" class="section">
    <h2>Contacto</h2>
    <form id="formularioContacto">
      <input type="text" placeholder="Nombre" required />
      <input type="email" placeholder="Correo electrónico" required />
      <textarea placeholder="Tu mensaje" required></textarea>
      <button type="submit">Enviar</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 Veterinaria Mi Mascota</p>
  </footer>

  <script>
    document.getElementById('formularioContacto').addEventListener('submit', function (e) {
      e.preventDefault();
      alert('Gracias por contactarnos. Te responderemos pronto.');
      this.reset();
    });
  </script>
</body>
</html>
