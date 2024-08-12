Menú Web para KAIZEN - BAR
Descripción
Este proyecto es una aplicación web para un bar local llamada KAIZEN - BAR. La aplicación presenta un menú digital moderno con un diseño estético rústico y tradicional, utilizando una paleta de colores en tonos de marrón y beige.

Estructura del Proyecto
El proyecto consta de dos archivos principales para esta etapa:

index.html: Contiene la estructura HTML de la página de inicio.
styles.css: Contiene los estilos CSS aplicados a la página.
Diseño
Paleta de Colores
Beige Claro: #F5F5DC (Fondo del cuerpo)
Marrón Oscuro: #4E342E (Texto y elementos importantes)
Marrón Medio: #8D6E63 (Enlaces y botones)
Blanco Suave: #FFFDE7 (Texto principal en la sección hero)
Sección Principal
Fondo: Imagen de madera (/images/5.jpg), con un background-size de cover para asegurar que la imagen cubra toda la sección.
Texto:
Título: KAIZEN - BAR con sombra de texto para resaltar en diversos colores de fondo.
Descripción: Texto adicional con una sombra sutil para mejorar la legibilidad.
Estilos Aplicados
HTML

html
Copiar código
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menú Web - Inicio</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>

    <!-- Navbar -->
    <nav class="navbar navbar-expand-lg navbar-light bg-transparent">
        <div class="container-fluid">
            <a class="navbar-brand" href="#"><strong>KAIZEN - BAR</strong></a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link active" aria-current="page" href="#">Inicio</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Menú</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Contacto</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Main Section -->
    <section class="hero-section d-flex justify-content-center align-items-center">
        <div class="text-center">
            <h1 class="display-4"><strong>KAIZEN - BAR</strong></h1>
            <p class="lead">Disfruta de nuestro nuevo menú digital</p>
            <a href="#" class="btn btn-primary btn-lg">Explorar Menú</a>
        </div>
    </section>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
CSS

css
Copiar código
body {
    font-family: 'Poppins', sans-serif;
    background-color: #F5F5DC; /* Beige Claro */
    color: #4E342E; /* Marrón Oscuro */
}

.navbar-brand {
    font-weight: 600;
    color: #4E342E !important; /* Marrón Oscuro */
}

.nav-link {
    color: #8D6E63 !important; /* Marrón Medio */
    transition: color 0.3s;
}

.nav-link:hover {
    color: #4E342E !important; /* Marrón Oscuro */
}

.hero-section {
    height: 100vh;
    background-image: url('/images/5.jpg'); 
    background-size: cover;
    background-position: center;
    text-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
    color: #FFFDE7; 
}

@keyframes fadeIn {
    0% {
        opacity: 0;
        transform: scale(0.8);
    }
    100% {
        opacity: 1;
        transform: scale(1);
    }
}

.hero-section h1 {
    font-size: 4rem;
    font-weight: 800;
    color: #e4d4ce; /* Blanco Suave */
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.6); /* Sombra del texto */
    padding: 10px 20px; /* Espaciado dentro del fondo */
    border-radius: 5px; /* Bordes redondeados */
    background-color: rgba(0, 0, 0, 0.3); /* Fondo semitransparente para el texto */
    animation: fadeIn 1.5s ease-in-out; /* Animación de entrada */
}

.hero-section .lead {
    color: #a37767; /* Marrón Medio */
    font-size: 1.2rem;
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.6); /* Sombra del texto */
    font-weight: 300;
    margin-bottom: 30px;
}

.btn-primary {
    background-color: #8D6E63; /* Marrón Medio */
    border-color: #8D6E63;
    transition: background-color 0.3s, border-color 0.3s;
}

.btn-primary:hover {
    background-color: #4E342E; /* Marrón Oscuro */
    border-color: #4E342E;
}
Funcionalidades Implementadas
Navbar: Navegación con enlaces a Inicio, Menú y Contacto.
Sección Principal: Texto de bienvenida con animación y sombra para mejorar la legibilidad en diferentes fondos.
Cómo Ejecutar
Instalar Dependencias: Asegúrate de tener una conexión a Internet para cargar Bootstrap desde CDN.
Estructura de Archivos: Guarda el archivo HTML en la raíz del proyecto y el CSS en una carpeta css.
Planes Futuros
Agregar más pantallas: Menú, Contacto, etc.
Mejorar la interactividad: Formularios de contacto, integración de Google Maps, etc