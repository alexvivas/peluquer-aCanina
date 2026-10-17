# Pelucas Caninas

**Sitio web académico de servicios de estética canina y catálogo de productos para mascotas.**

Proyecto grupal desarrollado con **HTML5, CSS3 y JavaScript**, sin frameworks ni backend. Este repositorio conserva la estructura del trabajo original y documenta sus funcionalidades, límites y requisitos para ejecutarlo localmente.

> **Estado:** prototipo frontend. Las imágenes originales no estaban incluidas en el archivo recibido, por lo que algunas secciones se visualizan incompletas. No es un sistema de ventas ni de reclamaciones listo para producción.

## Funcionalidades

- **Catálogo de productos** con páginas de detalle y búsqueda por texto.
- **Carrito local** para agregar, quitar y modificar cantidades; calcula el total y guarda los productos con `localStorage`.
- **Tema claro/oscuro** con preferencia persistida en el navegador.
- **Páginas informativas** de inicio, servicios, nosotros y contacto.
- **Galería y carruseles** con interacción JavaScript; requieren los recursos gráficos originales.
- **Formulario de reclamaciones** con validaciones de campos en el navegador. **No guarda ni envía datos a un servidor.**
- Enlaces de ejemplo para compartir consultas por WhatsApp. La versión pública **no contiene el número real del negocio**.

## Tecnologías

| Área | Tecnologías |
| --- | --- |
| Estructura y estilos | HTML5, CSS3, diseño responsivo |
| Interactividad | JavaScript, DOM, eventos, `localStorage` |
| Recursos externos | Font Awesome (iconos), Google Fonts (Nunito) |
| Ejecución | Navegador moderno; servidor estático opcional |

## Ejecución local

**Requisitos:** navegador moderno y, de forma opcional, Python 3 para servir los archivos por HTTP. No se requiere `npm install` ni base de datos.

1. Clonar el repositorio:

   ```bash
   git clone https://github.com/alexvivas/peluquer-aCanina.git
   cd peluquer-aCanina
   ```

2. Desde la carpeta raíz, iniciar el servidor:

   ```bash
   python -m http.server 8000
   ```

   En Windows, si `python` no está reconocido, probar `py -m http.server 8000`.

3. Abrir **http://localhost:8000/Proyecto/inicio.html**.

También puede abrirse `Proyecto/inicio.html` directamente, aunque un servidor local ofrece un entorno más consistente.

**Importante:** sin las imágenes originales, se verán espacios vacíos o imágenes rotas. Consulta [Recursos gráficos](docs/RECURSOS.md) antes de intentar mostrarlo como una demo completa.

## Estructura del repositorio

```text
.
├── README.md
├── CONTRIBUTORS.md
├── .gitignore
├── Proyecto/
│   ├── inicio.html
│   ├── servicios.html
│   ├── productos.html
│   ├── nosotros.html
│   ├── libro.html
│   ├── [páginas de detalle de productos].html
│   ├── css/
│   │   └── [estilos por sección].css
│   ├── js/
│   │   └── app.js
│   └── img/
│       └── README.md  (sin los recursos gráficos originales)
└── docs/
    ├── RECURSOS.md
    └── LIMITACIONES.md
```

## Limitaciones conocidas y consideraciones

- El ZIP de origen no incluía `Proyecto/img/`. La interfaz requiere imágenes y un logotipo externos al archivo recibido.
- El carrito se almacena **solo en el navegador**: no procesa pagos, usuarios ni órdenes reales.
- El formulario de reclamaciones realiza validación frontend, **sin persistencia ni envío**.
- Los datos de contacto, identificadores comerciales y enlaces a redes de un negocio se sustituyeron u omitieron en esta copia pública; son **marcadores de demostración**.
- Los textos y cifras comerciales presentes en el diseño son contenido de ejemplo del trabajo original; **no se certifican como resultados verificados**.
- Las librerías visuales cargadas desde CDN requieren conexión a Internet.

Revisa [Limitaciones y mejoras](docs/LIMITACIONES.md) para la situación técnica y próximos pasos.

## Autoría y procedencia

Proyecto académico **realizado en equipo**. La lista de integrantes y sus contribuciones debe completarse en [CONTRIBUTORS.md](CONTRIBUTORS.md), sin atribuir el trabajo a una sola persona.

El archivo compartido corresponde al proyecto original publicado en [Andre1609/Peluquerias-Caninas](https://github.com/Andre1609/Peluquerias-Caninas). Se reconoce esa procedencia; esta copia incorpora documentación y medidas de privacidad para presentarla como portafolio académico.

## Licencia

**No se ha añadido una licencia de reutilización.** Antes de adoptar una, publicar recursos gráficos o distribuir material de terceros, acordarlo con el equipo y verificar los permisos pertinentes.
