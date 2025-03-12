# Documentación del Proyecto Web: Mi Café Favorito

## Índice

- [Documentación del Proyecto Web: Mi Café Favorito](#documentación-del-proyecto-web-mi-café-favorito)
  - [Índice](#índice)
  - [Introducción](#introducción)
  - [Implementación y Publicación](#implementación-y-publicación)
  - [Estructura y Contenido](#estructura-y-contenido)
    - [**Inicio**](#inicio)
    - [**Tipos de Café**](#tipos-de-café)
    - [**Tienda**](#tienda)
    - [**Contacto**](#contacto)
  - [Elementos Multimedia](#elementos-multimedia)
  - [Diseño y Estilos](#diseño-y-estilos)
    - [**Fuentes Tipográficas**](#fuentes-tipográficas)
    - [**Iconografía**](#iconografía)
    - [**Esquema de Colores**](#esquema-de-colores)
  - [Uso de Bootstrap](#uso-de-bootstrap)
  - [Metodología Ágil](#metodología-ágil)
  - [Extras y Diferenciación](#extras-y-diferenciación)
  - [Conclusión](#conclusión)

## Introducción

La presente documentación describe el desarrollo de la página web **"Mi Café Favorito"**, un sitio informativo y comercial que explora el mundo del café y ofrece recetas de bebidas a base de café. La página se desarrolló utilizando **HTML, CSS3 y Bootstrap**, siguiendo metodologías ágiles y enfocándose en una experiencia visual atractiva y funcional.

Si bien se utilizó **Bootstrap** para la maquetación y diseño, la página **no es completamente responsiva**, ya que este no era el enfoque principal del proyecto.

## Implementación y Publicación

- **Repositorio de código:** [GitHub](https://github.com/andresmorenoj/mi-cafe-favorito)
- **Alojamiento web:** Despliegue en **Vercel**.
- **URL del sitio:** [Mi Café Favorito](https://mi-cafe-favorito.vercel.app/)

## Estructura y Contenido

La página web se compone de cuatro secciones principales:

### **Inicio**
- Contiene un banner con un título y un mensaje invitando a descubrir el mundo del café.
- Se incluye un listado de tres tarjetas informativas sobre los beneficios del café.

### **Tipos de Café**
- Presenta un video en modo **muted y autoplay**, acompañado de un texto y un botón animado para hacer scroll hacia las tarjetas con información sobre diferentes tipos de café.
- Estas tarjetas incluyen un **carrusel de imágenes** representativas.

### **Tienda**
- Contiene un banner con un mensaje llamativo seguido de tarjetas con información sobre bebidas a base de café.
- Cada tarjeta muestra el nombre de la bebida, el precio de la receta y una breve descripción.
- Al hacer clic en "Comprar receta", se abre un **modal** para completar la compra, seguido de otro **modal** que muestra la receta adquirida.

### **Contacto**
- Incluye un **formulario de contacto**.
- Al enviar el mensaje, se abre un **modal de confirmación** con un botón de regreso a la página de inicio.

## Elementos Multimedia

Se incorporaron diversos elementos multimedia:

- **Imágenes:** Descargadas de Google y convertidas a **formato WebP** para optimizar el rendimiento.
- **Iconos:** Obtenidos en **formato SVG** desde Bootstrap Icons.
- **Video:** Usado en **formato MP4** en la sección de tipos de café.
- **Animaciones y sombreados:** Aplicados a diferentes componentes para mejorar la experiencia visual.

## Diseño y Estilos

### **Fuentes Tipográficas**

- **Just Me Again Down Here:** para el logotipo.
- **Lato:** para los títulos.
- **Inter:** para los textos.
- Descargadas desde Google Fonts e incorporadas mediante un enlace en HTML.

```html
<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@100..900&family=Just+Me+Again+Down+Here&family=Lato:wght@100;300;400;700;900&display=swap" rel="stylesheet" />
```

### **Iconografía**
- Se utilizaron **iconos de Bootstrap** descargados en formato **SVG**.

### **Esquema de Colores**
Se definió un esquema de colores en un archivo `variables.css`, con tonos marrones, naranjas y amarillos para reflejar la temática del café.

```css
:root {
    /* Fuentes */
    --fuente-firma: "Just Me Again Down Here", cursive, sans-serif;
    --fuente-titulos: "Lato", sans-serif, Arial, Helvetica;
    --fuente-textos: "Inter", sans-serif, Arial, Helvetica;
  
    /* Colores */
    --color-marron-oscuro: #3c1518;
    --color-marron-medio: #69140e;
    --color-naranja: #a44200;
    --color-naranja-claro: #D58936;
    --color-amarillo-claro: #f2f3ae;
    --color-gris: #222222;
    --color-negro: #000000;
    --color-blanco: #ffffff;
  
   /* Tamaños de texto (en rem) */
   --tamano-texto-xs: 0.875rem; /* 14px */
   --tamano-texto-s: 1rem; /* 16px */
   --tamano-texto-m: 1.125rem; /* 18px */
   --tamano-texto-l: 1.5rem; /* 24px */
   --tamano-texto-xl: 1.75rem; /* 28px */
   --tamano-texto-xxl: 2rem; /* 32px */
   --tamano-texto-xxxl: 2.5rem; /* 40px */
 
   /* Tamaños generales (en rem) */
   --tamano-0: 0; /* 16px */
   --tamano-xs-general: 0.25rem; /* 4px */
   --tamano-s-general: 0.5rem; /* 8px */
   --tamano-m-general: 1rem; /* 16px */
   --tamano-l-general: 1.5rem; /* 24px */
   --tamano-xl-general: 2rem; /* 32px */
   --tamano-xxl-general: 3rem; /* 48px */
   --tamano-xxxl-general: 3.875rem; /* 62px */
 
   /* Bordes (en rem) */
   --borde-radio-extra-pequeno: 0.25rem; /* 4px */
   --borde-radio-pequeno: 0.5rem; /* 8px */
   --borde-radio-normal: 0.625rem; /* 10px */
   --borde-ancho-normal: 0.0625rem; /* 1px */
  }
```

## Uso de Bootstrap

Se implementaron los siguientes componentes de Bootstrap:

- **Cards:** Para estructurar información en diferentes secciones.
- **Carousels:** Para visualizar imágenes en la sección de tipos de café.
- **Modals:** Para la compra de recetas y confirmaciones de contacto.
- **Grid System:** Para estructurar el diseño.

Se usó una combinación de **estilos predeterminados de Bootstrap y estilos personalizados** para colores y tamaños.

## Metodología Ágil

Se utilizó **Kanban** como metodología ágil. El equipo planificó y organizó las tareas en base a tiempos estimados y el diseño previo.

## Extras y Diferenciación

- Las funcionalidades de la página son **demostrativas**, ya que no se implementó JavaScript para funciones dinámicas avanzadas.
- Se diseñó una **experiencia visual atractiva y optimizada**, aplicando buenas prácticas de diseño web.
- Aunque se usó Bootstrap, **la página no es completamente responsiva**.

## Conclusión

El proyecto **"Mi Café Favorito"** es una página informativa y comercial que combina **diseño atractivo, estructura clara y uso de tecnologías web modernas**. A través de la metodología **Kanban** y el uso de **Bootstrap**, se logró un desarrollo eficiente, con un diseño optimizado para el usuario final.

