# Yental Group SL

Web estatica corporativa para Yental Group SL.

## Archivos

- `index.html`: contenido de la web.
- `styles.css`: estilos visuales y responsive.
- `assets/logo-color.svg`: logo principal en color.
- `assets/logo-blanco.svg`: logo blanco para fondos oscuros.
- `assets/fonts/`: tipografia Urbanist guardada localmente.
- `assets/hero-yental.jpg`: imagen principal optimizada.
- `assets/favicon.svg`: icono basico del sitio.
- `assets/placeholder-container.svg`, `assets/placeholder-solar.svg`, `assets/placeholder-construction.svg`: marcadores temporales para sustituir por imagenes de stock.

## Multimedia recomendada

La web esta preparada para usar multimedia local, subida al mismo hosting. Esto es importante para Cuba: evita depender de YouTube, Vimeo, Google, mapas, formularios externos o imagenes alojadas fuera.

### Imagen principal

Archivo actual:

- `assets/hero-yental.jpg`

Esta imagen queda como respaldo/poster del video del banner.

Contenido recomendado:

- puerto comercial;
- contenedores;
- pallets o carga preparada;
- paneles solares o mercancia industrial;
- luz clara, aspecto profesional, sin logos de terceros visibles.

Formato recomendado:

- JPG;
- ancho minimo 1600 px;
- peso ideal menor de 500 KB;
- nombre final: `hero-yental.jpg`.

### Video principal de operaciones

El banner principal usa actualmente:

- `assets/hero-video.mp4`
- `assets/hero-video-mobile.mp4` para pantallas moviles hasta 620 px de ancho

Tambien puede usarse video en la seccion "Operacion internacional". Cuando tengas el video definitivo, lo recomendable es guardar:

- `assets/video-operaciones.mp4`
- opcional: `assets/video-operaciones-poster.jpg`

Contenido recomendado:

- barco portacontenedores entrando o saliendo de puerto;
- carga de contenedores;
- plano de puerto logistico;
- mercancia moviendose en almacen;
- duracion corta, entre 8 y 15 segundos;
- sin audio o con audio desactivado;
- peso ideal menor de 5 MB para produccion, especialmente pensando en conexiones desde Cuba.

Cuando tengas el archivo, se puede reemplazar el bloque placeholder por una etiqueta `<video>`.

### Imagen de logistica

Archivo placeholder actual:

- `assets/placeholder-container.svg`

Sustituir por:

- `assets/logistica-contenedores.jpg`

Contenido recomendado:

- contenedores en puerto;
- almacen con pallets;
- carga lista para exportacion;
- grua portuaria o camion logistico.

### Imagen de energia solar

Archivo placeholder actual:

- `assets/placeholder-solar.svg`

Sustituir por:

- `assets/energia-solar.jpg`

Contenido recomendado:

- paneles solares;
- baterias o inversores;
- instalacion fotovoltaica;
- imagen limpia, tecnica y luminosa.

### Imagen de construccion

Archivo placeholder actual:

- `assets/placeholder-construction.svg`

Sustituir por:

- `assets/construccion-materiales.jpg`

Contenido recomendado:

- materiales de construccion;
- herramientas;
- sacos, perfileria, ceramica, tuberias o acabados;
- mercancia organizada, no obra desordenada.

## Recomendacion de publicacion

Para que pueda verse en Cuba sin VPN, la opcion mas prudente es un hosting europeo barato con web estatica y DNS en Cloudflare en modo "DNS only".

Evitar en la primera version:

- constructores como Wix, Webflow o Squarespace si no se puede verificar bien el acceso desde Cuba;
- formularios externos;
- Google Fonts, reCAPTCHA, mapas, analytics o scripts de terceros;
- imagenes servidas desde dominios externos.

## Publicacion economica

1. Contratar un hosting compartido europeo sencillo.
2. Subir `index.html`, `styles.css` y la carpeta `assets` al directorio publico del hosting.
3. En Cloudflare, crear o editar estos DNS:
   - `A` para `@` apuntando a la IP del hosting.
   - `CNAME` para `www` apuntando a `yentalgroup.com`, o segun indique el hosting.
4. Dejar esos registros en gris, "DNS only", al menos al inicio.
5. Activar SSL en el hosting.

La web no usa backend ni base de datos, por lo que el costo mensual puede ser muy bajo.
