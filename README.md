<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Portafolio Artístico</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            margin: 0;
            height: 100vh;
        }
        #sidebar {
            width: 20%;
            background-color: #f4f4f4;
            padding: 10px;
            box-shadow: 2px 0 5px rgba(0,0,0,0.1);
        }
        #content {
            width: 80%;
            padding: 20px;
            overflow-y: auto;
        }
        h1 {
            font-size: 1.5em;
        }
        ul {
            list-style-type: none;
            padding: 0;
        }
        li {
            margin: 10px 0;
            cursor: pointer;
        }
        li:hover {
            text-decoration: underline;
        }
        .gallery {
            display: none;
        }
        .gallery.active {
            display: block;
        }
        .gallery img {
            width: 30%;
            margin: 5px;
        }
        .gallery video {
            width: 100%;
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <div id="sidebar">
        <h1>Proyectos</h1>
        <ul>
            <li onclick="showGallery('project1')">Proyecto 1</li>
            <li onclick="showGallery('project2')">Proyecto 2</li>
            <li onclick="showGallery('project3')">Proyecto 3</li>
        </ul>
    </div>
    <div id="content">
        <div id="project1" class="gallery">
            <h2>Proyecto 1</h2>
            <img src="img1.jpg" alt="Imagen 1">
            <img src="img2.jpg" alt="Imagen 2">
            <img src="img3.jpg" alt="Imagen 3">
            <img src="img4.jpg" alt="Imagen 4">
            <img src="img5.jpg" alt="Imagen 5">
            <img src="img6.jpg" alt="Imagen 6">
            <img src="img7.jpg" alt="Imagen 7">
            <img src="img8.jpg" alt="Imagen 8">
            <img src="img9.jpg" alt="Imagen 9">
            <img src="img10.jpg" alt="Imagen 10">
            <video controls>
                <source src="video1.mp4" type="video/mp4">
                Tu navegador no soporta la etiqueta de video.
            </video>
        </div>
        <div id="project2" class="gallery">
            <h2>Proyecto 2</h2>
            <img src="img1.jpg" alt="Imagen 1">
            <img src="img2.jpg" alt="Imagen 2">
            <img src="img3.jpg" alt="Imagen 3">
            <img src="img4.jpg" alt="Imagen 4">
            <img src="img5.jpg" alt="Imagen 5">
            <img src="img6.jpg" alt="Imagen 6">
            <img src="img7.jpg" alt="Imagen 7">
            <img src="img8.jpg" alt="Imagen 8">
            <img src="img9.jpg" alt="Imagen 9">
            <img src="img10.jpg" alt="Imagen 10">
            <video controls>
                <source src="video2.mp4" type="video/mp4">
                Tu navegador no soporta la etiqueta de video.
            </video>
        </div>
        <div id="project3" class="gallery">
            <h2>Proyecto 3</h2>
            <img src="img1.jpg" alt="Imagen 1">
            <img src="img2.jpg" alt="Imagen 2">
            <img src="img3.jpg" alt="Imagen 3">
            <img src="img4.jpg" alt="Imagen 4">
            <img src="img5.jpg" alt="Imagen 5">
            <img src="img6.jpg" alt="Imagen 6">
            <img src="img7.jpg" alt="Imagen 7">
            <img src="img8.jpg" alt="Imagen 8">
            <img src="img9.jpg" alt="Imagen 9">
            <img src="img10.jpg" alt="Imagen 10">
            <video controls>
                <source src="video3.mp4" type="video/mp4">
                Tu navegador no soporta la etiqueta de video.
            </video>
        </div>
    </div>
    <script>
        function showGallery(id) {
            const galleries = document.querySelectorAll('.gallery');
            galleries.forEach(gallery => {
                gallery.classList.remove('active');
            });
            document.getElementById(id).classList.add('active');
        }
    </script>
</body>
</html>
