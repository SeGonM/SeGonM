<!-- Reemplaza las URLs de las imágenes por tus propias imágenes para personalizar tu perfil. Sube las imágenes a /assets/ y usa las URLs en raw.githubusercontent.com si lo prefieres. -->
# SeGonM 👋

<p align="center">
  <!-- He cambiado height a auto para evitar que la imagen se deforme. -->
  <img src="https://i.pinimg.com/1200x/17/a8/31/17a8315b6869a21b72ffe7f9e06e8684.jpg" alt="Banner" style="width: 100%; height: auto; display: block; border-radius: 8px;">
</p>


### Samuel González Muñoz — SeGonM
<table>
  <tr>
    <td valign="top" width="65%">

Hola — soy Samuel. Profesional enfocado en la **extracción, limpieza y análisis de datos** para la toma de decisiones estratégicas. Me gusta construir soluciones prácticas, mantener código [...]

- ⚙️ **Enfoque:** Código modular y optimización de procesos.
- 🛠️ **Metodología:** Control de versiones y estructura de datos limpia.
- ⚡ **Disponibilidad:** Abierto a nuevos retos que requieran análisis crítico y ejecución técnica.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/SeGonM)
[![Gmail](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sml.munoz.gonzalez@gmail.com)

</td>
    <td valign="top" width="35%">
      <p align="center">
        <!-- Reemplaza esta URL por tu foto/avatar -->
        <img src="https://raw.githubusercontent.com/SeGonM/SeGonM/main/assets/image3.jpg" alt="Samuel" style="width:200px; border-radius: 50%;">
      </p>
    </td>
  </tr>
</table>

---

<p align="left">
  <img src="https://skillicons.dev/icons?i=python,postgres,git,github,vscode,arch&theme=dark" alt="skills" />
</p>

---

### Sobre mí

Soy especialista en convertir datos en información accionable: limpieza, transformación y visualización para apoyar decisiones. Me interesa especialmente la reproducibilidad, pipelines de datos[...]

### Contacto

- LinkedIn: https://www.linkedin.com/in/SeGonM
- Email: sml.munoz.gonzalez@gmail.com

---

<p align="right">
  <i>"Los datos son el lenguaje de la eficiencia."</i>
</p>

---

## Guía rápida: evitar que el banner (imagen) se deforme

Si al poner un banner la imagen se deforma, normalmente es porque se están fijando ancho y alto de forma que rompen la relación de aspecto original. Aquí tienes soluciones prácticas y ejemplos para mantener la imagen sin deformarse.

### 1) Usando una etiqueta <img> responsiva (mantiene la proporción)

HTML:

```html
<div class="banner">
  <img src="ruta/a/tu/banner.jpg" alt="Banner">
</div>
```

CSS (inline en README no siempre aplica; lo mejor es usar height:auto en la etiqueta):

```css
.banner img {
  width: 100%;    /* ocupa el ancho del contenedor */
  height: auto;   /* mantiene la proporción, no se deforma */
  display: block; /* elimina el espacio inferior */
}
```

Notas: la imagen nunca se estira; puede aparecer con espacios arriba/abajo si el contenedor tiene una altura fija.

### 2) Usando la imagen como background de un contenedor (dos opciones)

- Opción "llenar sin estirar" (mantiene proporción, puede recortar):

```css
.banner {
  height: 300px;
  background-image: url('ruta/a/tu/banner.jpg');
  background-size: cover;       /* rellena el contenedor, mantiene proporción, puede recortar */
  background-position: center;  /* centra la porción visible */
  background-repeat: no-repeat;
}
```

- Opción "mostrar toda la imagen sin recorte" (mantiene proporción, puede dejar espacio vacío):

```css
.banner {
  height: 300px;
  background-image: url('ruta/a/tu/banner.jpg');
  background-size: contain;     /* muestra toda la imagen, mantiene proporción, puede dejar espacio */
  background-position: center;
  background-repeat: no-repeat;
  background-color: #000;       /* color de relleno si hay espacios */
}
```

### 3) Usando <img> dentro de un contenedor con tamaño fijo (object-fit)

HTML:

```html
<div class="banner">
  <img src="ruta/a/tu/banner.jpg" alt="Banner">
</div>
```

CSS:

```css
.banner {
  height: 300px;
  width: 100%;
  overflow: hidden;
}
.banner img {
  width: 100%;
  height: 100%;
  object-fit: cover;     /* cover = llena y recorta si es necesario; contain = muestra todo */
  object-position: center;
  display: block;
}
```

Consejo: no pongas `width: 100%` y `height: 100%` en un <img> sin `object-fit` — eso estira la imagen.

### Consejos adicionales
- Revisa atributos HTML `width`/`height` en la etiqueta `<img>` y elimínalos o pon `height="auto"` si causan estiramiento.
- Usa imágenes de suficiente resolución para evitar pixelado si se escalan en pantallas grandes.
- Para móviles, considera `srcset` o `<picture>` y media queries para ofrecer recortes/resoluciones adecuados.
- Si quieres que el banner sea "estático" (no cambie al redimensionar), usa dimensiones en px en el contenedor y `object-fit: cover`; ten en cuenta que en pantallas pequeñas se recortará.

---

<!-- Notas:
  - Para usar tus propias imágenes: sube el banner y la foto al repo (por ejemplo en /assets/) y reemplaza las URLs por las del raw blob:
    https://raw.githubusercontent.com/SeGonM/SeGonM/main/assets/tu-imagen.png
  - Si quieres que coloque tus imágenes yo mismo, pásame los ficheros o las URLs y lo dejo listo.
  - Si prefieres un diseño más oscuro/estilizado (como la captura), puedo ajustar colores, añadir tarjetas y botones con enlaces.
-->
