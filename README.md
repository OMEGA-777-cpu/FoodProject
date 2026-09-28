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

The **Food Project** demonstrates modular front-end web development practices. By maintaining a clean separation between third-party frameworks in `vendors/` and custom implementations in `resources/`, the project establishes a scalable, production-ready foundation for responsive design[cite: 7, 8, 9, 10].

---

## 📁 Folder Architecture

The codebase separates custom code from external dependencies:

- **`resources/`**: Dedicated exclusively to custom assets and authored code, including stylesheets (`style.css`), images, application scripts, and mock data[cite: 7, 8].
- **`vendors/`**: Houses all external libraries, frameworks, vendor fonts, and utility files—such as `normalize.css` and `grid.css`—ensuring dependencies remain isolated and clean[cite: 7, 9, 10].

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
- **Layout Container Setup**: Introduced structural wrapper elements (`<div class="row">`) in `index.html` to center and constrain content rows.

---

## 🛠️ Technologies Used

- **HTML5**: Semantic document structuring[cite: 9].
- **CSS3**: Layouts, resets, typography, and responsive media queries[cite: 8, 10].
- **Normalize.css**: Cross-browser baseline normalization[cite: 9].
- **Responsive Grid System (`grid.css`)**: Lightweight fluid column framework[cite: 9, 10].
- **Google Fonts**: `Bitcount Single` and `Nova Round` web fonts[cite: 9].

---

## 📂 Project Structure

```text
15. Food Project/
├── resources/
│   ├── css/
│   │   ├── img/
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
