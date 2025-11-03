AppSalon - Sistema de Gestión para Salones de Belleza
https://img.shields.io/badge/AppSalon-SPA-orange?style=for-the-badge&logo=appveyor
https://img.shields.io/badge/PHP-8.0+-purple?style=for-the-badge&logo=php
https://img.shields.io/badge/MySQL-Database-blue?style=for-the-badge&logo=mysql

📖 Descripción
AppSalon es un sistema web completo desarrollado para la gestión de salones de belleza y barberías. Permite a los administradores gestionar citas, servicios, clientes y empleados de manera eficiente, mientras que los clientes pueden reservar citas fácilmente a través de una interfaz intuitiva.

✨ Características Principales
🗓️ Gestión de Citas
Sistema de reservas en tiempo real
Calendario interactivo
Recordatorios automáticos
Gestión de horarios y disponibilidad

💇 Servicios y Productos
Catálogo completo de servicios
Gestión de precios y duraciones
Inventario de productos
Categorización de servicios

👥 Gestión de Clientes
Base de datos de clientes
Historial de servicios
Preferencias y notas personalizadas
Sistema de fidelización

🧑‍💼 Panel de Administración
Dashboard con métricas clave
Gestión de empleados
Reportes y estadísticas
Configuración del sistema

🛠️ Tecnologías Utilizadas
Backend
PHP - Lenguaje de programación principal
MySQL - Base de datos relacional
MVC - Arquitectura del proyecto
REST API - Para comunicación frontend-backend

Frontend
HTML5 - Estructura semántica
CSS3 - Estilos y diseño responsive
JavaScript - Interactividad del lado del cliente
SASS - Preprocesador CSS
Herramientas de Desarrollo
Composer - Gestión de dependencias PHP
Gulp - Automatización de tareas
Git - Control de versiones

🚀 Instalación y Configuración
Prerrequisitos
PHP 8.0 o superior
MySQL 5.7 o superior
Servidor web (Apache/Nginx)
Composer

Pasos de Instalación
Clonar el repositorio
bash
git clone https://github.com/FranciscoGG09/AppSalon.git
cd AppSalon
Instalar dependencias PHP
bash
composer install
Configurar base de datos

Crear una base de datos MySQL
Importar el archivo database/schema.sql
Configurar credenciales en config/database.php
Configurar variables de entorno

bash
cp .env.example .env
# Editar el archivo .env con tus configuraciones
Configurar el servidor web
Apuntar el document root a la carpeta public/
Configurar rewrite rules para URLs amigables
Ejecutar el servidor de desarrollo

bash
php -S localhost:8000 -t public
📁 Estructura del Proyecto
text
AppSalon/
├── app/
│   ├── Controllers/
│   ├── Models/
│   ├── Views/
│   └── Core/
├── config/
├── public/
│   ├── assets/
│   │   ├── css/
│   │   ├── js/
│   │   └── images/
│   └── index.php
├── database/
├── vendor/
└── README.md
🎯 Uso del Sistema
Para Administradores
Iniciar sesión en el panel de administración

Gestionar servicios y empleados
Ver reportes y estadísticas
Configurar horarios y disponibilidad

Para Clientes
Registrarse en la plataforma
Explorar servicios disponibles
Reservar citas en línea
Gestionar su perfil e historial

🤝 Contribución
¡Las contribuciones son bienvenidas! Para contribuir al proyecto:
Haz un fork del repositorio
Crea una rama para tu feature (git checkout -b feature/AmazingFeature)
Commit tus cambios (git commit -m 'Add some AmazingFeature')
Push a la rama (git push origin feature/AmazingFeature)
Abre un Pull Request

👨‍💻 Desarrollador
FranciscoGG09 - GitHub
