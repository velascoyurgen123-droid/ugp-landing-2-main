# UGP-Proyecto SENA

Landing informativa para presentar un proyecto de sistema web para UGP, empresa dedicada a la organización y promoción de eventos de grappling y fighting.

El objetivo de esta página es explicar qué problema aborda el proyecto, cómo funcionaría la solución y qué beneficios tendría. La landing no es la ticketera final, no procesa pagos y no realiza ventas reales.

## Propuesta del proyecto

UGP-Proyecto SENA plantea centralizar la promoción de eventos y apoyar la automatización de la venta de tickets mediante una plataforma web.

El sistema proyectado podría incluir publicación de eventos, fechas, lugares y cartelera; información de participantes; consulta de localidades y precios; compra de entradas mediante una ticketera digital; integración futura con Wompi u otra pasarela; generación de comprobantes; y consulta administrativa de ventas y asistentes.

Estas funciones representan el alcance propuesto. No son funcionalidades conectadas o disponibles en esta landing.

## Cómo ejecutar el proyecto

Está construido con HTML, CSS y JavaScript puro. No utiliza Node.js, React, Vue ni un sistema de compilación.

- Abre `index.html` directamente en el navegador.
- Usa la extensión **Live Server** de Visual Studio Code.
- Sirve la carpeta con cualquier servidor local estático.

Las tipografías se cargan desde Google Fonts. Sin internet se utilizan las fuentes de respaldo definidas en CSS.

## Estructura

```text
index.html                         Estructura completa de la landing
css/style.css                      Identidad visual, layout y componentes
js/data.js                         Datos dinámicos de eventos y funcionalidades
js/ui.js                           Filtros, tablas, tarjetas y animaciones
assets/images/branding/             Logo y recursos gráficos de la marca
assets/images/events/               Flyers de eventos
assets/images/fighters/             Imágenes de enfrentamientos
assets/images/maps/                 Planos de localidades
assets/images/sponsors/             Recursos de patrocinadores
assets/vendor/three.min.js          Biblioteca conservada como recurso anterior
js/hero-3d.js                       Código anterior 3D, no cargado actualmente
```

## Identidad visual

La identidad se basa en el emblema UGP proporcionado para el proyecto y una ambientación deportiva con inspiración de Halloween.

```css
Negro carbón     #101010
Gris oscuro      #242424
Rojo vino        #8E1F2D
Rojo intenso     #F04438
Naranja          #FF7518
Morado oscuro    #24152F
Blanco           #F5F5F5
```

Se utilizan fondos oscuros, humo, resplandores rojos, pintura, puños de combate y efectos de impacto.

Tipografías:

- **Bebas Neue** para títulos, botones y elementos destacados.
- **Montserrat** para textos, navegación y contenido descriptivo.

## Recursos gráficos

```text
assets/images/branding/ugp-logo.png       Logo de UGP
assets/images/branding/fists.svg          Ilustración de puños deportivos
assets/images/branding/red-splatter.svg   Salpicaduras de pintura roja
assets/images/branding/impact-burst.svg   Líneas y efecto de impacto
```

Los SVG se integran como capas independientes para poder editarlos o reemplazarlos sin reescribir la portada.

## Secciones

- **Inicio:** presentación de UGP-Proyecto SENA y del sistema web.
- **El proyecto:** promoción, ticketera, pagos y control.
- **Metodología:** recorrido desde la publicación hasta la administración del evento.
- **Contenido:** información que el público consultaría antes de comprar.
- **Comunidad:** roles del administrador, organizador, comprador y personal de control.
- **Galería:** espacio para experiencias y recursos visuales.
- **Actividades:** eventos e historial mediante datos dinámicos.
- **Boletería:** localidades y precios de referencia.
- **Patrocinio:** propuesta para aliados.
- **Plataforma:** problema identificado y solución planteada.
- **Alcance:** funcionalidades previstas.
- **Contacto:** canales del proyecto.

## Archivos dinámicos

`js/data.js` concentra los datos utilizados por la interfaz:

- `DATA.events`: eventos, fechas, lugares, imágenes y estados.
- `DATA.stateLabel`: nombres visibles de los estados.
- `DATA.prices`: tablas de localidades y precios de referencia.
- `DATA.features`: funcionalidades planteadas para el sistema.

`js/ui.js` genera filtros, tarjetas, tablas, estados y animaciones de entrada.

Los scripts son clásicos y se cargan en este orden:

```text
data.js → ui.js
```

La escena 3D anterior ya no se carga; la portada actual utiliza una composición gráfica propia y responsive.

## Responsive y accesibilidad

- Diseño adaptable para escritorio, tablet y celular.
- Navegación controlada en pantallas pequeñas.
- Textos alternativos en imágenes informativas.
- Recursos decorativos tratados como no informativos.
- Animaciones mediante `IntersectionObserver`.
- Respeto de `prefers-reduced-motion`.
- Colores centralizados en variables CSS.

## Estado y límites

Esta carpeta contiene la landing de presentación, no el sistema web completo. Actualmente no incluye backend, base de datos, usuarios, procesamiento real con Wompi, venta real de tickets, validación de QR ni panel administrativo funcional.

La landing explica esas funciones como propuesta y alcance futuro del sistema.

## Reglas de contenido

- No presentar como implementada una función que solo está propuesta.
- No inventar fechas, precios, nombres o integraciones confirmadas.
- Marcar la información demostrativa o de referencia.
- Mantener separados los datos, la estructura HTML y los estilos.
- Usar recursos gráficos propios o autorizados para el proyecto.
