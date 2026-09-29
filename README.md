# 🍽️ Food Project

A responsive food delivery and restaurant web application built with clean HTML5 and modern CSS3. This repository documents lecture-by-lecture progress, tracking foundational folder architecture, typography setup, responsive grid integration, and full page section builds.

---

## 📑 Table of Contents
- [Overview](#overview)
- [Folder Architecture](#folder-architecture)
- [Course Progress & Lecture Summaries](#course-progress--lecture-summaries)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)

---

## 🎯 Overview

The **Food Project** demonstrates modular front-end web development practices. By maintaining a clean separation between third-party frameworks in `vendors/` and custom implementations in `resources/`, the project establishes a scalable, production-ready foundation for responsive design[cite: 7, 8, 9, 10, 11, 12].

---

## 📁 Folder Architecture

The codebase separates custom code from external dependencies:

- **`resources/`**: Dedicated exclusively to custom assets and authored code, including stylesheets (`style.css`), images (`hero-image.jpg`), application scripts, and mock data[cite: 7, 8, 11, 12].
- **`vendors/`**: Houses all external libraries, frameworks, vendor fonts, and utility files—such as `normalize.css` and `grid.css`—ensuring dependencies remain isolated and clean[cite: 7, 9, 10, 11].

---

## 📖 Course Progress & Lecture Summaries

### 📚 Lecture 1 Summary: Setting Up the Folder Structure
- **`resources/` Directory**: Houses your own custom assets and authored code (e.g., custom stylesheets `style.css`, project-specific images, client-side scripts, and local datasets)[cite: 7, 8].
- **`vendors/` Directory**: Houses all external, third-party libraries, frameworks, vendor fonts, and utility stylesheets such as `normalize.css` to keep dependencies cleanly separated from custom code[cite: 7].
- **CSS Reset & Normalization**: Incorporates `normalize.css` ahead of custom styles to ensure HTML elements render uniformly across different browsers before applying project-level resets[cite: 7, 8].
- **Global Base Rules & Typography**: Sets universal `box-sizing: border-box`, standardizes font sizing, integrates Google Web Fonts, and enhances text legibility using `optimizeLegibility`[cite: 7, 8].

### 📚 Lecture 2 Summary: Responsive Grid System
- **Grid System Integration**: Downloaded and added `grid.css` from the [Responsive Grid System](https://www.responsivegridsystem.co.uk/) into `vendors/css/` to establish a flexible, column-based layout foundation[cite: 9, 10].
- **Fluid Proportional Columns**: Utilizes percentage-based fractional column classes spanning from 2 up to 12 columns (e.g., `.span_1_of_2`, `.span_1_of_3`, `.span_1_of_4`) alongside `.col` floats and margins[cite: 10].
- **Clearfix Self-Clearing**: Implements micro-clearfix rules (`.group:before`, `.group:after`) to ensure parent containers properly contain floated grid columns[cite: 10].
- **Mobile Fluidity**: Employs a `@media only screen and (max-width: 480px)` query that removes column margins and stacks all grid spans to 100% full width on mobile screens[cite: 10].
- **Layout Container Setup**: Introduced structural wrapper elements (`<div class="row">`) in `index.html` to center and constrain content rows[cite: 9].

### 📚 Lecture 3 Summary: Header Section - Part-1
- **Hero Section Markup**: Structured a semantic `<header>` element containing a `.hero-text-box` with a primary headline (`<h1>`) and dual call-to-action anchor links.
- **Full-Screen Hero Background**: Applied `hero-image.jpg` as a responsive full-viewport background (`height: 100vh`) using `background-size: cover` and `background-position: center`[cite: 12].
- **Absolute Center Positioning**: Centered the `.hero-text-box` vertically and horizontally using `position: absolute`, `top: 50%`, `left: 50%`, and `transform: translate(-50%, -50%)` constrained to a `1140px` layout width[cite: 12].
- **Typography Transition**: Replaced initial fonts with the clean, versatile Google Font `Lato` (light weight 300) to establish an elegant modern aesthetic[cite: 11, 12].

---

## 🛠️ Technologies Used

- **HTML5**: Semantic document structuring (`<header>`, text containers, links)[cite: 11].
- **CSS3**: Layouts, resets, typography, absolute coordinate centering, and viewport-height styling[cite: 10, 12].
- **Normalize.css**: Cross-browser baseline normalization[cite: 11].
- **Responsive Grid System (`grid.css`)**: Lightweight fluid column framework[cite: 10, 11].
- **Google Fonts**: `Lato` web font family[cite: 11, 12].

---

## 📂 Project Structure

```text
15. Food Project/
├── resources/
│   ├── css/
│   │   ├── img/
│   │   │   └── hero-image.jpg
│   │   └── style.css
│   ├── data/
│   ├── img/
│   └── js/
├── vendors/
│   ├── css/
│   │   ├── grid.css
│   │   └── normalize.css
│   ├── fonts/
│   └── js/
└── index.html
