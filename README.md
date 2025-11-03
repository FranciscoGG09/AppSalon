<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AppSalon - Documentación</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        .readme-card {
            background: white;
            border-radius: 15px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            overflow: hidden;
            margin-bottom: 30px;
        }

        .header {
            background: linear-gradient(135deg, #2c3e50 0%, #3498db 100%);
            color: white;
            padding: 40px;
            text-align: center;
        }

        .badges {
            display: flex;
            justify-content: center;
            gap: 10px;
            flex-wrap: wrap;
            margin: 20px 0;
        }

        .badge {
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 0.9em;
            font-weight: bold;
        }

        .badge.php {
            background: #787CB5;
            color: white;
        }

        .badge.mysql {
            background: #00758F;
            color: white;
        }

        .badge.spa {
            background: #e67e22;
            color: white;
        }

        .section {
            padding: 30px;
            border-bottom: 1px solid #eee;
        }

        .section:last-child {
            border-bottom: none;
        }

        h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
        }

        h2 {
            color: #2c3e50;
            margin: 25px 0 15px 0;
            padding-bottom: 10px;
            border-bottom: 2px solid #3498db;
        }

        h3 {
            color: #34495e;
            margin: 20px 0 10px 0;
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }

        .feature-card {
            background: #f8f9fa;
            padding: 20px;
            border-radius: 10px;
            border-left: 4px solid #3498db;
            transition: transform 0.3s ease;
        }

        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
        }

        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            margin: 20px 0;
        }

        .tech-category {
            flex: 1;
            min-width: 250px;
            background: #f8f9fa;
            padding: 20px;
            border-radius: 10px;
        }

        .tech-category h4 {
            color: #2c3e50;
            margin-bottom: 15px;
            text-align: center;
        }

        .installation-steps {
            background: #f8f9fa;
            padding: 25px;
            border-radius: 10px;
            margin: 20px 0;
        }

        .step {
            margin: 15px 0;
            padding: 15px;
            background: white;
            border-radius: 8px;
            border-left: 4px solid #27ae60;
        }

        code {
            background: #2c3e50;
            color: #ecf0f1;
            padding: 2px 6px;
            border-radius: 4px;
            font-family: 'Courier New', monospace;
        }

        pre {
            background: #2c3e50;
            color: #ecf0f1;
            padding: 15px;
            border-radius: 8px;
            overflow-x: auto;
            margin: 15px 0;
        }

        .file-structure {
            background: #34495e;
            color: #ecf0f1;
            padding: 20px;
            border-radius: 8px;
            font-family: 'Courier New', monospace;
        }

        .file-item {
            margin: 5px 0;
            padding-left: 20px;
        }

        .folder {
            color: #3498db;
            font-weight: bold;
        }

        .file {
            color: #ecf0f1;
        }

        .contributor {
            display: flex;
            align-items: center;
            gap: 15px;
            margin: 20px 0;
            padding: 15px;
            background: #f8f9fa;
            border-radius: 10px;
        }

        .support-links {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }

        .support-link {
            padding: 10px 20px;
            background: #3498db;
            color: white;
            text-decoration: none;
            border-radius: 5px;
            transition: background 0.3s ease;
        }

        .support-link:hover {
            background: #2980b9;
        }

        @media (max-width: 768px) {
            .container {
                padding: 10px;
            }
            
            .header {
                padding: 20px;
            }
            
            h1 {
                font-size: 2em;
            }
            
            .section {
                padding: 20px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="readme-card">
            <div class="header">
                <h1>AppSalon</h1>
                <p>Sistema de Gestión para Salones de Belleza</p>
                <div class="badges">
                    <span class="badge spa">AppSalon SPA</span>
                    <span class="badge php">PHP 8.0+</span>
                    <span class="badge mysql">MySQL Database</span>
                </div>
            </div>

            <div class="section">
                <h2>📖 Descripción</h2>
                <p>AppSalon es un sistema web completo desarrollado para la gestión de salones de belleza y barberías. Permite a los administradores gestionar citas, servicios, clientes y empleados de manera eficiente, mientras que los clientes pueden reservar citas fácilmente a través de una interfaz intuitiva.</p>
            </div>

            <div class="section">
                <h2>✨ Características Principales</h2>
                <div class="features-grid">
                    <div class="feature-card">
                        <h3>🗓️ Gestión de Citas</h3>
                        <ul>
                            <li>Sistema de reservas en tiempo real</li>
                            <li>Calendario interactivo</li>
                            <li>Recordatorios automáticos</li>
                            <li>Gestión de horarios y disponibilidad</li>
                        </ul>
                    </div>
                    <div class="feature-card">
                        <h3>💇 Servicios y Productos</h3>
                        <ul>
                            <li>Catálogo completo de servicios</li>
                            <li>Gestión de precios y duraciones</li>
                            <li>Inventario de productos</li>
                            <li>Categorización de servicios</li>
                        </ul>
                    </div>
                    <div class="feature-card">
                        <h3>👥 Gestión de Clientes</h3>
                        <ul>
                            <li>Base de datos de clientes</li>
                            <li>Historial de servicios</li>
                            <li>Preferencias y notas personalizadas</li>
                            <li>Sistema de fidelización</li>
                        </ul>
                    </div>
                    <div class="feature-card">
                        <h3>🧑‍💼 Panel de Administración</h3>
                        <ul>
                            <li>Dashboard con métricas clave</li>
                            <li>Gestión de empleados</li>
                            <li>Reportes y estadísticas</li>
                            <li>Configuración del sistema</li>
                        </ul>
                    </div>
                </div>
            </div>

            <div class="section">
                <h2>🛠️ Tecnologías Utilizadas</h2>
                <div class="tech-stack">
                    <div class="tech-category">
                        <h4>Backend</h4>
                        <ul>
                            <li><strong>PHP</strong> - Lenguaje principal</li>
                            <li><strong>MySQL</strong> - Base de datos</li>
                            <li><strong>MVC</strong> - Arquitectura</li>
                            <li><strong>REST API</strong> - Comunicación</li>
                        </ul>
                    </div>
                    <div class="tech-category">
                        <h4>Frontend</h4>
                        <ul>
                            <li><strong>HTML5</strong> - Estructura</li>
                            <li><strong>CSS3</strong> - Estilos responsive</li>
                            <li><strong>JavaScript</strong> - Interactividad</li>
                            <li><strong>SASS</strong> - Preprocesador CSS</li>
                        </ul>
                    </div>
                    <div class="tech-category">
                        <h4>Herramientas</h4>
                        <ul>
                            <li><strong>Composer</strong> - Dependencias PHP</li>
                            <li><strong>Gulp</strong> - Automatización</li>
                            <li><strong>Git</strong> - Control de versiones</li>
                        </ul>
                    </div>
                </div>
            </div>

            <div class="section">
                <h2>🚀 Instalación y Configuración</h2>
                <div class="installation-steps">
                    <h3>Prerrequisitos</h3>
                    <ul>
                        <li>PHP 8.0 o superior</li>
                        <li>MySQL 5.7 o superior</li>
                        <li>Servidor web (Apache/Nginx)</li>
                        <li>Composer</li>
                    </ul>

                    <h3>Pasos de Instalación</h3>
                    <div class="step">
                        <strong>1. Clonar el repositorio</strong>
                        <pre><code>git clone https://github.com/FranciscoGG09/AppSalon.git
cd AppSalon</code></pre>
                    </div>
                    <div class="step">
                        <strong>2. Instalar dependencias PHP</strong>
                        <pre><code>composer install</code></pre>
                    </div>
                    <div class="step">
                        <strong>3. Configurar base de datos</strong>
                        <ul>
                            <li>Crear una base de datos MySQL</li>
                            <li>Importar el archivo <code>database/schema.sql</code></li>
                            <li>Configurar credenciales en <code>config/database.php</code></li>
                        </ul>
                    </div>
                    <div class="step">
                        <strong>4. Configurar variables de entorno</strong>
                        <pre><code>cp .env.example .env
# Editar el archivo .env con tus configuraciones</code></pre>
                    </div>
                    <div class="step">
                        <strong>5. Configurar servidor web</strong>
                        <ul>
                            <li>Apuntar el document root a la carpeta <code>public/</code></li>
                            <li>Configurar rewrite rules para URLs amigables</li>
                        </ul>
                    </div>
                    <div class="step">
                        <strong>6. Ejecutar servidor de desarrollo</strong>
                        <pre><code>php -S localhost:8000 -t public</code></pre>
                    </div>
                </div>
            </div>

            <div class="section">
                <h2>📁 Estructura del Proyecto</h2>
                <div class="file-structure">
                    <div class="file-item folder">AppSalon/</div>
                    <div class="file-item folder">├── app/</div>
                    <div class="file-item folder">│   ├── Controllers/</div>
                    <div class="file-item folder">│   ├── Models/</div>
                    <div class="file-item folder">│   ├── Views/</div>
                    <div class="file-item folder">│   └── Core/</div>
                    <div class="file-item folder">├── config/</div>
                    <div class="file-item folder">├── public/</div>
                    <div class="file-item folder">│   ├── assets/</div>
                    <div class="file-item folder">│   │   ├── css/</div>
                    <div class="file-item folder">│   │   ├── js/</div>
                    <div class="file-item folder">│   │   └── images/</div>
                    <div class="file-item file">│   └── index.php</div>
                    <div class="file-item folder">├── database/</div>
                    <div class="file-item folder">├── vendor/</div>
                    <div class="file-item file">└── README.md</div>
                </div>
            </div>

            <div class="section">
                <h2>🎯 Uso del Sistema</h2>
                <h3>Para Administradores</h3>
                <ol>
                    <li>Iniciar sesión en el panel de administración</li>
                    <li>Gestionar servicios y empleados</li>
                    <li>Ver reportes y estadísticas</li>
                    <li>Configurar horarios y disponibilidad</li>
                </ol>
                <h3>Para Clientes</h3>
                <ol>
                    <li>Registrarse en la plataforma</li>
                    <li>Explorar servicios disponibles</li>
                    <li>Reservar citas en línea</li>
                    <li>Gestionar su perfil e historial</li>
                </ol>
            </div>

            <div class="section">
                <h2>🤝 Contribución</h2>
                <p>¡Las contribuciones son bienvenidas! Para contribuir al proyecto:</p>
                <ol>
                    <li>Haz un fork del repositorio</li>
                    <li>Crea una rama para tu feature (<code>git checkout -b feature/AmazingFeature</code>)</li>
                    <li>Commit tus cambios (<code>git commit -m 'Add some AmazingFeature'</code>)</li>
                    <li>Push a la rama (<code>git push origin feature/AmazingFeature</code>)</li>
                    <li>Abre un Pull Request</li>
                </ol>
            </div>

            <div class="section">
                <h2>📝 Licencia</h2>
                <p>Este proyecto está bajo la Licencia MIT - ver el archivo <a href="LICENSE">LICENSE</a> para más detalles.</p>
            </div>

            <div class="section">
                <h2>👨‍💻 Desarrollador</h2>
                <div class="contributor">
                    <div>
                        <strong>FranciscoGG09</strong> - Desarrollador Principal
                    </div>
                    <a href="https://github.com/FranciscoGG09" class="support-link">GitHub</a>
                </div>
            </div>

            <div class="section">
                <h2>📞 Soporte</h2>
                <p>Si encuentras algún problema o tienes preguntas:</p>
                <div class="support-links">
                    <a href="https://github.com/FranciscoGG09/AppSalon/issues" class="support-link">Abrir Issue</a>
                    <a href="https://github.com/FranciscoGG09" class="support-link">Contactar Desarrollador</a>
                </div>
            </div>

            <div class="section" style="text-align: center; background: #f8f9fa;">
                <p><strong>⭐ ¡Dale una estrella al proyecto si te resulta útil!</strong></p>
            </div>
        </div>
    </div>
</body>
</html>
