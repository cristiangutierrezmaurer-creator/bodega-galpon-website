Bodega Galpon Website

Sitio web para arriendo de bodegas y galpones en La Pintana, Santiago (proyectos Miguel Angel 2851 y Los Olmos 2764). Reemplazo del sitio original bodega-galpon.cl.

Que se hizo

Se recreo el sitio como HTML y CSS estatico, sin dependencias ni build, en un archivo unico index.html. Se reprodujo el diseno original: hero, tarjetas de info, dos proyectos con listado de bodegas, caracteristicas, seguridad, galeria y formulario de contacto. El formulario de contacto usa Netlify Forms (atributo data-netlify true) para recibir las solicitudes sin backend propio. Bodega 3 y Bodega 4 de Los Olmos 2764 se marcaron como Disponible segun lo solicitado.

Estructura

index.html es el sitio completo (HTML mas CSS inline). La carpeta images contiene las imagenes, que hay que agregar manualmente (ver siguiente seccion).

Imagenes pendientes

Por limitaciones tecnicas no se pudieron copiar automaticamente las imagenes originales. Hay que subir estos archivos a la carpeta images del repo, arrastrandolos en GitHub con el boton Add file, Upload files: logo.jpg, hero.jpg, miguel-angel.jpg, los-olmos.jpg, gallery-1.jpg, gallery-2.jpg, gallery-3.jpg, gallery-4.jpg.

Como cambiar el estado de una bodega, Disponible o Arrendada

Paso uno: abrir index.html en GitHub con el boton lapiz (Edit). Paso dos: buscar la fila de la bodega que se quiere cambiar. Paso tres: cambiar la clase badge y el texto: para Disponible usar la clase badge disponible con el texto Disponible; para Arrendada usar la clase badge arrendada con el texto Arrendada. Paso cuatro: hacer commit de los cambios (Commit changes). Paso cinco: si el sitio esta conectado a Netlify, se publica solo en uno o dos minutos.

Hosting

Este repo esta pensado para desplegarse gratis en Netlify, conectandolo como sitio nuevo: Add new site, Import an existing project, GitHub, elegir este repo. No requiere build command ni carpeta de publicacion especial.

Formulario de contacto

Para que las respuestas del formulario lleguen por correo, hay que activar en Netlify: Site configuration, Forms, Form notifications, Add notification, Email notification, y poner ahi el correo personal de destino.
