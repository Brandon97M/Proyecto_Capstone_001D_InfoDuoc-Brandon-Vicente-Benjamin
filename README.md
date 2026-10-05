### Instrucciones para ejecutar el proyecto localmente
Para levantar el entorno de desarrollo web en tu máquina, sigue estos pasos:
1. Clona este repositorio en tu equipo local:
   `git clone https://github.com/TuUsuario/InfoDuoc-SanJoaquin.git`
2. Abre la terminal y navega hasta la carpeta del proyecto:
   `cd InfoDuoc-SanJoaquin`
3. Instala las dependencias necesarias de Node.js:
   `npm install`
4. Ejecuta el servidor de desarrollo local:
   `npm run dev`
5. Abre tu navegador web e ingresa a la dirección indicada en la terminal (por defecto `http://localhost:5173`) para ver el kiosco en funcionamiento.

### Metodología de trabajo del equipo
El equipo gestiona el ciclo de vida del proyecto utilizando el marco de trabajo ágil **Scrum**. El desarrollo se estructura en iteraciones (Sprints) enfocadas en entregar valor funcional y visual para el kiosco interactivo. Se aplican prácticas de Agile Coaching para mantener una comunicación fluida entre las áreas de Frontend, Backend y QA, priorizando la adaptabilidad y la mejora continua ante los nuevos requerimientos del entorno web.

### Arquitectura de la solución
El sistema está diseñado bajo una arquitectura de Aplicación Web de Página Única (SPA) estrictamente orientada a pantallas y tótems interactivos web.
* **Capa de Presentación (Frontend):** Interfaz gráfica desarrollada con React y estilizada con Tailwind CSS. El enrutamiento de las vistas (Mapa, Directorio) se gestiona de forma nativa en el navegador mediante TanStack Router para evitar recargas de página y entregar una experiencia táctil fluida.
* **Capa de Lógica y Datos (Backend):** Servidor construido sobre Node.js y Express que gestiona las peticiones de datos de las escuelas y la información espacial del mapa. La persistencia de datos se maneja mediante un motor de base de datos relacional (PostgreSQL / MySQL).
* **Infraestructura:** El empaquetamiento y despliegue de los servicios web se orquesta a través de contenedores con Docker y Docker Compose, asegurando alta disponibilidad en el entorno de la sede.
