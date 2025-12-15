# Lufkebike

Lufkebike es una plataforma de e-commerce especializada en la venta de bicicletas, desarrollada con Django. Ofrece un catálogo completo de bicicletas, sistema de carrito de compras, reseñas de usuarios, gestión de eventos y un panel de administración para gestionar el inventario.

## Características

- **Catálogo de Bicicletas**: Explora una amplia variedad de bicicletas por marca, modelo, tipo y precio.
- **Carrito de Compras**: Agrega productos al carrito, gestiona cantidades y realiza pedidos.
- **Sistema de Reseñas**: Los usuarios pueden dejar reseñas y calificaciones en las bicicletas.
- **Gestión de Eventos**: Inscríbete y administra eventos relacionados con ciclismo.
- **Autenticación de Usuarios**: Registro, login y perfiles de usuario.
- **Panel de Administración**: Interfaz para gestionar bicicletas, órdenes, clientes y eventos.
- **Interfaz Responsiva**: Diseño moderno y profesional con Bootstrap.

## Tecnologías Utilizadas

- **Backend**: Django 5.2.7
- **Base de Datos**: MySQL
- **Frontend**: HTML5, CSS3, Bootstrap 5.3.2
- **Lenguaje**: Python 3.13
- **Servidor**: Gunicorn (producción), WhiteNoise (estáticos)
- **Otros**: Pillow (imágenes), MySQLClient

## Requisitos Previos

- Python 3.8 o superior
- MySQL Server instalado y en ejecución
- Git

## Instalación

1. **Clona el repositorio**:
   ```bash
   git clone https://github.com/tu-usuario/lufkebike.git
   cd lufkebike
   ```

2. **Crea un entorno virtual**:
   ```bash
   python -m venv .venv
   ```

3. **Activa el entorno virtual**:
   - En Windows:
     ```bash
     .\.venv\Scripts\activate
     ```
   - En macOS/Linux:
     ```bash
     source .venv/bin/activate
     ```

4. **Instala las dependencias**:
   ```bash
   pip install -r requirements.txt
   ```

5. **Configura la base de datos**:
   - Crea una base de datos en MySQL:
     ```sql
     CREATE DATABASE Lufkebike;
     ```
   - Edita `Lufkebike/settings.py` con tus credenciales de MySQL.

6. **Aplica las migraciones**:
   ```bash
   python manage.py migrate
   ```

7. **Crea un superusuario**:
   ```bash
   python manage.py createsuperuser
   ```

8. **Ejecuta el servidor**:
   ```bash
   python manage.py runserver
   ```

9. **Accede a la aplicación**:
   - Sitio web: http://127.0.0.1:8000/
   - Panel de administración: http://127.0.0.1:8000/admin/

## Uso

### Para Usuarios
- Regístrate o inicia sesión.
- Explora el catálogo de bicicletas.
- Agrega productos al carrito.
- Deja reseñas en las bicicletas.
- Inscríbete en eventos.

### Para Administradores
- Accede al panel de admin para gestionar:
  - Bicicletas (agregar, editar, eliminar).
  - Órdenes y clientes.
  - Eventos.

## Estructura del Proyecto

```
lufkebike/
├── manage.py
├── Lufkebike/              # Configuración del proyecto
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   └── asgi.py
├── app_bicicletas/         # App de bicicletas
├── app_carrito/            # App de carrito de compras
├── app_clientes/           # App de autenticación y perfiles
├── app_eventos/            # App de eventos
├── app_ordenes/            # App de órdenes
├── app_resenas/            # App de reseñas
├── templates/              # Plantillas HTML
├── static/                 # Archivos estáticos
├── media/                  # Archivos multimedia
├── logs/                   # Logs de la aplicación
└── requirements.txt
```

## Contribución

1. Haz un fork del proyecto.
2. Crea una rama para tu feature (`git checkout -b feature/nueva-funcionalidad`).
3. Commit tus cambios (`git commit -am 'Agrega nueva funcionalidad'`).
4. Push a la rama (`git push origin feature/nueva-funcionalidad`).
5. Abre un Pull Request.

## Licencia

Este proyecto es de código abierto y está disponible bajo la Licencia MIT.

## Autor

Desarrollado como parte del curso de Talento Digital - Módulo 8. Omar Sepúlveda

## Contacto

Si tienes preguntas o sugerencias, abre un issue en GitHub.