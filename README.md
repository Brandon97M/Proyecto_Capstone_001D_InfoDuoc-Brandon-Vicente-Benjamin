# Sistema Kiosco Interactivo (InfoDuoc UC San Joaquín)

### Descripción
* **Qué hace:** Aplicación web optimizada para tótem táctil que integra un mapa isométrico interactivo de 8 pisos y un directorio institucional dinámico.
* **A quién va dirigido:** Alumnos de primer año, docentes nuevos, visitas y la comunidad académica en general de Duoc UC Sede San Joaquín.
* **Qué problema resuelve:** Elimina la desorientación espacial al ubicar salas, laboratorios y servicios dentro del edificio, y agiliza el acceso a la información de contacto de las distintas escuelas y áreas administrativas.

### Tecnologías Utilizadas
* **Frontend:** React, TanStack Router (Navegación SPA), Tailwind CSS.
* **Backend:** Node.js, Express.
* **Base de Datos:** PostgreSQL / MySQL.
* **Cloud / Infraestructura:** Docker, Docker Compose.

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

### Integrantes del equipo con sus roles
* **Vicente Salinas:** Lead Backend / DevOps, Data Modeling & Agile Coach.
* **Benjamín Nuñez:** Lead Frontend / UI/UX & Map Graphics Specialist.
* **Brandon Monsalve:** Full-Stack Developer / QA & Service Integration.

### Metodología de trabajo del equipo
El equipo gestiona el ciclo de vida del proyecto utilizando el marco de trabajo ágil **Scrum**. El desarrollo se estructura en iteraciones (Sprints) enfocadas en entregar valor funcional y visual continuo para el kiosco interactivo. Se aplican activamente prácticas de Agile Coaching para mantener una comunicación fluida entre las áreas de Frontend, Backend y Calidad (QA), priorizando la adaptabilidad y la mejora continua ante los requerimientos web del cliente (Sede San Joaquín).

### Arquitectura de la solución
El sistema está diseñado bajo una arquitectura de Aplicación Web de Página Única (SPA) estrictamente orientada a pantallas y tótems interactivos web.
* **Capa de Presentación (Frontend):** Interfaz gráfica desarrollada en React y estilizada con Tailwind CSS. El enrutamiento de las vistas (Mapa, Directorio) se gestiona de forma nativa en el navegador mediante TanStack Router para evitar recargas de página y entregar una experiencia táctil fluida.
* **Capa de Lógica y Datos (Backend):** Servidor construido sobre Node.js y Express que gestiona las peticiones de datos de las escuelas y la información espacial del mapa. La persistencia de datos se maneja mediante un motor de base de datos relacional.
* **Infraestructura:** El empaquetamiento y despliegue de los servicios web se orquesta a través de contenedores con Docker, asegurando alta disponibilidad e independencia del entorno para su ejecución en la sede.
