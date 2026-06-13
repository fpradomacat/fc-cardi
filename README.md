# Cardi Wrapped 🎂

Un "Spotify Wrapped" falso para el cumple de Cardi.

## Cómo publicarlo

1. Subí `index.html` a la raíz del repo
2. Settings → Pages → Source: `Deploy from a branch` → `main` / `root`
3. Listo: `https://[tu-usuario].github.io/fc-cardi`

## Cómo personalizar

Todo el contenido está en `index.html`, organizado por bloques claramente marcados con comentarios.

### Agregar una stat grande (slide entero)

Copiá este bloque y cambiá el número, título y footnote:

```html
<section class="slide slide-bigstat theme-purple" id="slide-NOMBRE">
  <p class="eyebrow">Subtítulo pequeño</p>
  <p class="number">42</p>
  <p class="stat-label">descripción de la estadística</p>
  <p class="footnote">Comentario gracioso opcional.</p>
  <div class="tap-zone" onclick="nextSlide()"></div>
</section>
```

**Temas de color disponibles:** `theme-green` · `theme-purple` · `theme-orange` · `theme-pink` · `theme-teal` · `theme-red` · `theme-yellow` · `theme-dark` · `theme-lime`

### Agregar una stat card (grilla)

Dentro de un `.stats-grid`, copiá una de estas:

```html
<!-- Card normal (ocupa 1 columna) -->
<div class="stat-card">
  <div class="sc-num">99</div>
  <div class="sc-label">descripción corta</div>
</div>

<!-- Card ancha (ocupa 2 columnas) -->
<div class="stat-card wide">
  <span class="sc-num">99</span>
  <span class="sc-label">descripción corta</span>
</div>

<!-- Card verde destacada (accent) -->
<div class="stat-card accent">
  <div class="sc-num">99</div>
  <div class="sc-label">descripción corta</div>
</div>
```

### Agregar un apodo

Dentro de `#slide-apodos .apodos-list`:

```html
<div class="apodo-item">
  <span class="apodo-num">#5</span>
  <span class="apodo-name">El Apodo</span>
  <span class="apodo-context">cuándo se usa</span>
</div>
```
