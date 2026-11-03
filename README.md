# Restaurante Boyacense

Sitio web de un restaurante de **comida típica boyacense** hecho en **PHP y MySQL** siguiendo el patrón **MVC** (modelo, vista y controlador). Incluye página de inicio, menú de platos y un módulo de **gestión de clientes**.

## Funcionalidades

- Página de inicio con la presentación y la filosofía del restaurante.
- Menú con platos típicos (arepa boyacense, cocido boyacense, entre otros).
- Registro de clientes: **crear, listar, modificar y eliminar** (nombre, apellido, teléfono, ciudad y correo).
- Listado de clientes con paginación.
- Limpieza de entradas con `htmlspecialchars`.

## Tecnologías

- **PHP** (programación orientada a objetos, patrón MVC)
- **MySQL / MariaDB** con `mysqli`
- HTML y CSS

## Estructura

```
Guia20Ramon/
├── index.php              # Página de inicio
├── modelo/
│   ├── conexion.php       # Conexión a MySQL
│   └── Clientes.php       # Clase con insertar, modificar, eliminar y listar
├── controlador/
│   └── controladorCliente.php
├── vista/                 # Menú, formulario y listado de clientes
├── estilos2/  estilos.css/
├── img/
└── cliente.sql            # Estructura de la base de datos
```

## Cómo ejecutarlo

1. Instalar **XAMPP** (Apache + MySQL).
2. Copiar la carpeta del proyecto en `htdocs` con el nombre `guia20Ramon` (las rutas del menú usan `/guia20Ramon/...`).
3. En phpMyAdmin, crear la base de datos `restaurante` e importar `cliente.sql`.
4. Abrir http://localhost/guia20Ramon/

## Capturas

| Inicio | Menú | Registro de clientes | Listado |
|---|---|---|---|
| ![Inicio](docs/inicio.png) | ![Menú](docs/menu.png) | ![Registro](docs/registro.png) | ![Listado](docs/listado.png) |

> Pendiente: agregar capturas en `docs/`.

## Mejoras planeadas

- Usar consultas preparadas (`mysqli_prepare`) en `Clientes.php` para evitar inyección SQL.
- Dejar en `cliente.sql` solo la estructura de la tabla, sin datos personales.
- Comprimir las imágenes (`arepaboyacense.png` pesa 14,7 MB) y agregar `img/pasta.jpg`, que falta.
- Igualar mayúsculas y minúsculas de los enlaces con los nombres reales de los archivos, para que funcione en servidores Linux.
- Renombrar la carpeta `Guia20Ramon` y `estilos.css/` a nombres más claros.

## Autora

**Diana Alejandra Mancipe Jiménez** · [LinkedIn](https://www.linkedin.com/in/diana-alejandra-mancipe-jimenez-737669334/) · mancipealejandra63@gmail.com

---

