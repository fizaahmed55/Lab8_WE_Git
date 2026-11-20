# ShopGrid – Responsive E-Commerce Product Gallery

Web Engineering **Lab 8** (UET Taxila) – CSS Grid Layouts & Git/GitHub Version Control.

A product gallery page whose grid adjusts its number of columns to the screen width by itself,
using CSS Grid `auto-fit` and `minmax()`, with **no media queries**. Each product card has hover animations.

## Features

- Auto-responsive grid: `repeat(auto-fit, minmax(250px, 1fr))`
  - 4 columns on a wide desktop, 3 on a laptop/tablet, 2 on a small tablet, 1 on a phone
  - Cards are never narrower than 250px and stretch to share any leftover space
- Hover animations on every card:
  - card lifts up (`translateY`) with a deeper shadow
  - product image zooms and tilts (`scale` + `rotate`)
  - "Add to Cart" button fills in with colour
  - "New" / "Sale" badge pulses (`@keyframes`)
- Flexbox header with wrapping navigation, also without media queries

## Key CSS

```css
.product-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 24px;
}

.product-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 16px 30px rgba(0, 51, 102, 0.25);
}
```

## Files

| File | Purpose |
| --- | --- |
| `index.html` | Page structure: header, product grid with 8 product cards, footer |
| `style.css` | CSS Grid layout, card styling and hover animations |
| `README.md` | Project description (this file) |

## How to run

1. Clone the repository:
   `git clone https://github.com/your-username/Lab8_WE_Git.git`
2. Open `index.html` in any modern browser (or use the VS Code *Live Server* extension).
3. Resize the browser window to watch the grid change its number of columns.

## Tools

HTML5, CSS3 (Grid, Flexbox, transitions, keyframes), Visual Studio Code, Git, GitHub.

## Author
Fiza Ahmed
