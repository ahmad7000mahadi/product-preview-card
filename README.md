# 🛍️ Product Preview Card Component

## 🔗 Live Site

  * **Live Demo:** [https://ahmad7000mahadi.github.io/product-preview-card/]
  * **Frontend Mentor Solution:** [https://github.com/ahmad7000mahadi/product-preview-card]

## 📝 Overview

This project is a solution to the "Product Preview Card Component" challenge on Frontend Mentor. The goal was to build a mobile-first, responsive e-commerce card that accurately matches the provided design specifications, focusing on layout adaptation between mobile and desktop views.

### The Challenge

Users should be able to:

  * View the optimal layout for the site depending on their device's screen size.
  * See hover and focus states for the interactive elements (the "Add to Cart" button).

## ✨ Features

  * **Responsive Layout:** Automatically switches from a vertical stack on mobile to a two-column, side-by-side layout on desktop.
  * **Fluid Sizing:** Uses the modern CSS function **`min()`** to define the card's maximum width, ensuring it scales responsively while staying visually contained.
  * **Fluid Typography:** Utilizes the CSS function **`clamp()`** on all major text elements (especially the product title) to ensure text size scales smoothly with the viewport, respecting defined minimum and maximum limits.
  * **Semantic HTML5:** Uses appropriate tags (`<main>`, `<picture>`, `<h1>`, `<button>`) for structure and accessibility.
  * **Custom Properties:** A well-organized CSS variable system is used for colors, typography, and spacing, ensuring high maintainability.

## 🛠️ Tech Stack

  * **HTML:** Semantic HTML5
  * **CSS:** Custom Properties (Variables), Flexbox, Mobile-First Workflow
  * **Responsive Tools:** `min()`, `clamp()`, `picture` element for responsive images.

## ⚙️ Project Structure and Setup

### Design Decisions

1.  **Mobile-First Approach:** The base CSS styles the vertical, single-column layout (mobile). The horizontal, two-column layout is implemented only within the `@media (min-width: 600px)` query.
2.  **Layout Switching:** The core of the responsiveness is switching the main `.card` container from `flex-direction: column` (mobile) to `flex-direction: row` (desktop).
3.  **Image Handling:** The `<picture>` element was used to serve different image sources (`image-product-mobile.jpg` and `image-product-desktop.jpg`) based on the screen size, improving initial load performance.
4.  **Pricing Semantics:** The crossed-out price is styled using `text-decoration: line-through;`, accurately communicating the discount.


## 🎨 Styling Guide & Design Tokens

The following design system was implemented using CSS Custom Properties:

| Variable | Property | HSL/Value |
| :--- | :--- | :--- |
| `--color-green-500` | Primary Price/Button | `hsl(158, 36%, 37%)` |
| `--color-cream` | Body Background | `hsl(30, 38%, 92%)` |
| `--color-grey` | Description/Old Price | `hsl(228, 12%, 48%)` |
| `--font-family-heading` | Product Title | Fraunces (700) |
| `--font-family-body` | Body Text | Montserrat (500) |

## 🌟 Author
  * **Frontend Mentor:** [ahmadmahadi](https://www.frontendmentor.io/profile/ahmad7000mahadi)

-----