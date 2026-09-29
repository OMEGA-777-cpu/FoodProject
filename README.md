# 🍽️ Food Project

A responsive food delivery and restaurant web application built with clean HTML5 and modern CSS3[cite: 16, 17]. This repository documents lecture-by-lecture progress, tracking foundational folder architecture, typography setup, responsive grid integration, and full page section builds[cite: 7, 8, 9, 10, 11, 14, 16, 17].

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

The **Food Project** demonstrates modular front-end web development practices[cite: 7, 9, 16]. By maintaining a clean separation between third-party frameworks in `vendors/` and custom implementations in `resources/`, the project establishes a scalable, production-ready foundation for responsive design[cite: 7, 9, 10, 16, 17].

---

## 📁 Folder Architecture

The codebase separates custom code from external dependencies[cite: 7, 9, 16]:

- **`resources/`**: Dedicated exclusively to custom assets and authored code, including stylesheets (`style.css`), images (`hero-image.jpg`, `Logo.png`), application scripts, and mock data[cite: 7, 8, 14, 16, 17, 18].
- **`vendors/`**: Houses all external libraries, frameworks, vendor fonts, and utility files—such as `normalize.css` and `grid.css`—ensuring dependencies remain isolated and clean[cite: 7, 9, 10, 16].

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
- **Hero Section Markup**: Structured a semantic `<header>` element containing a `.hero-text-box` with a primary headline (`<h1>`) and dual call-to-action anchor links[cite: 11].
- **Full-Screen Hero Background**: Applied `hero-image.jpg` as a responsive full-viewport background (`height: 100vh`) using `background-size: cover` and `background-position: center`[cite: 12].
- **Absolute Center Positioning**: Centered the `.hero-text-box` vertically and horizontally using `position: absolute`, `top: 50%`, `left: 50%`, and `transform: translate(-50%, -50%)` constrained to a `1140px` layout width[cite: 12].
- **Typography Transition**: Replaced initial fonts with the clean, versatile Google Font `Lato` (light weight 300) to establish an elegant modern aesthetic[cite: 11, 12].

### 📚 Lecture 4 Summary: Header Section - Part-2
- **Dark Gradient Overlay**: Layered a semi-transparent dark linear gradient (`linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7))`) over the hero background image to dramatically boost headline contrast and readability[cite: 14].
- **Headline Styling**: Formatted the `<h1>` with uppercase transformation, customized letter spacing (`1px`), word spacing (`3px`), white text color, and responsive font sizing (`240%`)[cite: 14].
- **Reusable Button Framework**: Configured a base `.btn` class with inline-block display, rounded corners (`border-radius: 10px`), and smooth property transition effects (`0.2s`)[cite: 14, 15].
- **Primary & Ghost Variants**: Developed `.btn-full` (solid orange background `#e67e22`) and `.btn-ghost` (transparent outline style) to establish clear call-to-action visual hierarchy[cite: 14, 15].
- **Interactive State Transitions**: Added `:hover` and `:active` pseudo-class states transitioning background and border colors smoothly to a deeper shade of orange (`#cf6d17`)[cite: 14].

### 📚 Lecture 5 Summary: Header Section - Part-3
- **Navigation Bar Layout**: Implemented a semantic `<nav>` bar inside the header wrapped in a `.row` container with a maximum width of `1140px` and centered alignment (`margin: 0 auto`)[cite: 16, 17].
- **Brand Identity Asset**: Added the brand logo image (`Logo.png`) into `resources/img/`, floated it to the left, and set a clean proportional height of `100px`[cite: 16, 17, 18].
- **Navigation Menu Alignment**: Floated `.main-nav` to the right with zero list markers and styled inline-block items with `40px` horizontal spacing[cite: 16, 17].
- **Animated Underline Hover State**: Styled uppercase anchor links with `padding: 8px 0px`, a transparent baseline border, and a smooth `0.2s` transition to a solid accent color (`border-bottom: 2px solid #e67e22`) on `:hover` and `:active`[cite: 17].

---

## 🛠️ Technologies Used

- **HTML5**: Semantic document structuring (`<header>`, `<nav>`, buttons, text wrappers).
- **CSS3**: Linear gradient overlays, transitions, button component design, float-based navigation, absolute positioning, and typography[cite: 17].
- **Normalize.css**: Cross-browser baseline normalization[cite: 16].
- **Responsive Grid System (`grid.css`)**: Lightweight fluid column framework[cite: 10, 16].
- **Google Fonts**: `Lato` web font family[cite: 16, 17].

---

## 📂 Project Structure

```text
Food Project/
├── resources/
│   ├── css/
│   │   ├── img/
│   │   │   └── hero-image.jpg
│   │   └── style.css
│   ├── data/
│   ├── img/
│   │   └── Logo.png
│   └── js/
├── vendors/
│   ├── css/
│   │   ├── grid.css
│   │   └── normalize.css
│   ├── fonts/
│   └── js/
└── index.html
