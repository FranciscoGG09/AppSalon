# AppSalon 💈

<p align="center">
  <img src="https://img.shields.io/badge/Estado-Terminado-brightgreen" alt="Estado del Proyecto">
  <img src="https://img.shields.io/badge/PHP-777BB4?style=flat&logo=php&logoColor=white" alt="PHP">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/Sass-CC6699?style=flat&logo=sass&logoColor=white" alt="Sass">
  <img src="https://img.shields.io/badge/SQL-4479A1?style=flat&logo=mysql&logoColor=white" alt="SQL">
</p>

Aplicación web completa para la gestión de citas en un salón de belleza o barbería. Este proyecto implementa un sistema robusto que permite a los clientes registrarse, iniciar sesión y agendar servicios, mientras que un panel de administrador permite gestionar las citas y servicios ofrecidos.

## 📋 Características Principales

Este proyecto se divide en dos áreas principales:

### Área de Cliente (Frontend)
* **Login y Creación de Cuentas:** Sistema de autenticación seguro con validación de formularios.
* **Visualización de Servicios:** Los clientes pueden ver todos los servicios disponibles (cortes, tintes, etc.) con sus precios.
* **Sistema de Reservas:** Un flujo de usuario intuitivo para seleccionar servicios, elegir una fecha y hora, y confirmar una cita.
* **Resumen de Cita:** El usuario ve un resumen de su cita antes de confirmarla.
* **Perfil de Usuario:** (Opcional) Área donde el cliente puede ver su historial de citas.

### Área de Administración (Backend/Admin)
* **Dashboard de Citas:** Un panel donde el administrador puede ver todas las citas agendadas, filtradas por fecha.
* **Gestión de Citas:** El administrador puede confirmar o eliminar citas.
* **Gestión de Servicios:** Un CRUD completo (Crear, Leer, Actualizar, Eliminar) para que el administrador pueda añadir nuevos servicios o modificar los existentes.
* **Seguridad:** El panel de administración está protegido y solo es accesible para usuarios con permisos de administrador.

## 🛠️ Stack Tecnológico

Este proyecto fue construido utilizando una arquitectura **Modelo-Vista-Controlador (MVC)** para separar la lógica de negocio de la presentación.

* **Backend:** **PHP 8**
* **Frontend:** **HTML5**, **SASS** (compilado con Gulp) y **JavaScript (Vanilla)**
* **Base de Datos:** **MySQL / PostgreSQL** (SQL)
* **Arquitectura:** Modelo-Vista-Controlador (MVC)
* **Dependencias PHP:** **Composer**
* **Automatización:** **Gulp** para compilar SASS y minificar JavaScript en tiempo real.
* **Hosting/Deploy:** (Opcional: menciona dónde lo desplegaste, ej: Heroku, Railway, Hostinger)

## 🔧 Instalación y Puesta en Marcha

Si deseas ejecutar este proyecto en tu entorno local, sigue estos pasos:

1.  **Clonar el repositorio:**
    ```bash
    git clone [https://github.com/FranciscoGG09/AppSalon.git](https://github.com/FranciscoGG09/AppSalon.git)
    cd AppSalon
    ```

2.  **Instalar dependencias de PHP:**
    ```bash
    composer install
    ```

3.  **Instalar dependencias de Frontend (Node.js):**
    ```bash
    npm install
    ```

4.  **Configurar la Base de Datos:**
    * Importa el archivo `.sql` (que deberías incluir en tu repo) a tu gestor de base de datos (MySQL Workbench, pgAdmin, etc.).
    * Crea un archivo `.env` (basado en el `.env.example` si tienes uno) y añade tus credenciales de la base de datos.
    ```env
    DB_HOST=localhost
    DB_USER=root
    DB_PASS=[TU_CONTRASEÑA]
    DB_NAME=appsalon_db
    ```

5.  **Compilar los assets (SASS y JS):**
    ```bash
    gulp
    ```
    *O, para modo desarrollo (observa cambios):*
    ```bash
    gulp dev
    ```

6.  **Iniciar el servidor:**
    * Inicia tu servidor local (XAMPP, WAMP, MAMP) o usa el servidor integrado de PHP:
    ```bash
    php -S localhost:8000 -t public
    ```

7.  Abre `http://localhost:8000` en tu navegador.

## 👨‍💻 Autor

Desarrollado por **Francisco González**.

* **LinkedIn:** [linkedin.com/in/francisco-gonzalez](https://linkedin.com/in/francisco-gonzalez)
* **GitHub:** [@FranciscoGG09](https://github.com/FranciscoGG09)
