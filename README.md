# Image Grid Layout Component

Un componente de galería de imágenes responsiva, creado con **HTML y CSS puro** usando CSS Grid. Ideal para portfolios o landing pages que requieran mostrar múltiples imágenes de forma ordenada sin depender de JavaScript.

[![Project](https://roadmap.sh/projects/image-grid)](https://roadmap.sh/projects/image-grid)

---

## 🎯 Características

- Galería de imágenes usando solo **CSS Grid**
- Diseño responsive y fluido en diferentes dispositivos
- Elementos autoajustables según el ancho disponible
- Estilos simples y fáciles de personalizar
- Compatible con todos los navegadores modernos

---

## 🚀 Cómo usar

1. Cloná el repositorio o descargá el archivo ZIP.
2. Abrí `index.html` en tu navegador para ver el componente en acción.
3. Editá `index.html` para agregar tus propias imágenes (`<img src="...">`).
4. Ajustá el estilo en `style.css` para modificar **columnas**, **gaps**, **proporciones**, etc.
5. (Opcional) Subí el proyecto a GitHub Pages o tu servidor personal para compartir una demo pública.

---

## 🔧 Personalización

- **Columnas**: Podés cambiar el número de columnas editando `grid-template-columns` en `style.css`.
- **Espacio entre imágenes**: Modificá los `gap` (fila/columna) para ajustar el espaciado.
- **Tamaño y posición**: Usá `grid-row`, `grid-column` o `grid-area` para destacar imágenes específicas.
- **Galería organizada**: Podés definir una sección con imágenes grandes y otras más pequeñas para mayor dinamismo visual.

---

## 📁 Estructura del Proyecto

```
Image-Grid-Layout/
├── assets/
│   └── preview.png          # Vista previa opcional del layout final
├── index.html               # Estructura HTML de la galería
├── style.css                # Estilos CSS con CSS Grid
└── README.md                # Este archivo
```

---

## 🧪 Ejemplo de implementación

```html
<div class="grid-container">
  <div class="item item1">
    <img src="images/img1.jpg" alt="Descripción 1" />
  </div>
  <div class="item item2">
    <img src="images/img2.jpg" alt="Descripción 2" />
  </div>
  <div class="item item3">
    <img src="images/img3.jpg" alt="Descripción 3" />
  </div>
  <!-- ...más imágenes según tu gusto -->
</div>
```

```css
.grid-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  grid-auto-rows: 150px;
  gap: 10px;
}
.grid-container .item img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
```

---

## 📸 Captura de pantalla

> Si contás con una imagen o GIF que muestre el resultado final, incluila como `assets/preview.png`: mejorará mucho la primera impresión del proyecto.

---

## 📜 Licencia

Este proyecto está bajo la **Licencia Apache‑2.0**. Podés usarlo, modificarlo y distribuirlo libremente bajo sus términos.

---

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Podés abrir un `issue` o enviar un `pull request` para:

- Mejorar el layout (e.g. más formatos de grid)
- Agregar animaciones CSS (hover, transición)
- Añadir accesibilidad (alt, foco visual)
- Integrar versiones con JavaScript para crear lightbox, filtrado, etc.

---

Hecho con ❤️ por [David Rogaci](https://github.com/davidrogaci)
