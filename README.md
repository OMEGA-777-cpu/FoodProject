# 🍽️ Food Project

A responsive food delivery and restaurant web application built with clean HTML5 and CSS3. This repository documents lecture-by-lecture progress, starting from foundational directory structuring and typography resets to building out full page layouts.

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

The **Food Project** demonstrates modern web layout techniques and maintainable front-end code organization. Third-party dependencies are strictly separated from custom source code to ensure clear separation of concerns and easier scalability.

---

## 📁 Folder Architecture

The project structure is organized around two primary folders:

- **`resources/`**: Houses all custom, author-created assets and code, including project stylesheets (`style.css`), original images, mock data, and application scripts[cite: 7, 8].
- **`vendors/`**: Houses external libraries, vendor fonts, utility frameworks, and pre-built stylesheets like `normalize.css` to prevent third-party code from mixing with custom implementation.

---

## 📖 Course Progress & Lecture Summaries

### 📚 Lecture 1 Summary: Setting Up the Folder Structure
- **`resources/` Directory**: Houses your own custom assets and authored code (e.g., custom stylesheets `style.css`, project-specific images, client-side scripts, and local datasets)[cite: 7, 8].
- **`vendors/` Directory**: Houses all external, third-party libraries, frameworks, vendor fonts, and utility stylesheets such as `normalize.css` to keep dependencies cleanly separated from custom code[cite: 7].
- **CSS Reset & Normalization**: Incorporates `normalize.css` ahead of custom styles to ensure HTML elements render uniformly across different browsers before applying project-level resets[cite: 7, 8].
- **Global Base Rules & Typography**: Sets universal `box-sizing: border-box`, standardizes font sizing, integrates Google Web Fonts, and enhances text legibility using `optimizeLegibility`[cite: 7, 8].

---

## 🛠️ Technologies Used

- **HTML5**: Semantic markup[cite: 7].
- **CSS3**: Global resets, typography rules, and custom styles[cite: 8].
- **Normalize.css**: Cross-browser styling normalization[cite: 7].
- **Google Fonts**: `Bitcount Single` and `Nova Round` web fonts[cite: 7, 8].

---

## 📂 Project Structure

```text
Food Project/
├── resources/
│   ├── css/
│   │   ├── img/
│   │   └── style.css
│   ├── data/
│   ├── img/
│   └── js/
├── vendors/
│   ├── css/
│   │   └── normalize.css
│   ├── fonts/
│   └── js/
└── index.html
