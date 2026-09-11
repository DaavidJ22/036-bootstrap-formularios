# 036 Bootstrap Formularios

Proyecto desarrollado con Python, Flask, Jinja2 y Bootstrap para practicar rutas, formularios, métodos GET y POST, herencia de plantillas y componentes responsivos.

## Funcionalidades

El proyecto incluye:

- Página de inicio
- Registro de clientes
- Registro de proveedores
- Inicio de sesión
- Plantilla base reutilizable con Jinja2
- Formularios procesados mediante POST
- Confirmaciones usando render_template
- Bootstrap integrado por CDN
- Diseño responsivo

## Estructura del proyecto

```text
036-bootstrap-formularios/
│
├── app.py
├── README.md
│
├── templates/
│   ├── base.html
│   ├── inicio.html
│   ├── clientes.html
│   ├── clientes_confirmacion.html
│   ├── proveedores.html
│   ├── proveedores_confirmacion.html
│   ├── login.html
│   └── login_resultado.html
│
└── static/
    └── estilos.css
    ## Rutas del proyecto

- `/` - Página de inicio
- `/clientes` - Registro de clientes
- `/proveedores` - Registro de proveedores
- `/login` - Inicio de sesión

## Credenciales de prueba

Para probar el login:

Usuario: admin  
Contraseña: 1234

## Funcionamiento de los formularios

Los formularios utilizan los métodos GET y POST.

Los datos enviados se procesan mediante `request.form` y luego se muestran en páginas de confirmación usando `render_template`.

Los datos no se guardan en una base de datos ni en archivos.

## Bootstrap

Bootstrap se integra mediante CDN en la plantilla `base.html`.

Se utilizan componentes como:

- Navbar
- Cards
- Formularios
- Botones
- Alertas
- Tablas
- Sistema de rejilla responsiva

## Bonus

Se agregó un modal de Bootstrap en el formulario de clientes.

El modal solicita confirmación antes de enviar el formulario.

## Modo de desarrollo

Durante el desarrollo se utiliza:

```python
app.run(debug=True)