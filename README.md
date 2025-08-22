<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>AgroFichas System</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background: #f9f9f9;
      color: #333;
    }
    header {
      background: linear-gradient(90deg, #2e7d32, #4caf50);
      color: white;
      padding: 15px;
      text-align: center;
    }
    header h1 {
      margin: 0;
      font-size: 1.5em;
    }
    nav {
      margin-top: 10px;
    }
    nav a {
      color: white;
      margin: 0 10px;
      text-decoration: none;
      font-weight: bold;
    }
    .container {
      max-width: 1000px;
      margin: auto;
      padding: 20px;
    }
    .card {
      background: white;
      border-radius: 10px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      padding: 20px;
      margin-bottom: 20px;
    }
    .search-box input {
      width: 80%;
      padding: 10px;
      border-radius: 6px;
      border: 1px solid #ccc;
    }
    .search-box button {
      padding: 10px 15px;
      border: none;
      border-radius: 6px;
      background: #4caf50;
      color: white;
      cursor: pointer;
    }
    .filters button {
      margin: 5px;
      padding: 8px 12px;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      font-weight: bold;
    }
    .filters .herbicidas { background: #66bb6a; color: white; }
    .filters .fungicidas { background: #42a5f5; color: white; }
    .filters .insecticidas { background: #ef5350; color: white; }
    .filters .fertilizantes { background: #ffca28; color: white; }
    table {
      width: 100%;
      border-collapse: collapse;
    }
    table th, table td {
      padding: 10px;
      border: 1px solid #ddd;
      text-align: left;
    }
    table th {
      background: #f1f1f1;
    }
    .btn-agregar {
      background: #4caf50;
      color: white;
      padding: 10px 15px;
      border: none;
      border-radius: 6px;
      margin-bottom: 10px;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <header>
    <h1>🌱 AgroFichas System</h1>
    <nav>
      <a href="#">Búsqueda Rápida</a>
      <a href="#">Catálogo</a>
      <a href="#">Compartir</a>
    </nav>
  </header>

  <div class="container">
    <!-- Búsqueda Rápida -->
    <div class="card">
      <h2>Búsqueda Rápida</h2>
      <div class="search-box">
        <input type="text" placeholder="Buscar productos agroquímicos...">
        <button>🔍</button>
      </div>
      <div class="filters">
        <button class="herbicidas">Herbicidas</button>
        <button class="fungicidas">Fungicidas</button>
        <button class="insecticidas">Insecticidas</button>
        <button class="fertilizantes">Fertilizantes</button>
      </div>
    </div>

    <!-- Catálogo de Productos -->
    <div class="card">
      <h2>Catálogo de Productos</h2>
      <button class="btn-agregar">+ Agregar Producto</button>
      <table>
        <thead>
          <tr>
            <th>Ingrediente Activo</th>
            <th>Tipo de Agroquímico</th>
            <th>PDF</th>
            <th>Acciones</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>Glifosato</td>
            <td>Herbicida</td>
            <td><a href="#">Ver PDF</a></td>
            <td><button>Editar</button> <button>Eliminar</button></td>
          </tr>
          <tr>
            <td>Imidacloprid</td>
            <td>Insecticida</td>
            <td><a href="#">Ver PDF</a></td>
            <td><button>Editar</button> <button>Eliminar</button></td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</body>
</html>
