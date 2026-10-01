# 🍽️ Food Project

A responsive food delivery and restaurant web application built with clean HTML5 and modern CSS3. This repository documents lecture-by-lecture progress, tracking foundational folder architecture, typography setup, responsive grid integration, semantic heading hierarchy, and full page section builds.

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

The **Food Project** demonstrates modular front-end web development practices. By maintaining a clean separation between third-party frameworks in `vendors/` and custom implementations in `resources/`, the project establishes a scalable, production-ready foundation for responsive design.

---

## 📁 Folder Architecture

The codebase separates custom code from external dependencies:

- **`resources/`**: Dedicated exclusively to custom assets and authored code, including stylesheets (`style.css`), media assets (`hero-image.jpg`, `Logo.png`, food showcase images, mobile mockups, and app store badges), application scripts, and mock data.
- **`vendors/`**: Houses all external libraries, frameworks, vendor fonts, and utility files—such as `normalize.css` and `grid.css`—ensuring dependencies remain isolated and clean.

---

## 📖 Course Progress & Lecture Summaries

### 📚 Lecture 1 Summary: Setting Up the Folder Structure
- **`resources/` Directory**: Houses your own custom assets and authored code (e.g., custom stylesheets `style.css`, project-specific images, client-side scripts, and local datasets).
- **`vendors/` Directory**: Houses all external, third-party libraries, frameworks, vendor fonts, and utility stylesheets such as `normalize.css` to keep dependencies cleanly separated from custom code.
- **CSS Reset & Normalization**: Incorporates `normalize.css` ahead of custom styles to ensure HTML elements render uniformly across different browsers before applying project-level resets.
- **Global Base Rules & Typography**: Sets universal `box-sizing: border-box`, standardizes font sizing, integrates Google Web Fonts, and enhances text legibility using `optimizeLegibility`.

### 📚 Lecture 2 Summary: Responsive Grid System
- **Grid System Integration**: Downloaded and added `grid.css` from the [Responsive Grid System](https://www.responsivegridsystem.co.uk/) into `vendors/css/` to establish a flexible, column-based layout foundation.
- **Fluid Proportional Columns**: Utilizes percentage-based fractional column classes spanning from 2 up to 12 columns (e.g., `.span_1_of_2`, `.span_1_of_3`, `.span_1_of_4`) alongside `.col` floats and margins.
- **Clearfix Self-Clearing**: Implements micro-clearfix rules (`.group:before`, `.group:after`) to ensure parent containers properly contain floated grid columns.
- **Mobile Fluidity**: Employs a `@media only screen and (max-width: 480px)` query that removes column margins and stacks all grid spans to 100% full width on mobile screens.
- **Layout Container Setup**: Introduced structural wrapper elements (`<div class="row">`) in `index.html` to center and constrain content rows.

### 📚 Lecture 3 Summary: Header Section - Part-1
- **Hero Section Markup**: Structured a semantic `<header>` element containing a `.hero-text-box` with a primary headline (`<h1>`) and dual call-to-action anchor links.
- **Full-Screen Hero Background**: Applied `hero-image.jpg` as a responsive full-viewport background (`height: 100vh`) using `background-size: cover` and `background-position: center`.
- **Absolute Center Positioning**: Centered the `.hero-text-box` vertically and horizontally using `position: absolute`, `top: 50%`, `left: 50%`, and `transform: translate(-50%, -50%)` constrained to a `1140px` layout width.
- **Typography Transition**: Replaced initial fonts with the clean, versatile Google Font `Lato` (light weight 300) to establish an elegant modern aesthetic.

### 📚 Lecture 4 Summary: Header Section - Part-2
- **Dark Gradient Overlay**: Layered a semi-transparent dark linear gradient (`linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7))`) over the hero background image to dramatically boost headline contrast and readability.
- **Headline Styling**: Formatted the `<h1>` with uppercase transformation, customized letter spacing (`1px`), word spacing (`3px`), white text color, and responsive font sizing (`240%`).
- **Reusable Button Framework**: Configured a base `.btn` class with inline-block display, rounded corners (`border-radius: 10px`), and smooth property transition effects (`0.2s`).
- **Primary & Ghost Variants**: Developed `.btn-full` (solid orange background `#e67e22`) and `.btn-ghost` (transparent outline style) to establish clear call-to-action visual hierarchy.
- **Interactive State Transitions**: Added `:hover` and `:active` pseudo-class states transitioning background and border colors smoothly to a deeper shade of orange (`#cf6d17`).

### 📚 Lecture 5 Summary: Header Section - Part-3
- **Navigation Bar Layout**: Implemented a semantic `<nav>` bar inside the header wrapped in a `.row` container with a maximum width of `1140px` and centered alignment (`margin: 0 auto`).
- **Brand Identity Asset**: Added the brand logo image (`Logo.png`) into `resources/img/`, floated it to the left, and set a clean proportional height of `100px`.
- **Navigation Menu Alignment**: Floated `.main-nav` to the right with zero list markers and styled inline-block items with `40px` horizontal spacing.
- **Animated Underline Hover State**: Styled uppercase anchor links with `padding: 8px 0px`, a transparent baseline border, and a smooth `0.2s` transition to a solid accent color (`border-bottom: 2px solid #e67e22`) on `:hover` and `:active`.

### 📚 Lecture 6 Summary: Feature section - Part-1
- **Semantic Heading Hierarchy**: Applied SEO and accessibility standards requiring exactly one `<h1>` per page (exclusive to the hero banner), transitioning to `<h2>` for section headings and `<h3>` for subheadings.
- **Feature Section Scaffolding**: Built `<section class="section-features">` featuring an introductory `.row` container with an `<h2>` heading and a descriptive `.long-copy` lead paragraph.
- **4-Column Grid Structure**: Implemented four equal columns using `.col.span_1_of_4` inside a `.row` to present key product selling points side-by-side.
- **Ionicons Integration**: Connected external vector icons via [Ionicons](https://ionic.io/ionicons) by embedding ES module and fallback scripts directly above the closing `</body>` tag.
- **Feature Component Assembly**: Paired individual columns with distinct outline icons (`infinite-outline`, `flash-outline`, `leaf-outline`, `cart-outline`), `<h3>` titles, and service detail text.

### 📚 Lecture 7 Summary: Feature section - Part-2
- **Section Vertical Rhythm**: Added `padding: 80px 0;` to section containers to establish spacious, clean separation between page segments.
- **Heading Underline Accent**: Styled `<h2>` headings and implemented a centered orange underline bar using the `h2::after` pseudo-element (`width: 100px`, `height: 2px`, `background-color: #e67e22`).
- **Lead Paragraph Layout**: Created the `.long-copy` utility class with `line-height: 145%`, constrained to `width: 70%` and centered with `margin-left: 15%` for optimal line length and readability.
- **Column Card Padding**: Added the `.box` class to the grid columns with `padding: 1%` to prevent inner text and icons from touching container edges.
- **Large Vector Icon Styling**: Styled `.icon-big` to render Ionicons at `font-size: 350%`, changed their display to `block`, tinted them with brand accent color `#e67e22`, and added a bottom margin.
- **Typography Balance**: Standardized `<h3>` subheadings with lightweight uppercase typography (`110%`) and refined column paragraph text with `90%` font sizing and `145%` line height.

### 📚 Lecture 8 Summary: Creating Favorite meal section - Part-1
- **Semantic `<figure>` Container**: Utilized the HTML5 `<figure class="meal-photo">` element to semantically encapsulate food images, establishing a dedicated container that groups visual media with its context or caption.
- **Meals Showcase Section Scaffolding**: Structured `<section class="section-meals">` containing two separate unordered lists (`.meals-showcase`) showcasing eight meal images (`1.jpg` through `8.jpg`) located in `resources/img/`.
- **Edge-to-Edge 4-Column Layout**: Styled `.meals-showcase` to span `width: 100%` and set list items to `float: left` with `width: 25%` to create an edge-to-edge four-column image grid across two rows.
- **Figure Margin Reset & Responsive Sizing**: Stripped default browser margins on `<figure>` (`margin: 0; width: 100%`) and applied `width: 100%; height: auto;` to `.meal-photo img` for fluid image scaling.

### 📚 Lecture 9 Summary: Creating Favorite meal section - Part-2
- **Overflow Clipping & Dark Backdrop**: Configured `overflow: hidden;` and `background-color: #000;` on the `.meal-photo` container to keep scaling images confined within their grid cells while creating a dark backdrop behind semi-transparent photos.
- **Default Image Zoom & Opacity**: Applied `transform: scale(1.15)` and `opacity: 0.7` to `.meal-photo img` so images start slightly enlarged with subdued brightness.
- **Interactive Hover Reveal**: Added an interactive hover state on `.meal-photo img:hover` that scales down slightly to `scale(1.03)` and brightens to `opacity: 1` with smooth transition timing.
- **Flush Edge-to-Edge Layout**: Applied `padding: 0;` to `.section-meals` to remove default section padding and allow the showcase to sit flush against surrounding page segments.
- **Content Spacing Refinement**: Adjusted spacing on `.long-copy` with a bottom margin of `30px` to create visual breathing room before feature cards.

### 📚 Lecture 10 Summary: Creating how it works section - Part-1
- **Section Architecture**: Created `<section class="section-steps">` featuring an `<h2>` heading row ("How it work — Simple as 1,2,3") to explain the service onboarding workflow.
- **Two-Column Split Layout**: Divided the section using `.col.span_1_of_2 steps-box` containers from the responsive grid system to balance mobile visuals on the left and instructions on the right.
- **Phone Mockup Visual**: Embedded a smartphone application mockup graphic (`Phone.png`) inside the left column to provide a mobile app preview.
- **Numbered Step Workflow**: Structured three sequential `.works-step` containers in the right column, pairing numeric step badges (`1`, `2`, `3`) with clear sign-up, ordering, and delivery directions.
- **App Store Badges**: Added mobile application call-to-action links (`.btn-app`) incorporating official badges for Google Play (`playstore.png`) and the Apple App Store (`appstore.png`).

### 📚 Lecture 11 Summary: Creating how it works section - Part-2
- **Circular Step Number Badges**: Styled the numeric step badges (`.works-step div`) as rounded circular elements using `border: 4px solid #e67e22`, `border-radius: 50%`, fixed dimensions (`55px × 55px`), and `float: left` so text lines up neatly beside them.
- **Micro-Clearfix Utility**: Implemented a reusable `.clearfix` utility with `zoom: 1` and `::after` clearing pseudo-element applied to `.meals-showcase` to contain floated image items properly.
- **Column Balance & Alignment**: Sized `.app-screen` to `52%` width with centered alignment and asymmetric column padding (`padding-right: 3%` on the phone column and `padding-left: 3%` on the instructions column) for visual balance.
- **Vertical Step Rhythm**: Added `margin-bottom: 50px` to `.works-step` elements, extending the final step's margin with `:last-of-type` to `80px` before the app download buttons.
- **Section Contrast Styling**: Gave `.section-steps` an off-white background (`background-color: #f4f4f4`) and `overflow: hidden` to visually delineate the steps section from the meals gallery.
- **App Store Button Sizing**: Styled `.btn-app img` with fixed height (`150px`), automatic aspect ratio width, and horizontal spacing.

---

## 🛠️ Technologies Used

- **HTML5**: Semantic document structuring (`<header>`, `<nav>`, `<section>`, `<figure>`, `<ul>`, `<script>`).
- **CSS3**: Image transform scaling, opacity transitions, linear gradient overlays, pseudo-elements (`::after`), micro-clearfix pattern, button component design, float layouts, and typography.
- **Normalize.css**: Cross-browser baseline normalization.
- **Responsive Grid System (`grid.css`)**: Lightweight fluid column framework.
- **Google Fonts**: `Lato` web font family.
- **Ionicons**: Modern open-source icon pack loaded via script modules.

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
│   │   ├── 1.jpg
│   │   ├── 2.jpg
│   │   ├── 3.jpg
│   │   ├── 4.jpg
│   │   ├── 5.jpg
│   │   ├── 6.jpg
│   │   ├── 7.jpg
│   │   ├── 8.jpg
│   │   ├── appstore.png
│   │   ├── Logo.png
│   │   ├── Phone.png
│   │   └── playstore.png
│   └── js/
├── vendors/
│   ├── css/
│   │   ├── grid.css
│   │   └── normalize.css
│   ├── fonts/
│   └── js/
└── index.html
