# Brew & Bloom Café — CET138 Full Stack Development Assignment 1

## Project Overview
A responsive café website built to demonstrate understanding of:
- HTML (semantic structure)
- CSS (custom styling and design)
- Bootstrap 5 Framework (responsive layout and components)
- JavaScript (interactivity and DOM manipulation)

---

## File Structure

```
cafe-website/
│
├── index.html          ← Homepage (hero, about, popular items, hours)
├── menu.html           ← Menu page with JS-powered category filter
├── gallery.html        ← Gallery with Bootstrap carousel + lightbox modal
├── contact.html        ← Booking form with full JS validation
│
├── css/
│   └── style.css       ← All custom CSS styles
│
├── js/
│   ├── main.js         ← Shared JS: navbar scroll, fade-in animations
│   ├── menu.js         ← Menu filter functionality
│   ├── gallery.js      ← Lightbox modal population
│   └── contact.js      ← Form validation and submission
│
└── images/             ← Add your own photos here (see instructions below)
    └── README.txt
```

---

## How to Run

1. Open `index.html` in any modern web browser.
2. No server or installation required — it runs as static files.
3. For best results, use VS Code with the **Live Server** extension.

---

## Adding Real Images

Replace placeholder elements with `<img>` tags:

### Carousel (gallery.html)
```html
<!-- Replace this: -->
<div class="carousel-placeholder">...</div>

<!-- With this: -->
<img src="images/bar.jpg" class="d-block w-100" alt="The espresso bar">
```

### Gallery Grid (gallery.html)
The `data-img` attribute on each `.gallery-thumb` controls the lightbox image:
```html
<div class="gallery-thumb" data-img="images/photo1.jpg" ...>
```
Add your photo file to the `images/` folder and update the path.

### Menu Cards
```html
<!-- Replace this: -->
<div class="menu-card-img-placeholder"><i class="bi bi-cup-hot"></i></div>

<!-- With this: -->
<img src="images/flat-white.jpg" alt="Oat flat white">
```

---

## Technologies Demonstrated

### HTML
- Semantic tags: `<nav>`, `<header>`, `<main>`, `<section>`, `<footer>`, `<article>`
- Forms: `<form>`, `<input>`, `<select>`, `<textarea>`, `<label>`
- Accessibility: `aria-label`, `aria-expanded`, `role`, `tabindex`
- Bootstrap integration via CDN `<link>` and `<script>`

### CSS (css/style.css)
- CSS custom properties (variables) for a consistent design system
- Flexbox and CSS Grid layout
- Responsive typography with `clamp()`
- Hover effects and transitions
- Pseudo-elements (`::before`, `::after`) for decorative circles
- `@media` query for mobile breakpoints
- `position: sticky` for the booking sidebar

### Bootstrap 5
- Responsive navbar with hamburger toggle (`navbar-expand-lg`)
- Grid system (`col-sm-6 col-lg-4`)
- Carousel with fade transition (`carousel-fade`)
- Modal component for lightbox (`modal`, `modal-dialog-centered`)
- Form classes (`form-control`, `form-select`, `form-check`)
- Utility classes (`d-flex`, `gap-3`, `text-center`, `py-5`, etc.)
- Bootstrap Icons via CDN

### JavaScript
| File | What it demonstrates |
|------|---------------------|
| `main.js` | `scroll` event listener, `IntersectionObserver`, `classList.add/remove` |
| `menu.js` | `data-*` attributes, `forEach`, filter logic, show/hide elements |
| `gallery.js` | Bootstrap modal events (`show.bs.modal`), dynamic HTML injection |
| `contact.js` | Form validation, regex, `Date` object, `setTimeout`, error handling |

---

## Customisation

- **Brand name**: Find and replace "Brew & Bloom" throughout HTML files
- **Colours**: Edit CSS variables at the top of `css/style.css` (`:root` block)
- **Menu items**: Add/edit `.menu-item` divs in `menu.html`
- **Prices**: Update the `.menu-card-price` spans in `menu.html` and `index.html`
- **Location/hours**: Update `index.html` and `contact.html`

---

## Browser Support
Chrome, Firefox, Safari, Edge — all modern browsers. Requires ES6+ support.
