# 🍽️ Food Project

A responsive food delivery and restaurant web application built with clean HTML5 and modern CSS3. This repository documents lecture-by-lecture progress, tracking foundational folder architecture, typography setup, responsive grid integration, semantic heading hierarchy, full page section builds, and comprehensive multi-device responsive media queries.

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

- **`resources/`**: Dedicated exclusively to custom assets and authored code, including stylesheets (`style.css`), media queries (`queries.css`), background banners (`hero-image.jpg`, `back-cust.jpg`), brand media (`Logo.png`), food gallery photos, mobile mockups, app badges, city photography, and customer review avatars.
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
- **Ionicons Integration**: Connected external vector icons via Ionicons by embedding ES module and fallback scripts directly above the closing `</body>` tag.
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

### 📚 Lecture 12 Summary: Creating the city section - Part-1
- **City Section Scaffolding**: Built `<section class="section-cities">` featuring a centered `<h2>` heading ("We're currently in these cities") to showcase available service locations.
- **4-Column Geographic Grid**: Used the responsive grid system (`.col.span_1_of_4.box`) inside a `.row` to display cards for Lisbon, San Francisco, Berlin, and London side-by-side.
- **Location Visual Assets**: Embedded city photography (`lisbon.jpg`, `san-francisco.jpg`, `berlin.jpg`, `london.jpg`) in `resources/img/` to anchor each city showcase card.
- **City Metadata Structure**: Structured city feature rows below each `<h3>` city title, organizing operational statistics like active eater counts, star chefs, and Twitter handles with icon placeholders.

### 📚 Lecture 13 Summary: Creating the city section - Part-2
- **Responsive City Card Images**: Styled `.box img` with `width: 100%`, `height: auto`, and `margin-bottom: 15px` to keep location photography fully responsive and separated from headings.
- **City Metadata Spacing**: Added `.city-feature` with `margin-bottom: 5px` to establish consistent vertical rhythm between city stats (eater count, chef count, and social handle).
- **Small Vector Icon Alignment**: Configured `.icon-small` with `display: inline-block`, fixed `width: 30px`, center text alignment, brand accent `#e67e22`, and subtle vertical shifting (`vertical-align: middle; margin-top: -5px; margin-right: 10px`) to align icons with adjacent text.
- **Global Text Link Styling**: Implemented styled anchor links (`a:link`, `a:visited`) with `#e67e22` color and a subtle bottom border (`border-bottom: 1px solid #e67e22`), transitioning smoothly over `0.5s` to dark gray (`#555`) with a transparent border on `:hover` and `:active`.
- **App Badge Border Reset**: Added a border reset (`border: 0;`) specifically for `.btn-app` links to ensure mobile store badge images do not inherit the default text link underline.

### 📚 Lecture 14 Summary: Creating Customer testimonial section - Part-1
- **Semantic Quotation Elements**: Introduced semantic HTML5 `<blockquote>` elements to encapsulate customer feedback, pairing each testimonial with a `<cite>` tag to attribute the customer name and avatar photo.
- **3-Column Testimonial Layout**: Implemented `.col.span_1_of_3` column wrappers from the responsive grid system to align three customer review cards side-by-side within a `.row` container.
- **Customer Profile Assets**: Integrated customer headshots (`cust-1.jpg`, `cust-2.jpg`, `cust-3.jpg`) inside `resources/img/` as avatars within the `<cite>` author tag.
- **Social Proof Section Structure**: Scaffolded `<section class="section-testimonials">` with an `<h2>` heading row ("Our customers can't live without us") to build trust and social proof on the landing page.

### 📚 Lecture 15 Summary: Creating Customer testimonial section - Part-2
- **Parallax Scrolling Effects**: Applied `background-attachment: fixed` to both `<header>` and `.section-testimonials`, producing a modern parallax scrolling effect as elements slide over the fixed images.
- **Darkened Testimonial Background**: Positioned `back-cust.jpg` behind `.section-testimonials` under a semi-transparent dark overlay (`linear-gradient(rgba(0,0,0,0.8), rgba(0,0,0,0.8))`) with `color: #fff` for sharp typographic contrast.
- **Decorative Giant Quotation Marks**: Integrated large opening quote marks above every quote via `blockquote::before` (`content: '\201C'`, `font-size: 500%`, `position: absolute`, `top: 0`, `left: -5px`).
- **Blockquote Typographic Styling**: Enhanced quote text using `font-style: italic`, spacious line height (`145%`), `padding: 2%`, and `position: relative` to anchor the quote mark glyph.
- **Circular Author Avatars**: Rendered profile headshots with circular borders (`border-radius: 50%`, `height: 45px`) and `vertical-align: middle` beside author names.
- **Container Clearfix Fix**: Implemented a clearing fix on `.row::after` (`content: ""; display: table; clear: both;`) to reliably prevent parent layout collapse around floated columns.

### 📚 Lecture 16 Summary: Creating Sign up section - Part-1
- **Pricing Plans Section Scaffolding**: Scaffolded `<section class="section-plans">` accompanied by an `<h2>` heading ("Start eating healthy today") to introduce tiered subscription packages.
- **3-Tier Responsive Layout**: Utilized `.col.span_1_of_3` column wrappers from the responsive grid system to arrange three subscription cards side-by-side within a `.row` container.
- **Card Container Structure (`.plan-box`)**: Segmented each `.plan-box` into three structural `<div>` blocks separating the plan header/pricing, the feature checklist (`<ul>`), and the signup button.
- **Feature Inclusion Indicators**: Utilized Ionicons (`checkmark-outline` and `close-outline`) within the feature lists to visually indicate perk availability across different tiers.
- **Visual CTA Hierarchy**: Assigned the high-contrast solid button (`.btn-full`) to the recommended Premium plan while styling the Pro and Starter options with the secondary outline button (`.btn-ghost`).

### 📚 Lecture 17 Summary: Creating Sign up section - Part-2
- **Pricing Card Visual Architecture**: Styled `.section-plans` with a contrasting light background (`#f4f4f4`) and shaped `.plan-box` into clean white cards (`width: 90%; margin-left: 5%; border-radius: 5px`) with subtle partition dividers (`border-bottom: 1px solid #e8e8e8`).
- **Card Header Distinction**: Tinted the first block (`.plan-box div:first-child`) with an off-white backdrop (`#fcfcfc`) and matching rounded top corners to emphasize pricing headers.
- **Proportional Price Typography**: Enlarged `.plan-price` numbers to `300%` in an ultra-light weight (`font-weight: 100`) tinted with orange (`#e67e22`), while scaling down frequency tags (`<span>/ month</span>`) to `30%` size.
- **Feature List Polish & Icon Alignment**: Cleared list decorations (`list-style: none`), added vertical padding (`5px 0`) per feature, and aligned checkmarks and crosses using `.icon-small`.
- **Feature Strikethrough Indicator**: Created the `.not-available` helper class with `text-decoration: line-through` to denote features excluded from lower-tier plans.
- **Action Footer Alignment**: Formatted `.plan-box div:last-child` with `border: 0` and `text-align: center` to center-align the call-to-action buttons.

### 📚 Lecture 18 Summary: Creating the contact form section - Part-1
- **Contact Section Scaffolding**: Built `<section class="section-form">` containing a centered `<h2>` heading ("We're happy to hear from you") to introduce the user feedback and inquiry area.
- **Form Grid Integration**: Embedded grid `.row` containers inside `<form action="#" method="post">`, dividing each row into `.col.span_1_of_3` for descriptive `<label>` tags and `.col.span_2_of_3` for input controls to ensure alignment across devices.
- **Diverse HTML5 Form Controls**: Integrated standard form elements including text inputs (`type="text" placeholder="Your Name" required`), email inputs (`type="email" placeholder="Your Email" required`), a `<select>` dropdown menu with option tags, a pre-selected newsletter checkbox (`checked`), and a multi-line `<textarea>`.
- **Form Submission Layout**: Configured a submit button row using an empty non-breaking space label (`&nbsp;`) in the left column to align the `<input type="submit" value="Send Me">` element with the rest of the form fields.

### 📚 Lecture 19 Summary: Creating the contact form section - Part-2
- **Form Centering & Width**: Applied the `.contact-form` class to `<form>` with `width: 60%` and `margin: 0 auto` to restrict the form container to an optimal reading width centered within the section.
- **Standardized Form Control Styling**: Styled `input[type="text"]`, `input[type="email"]`, `<select>`, and `<textarea>` with unified full widths (`width: 100%`), consistent padding (`7px`), subtle gray borders (`1px solid #ccc`), and soft rounded corners (`border-radius: 3px`).
- **Checkbox Margin Alignment**: Sized and spaced `input[type="checkbox"]` using `margin: 10px 5px 10px 0` to ensure balanced alignment alongside the newsletter label text.
- **Shared Submit Button System**: Extended the `.btn` and `.btn-full` button rules directly to `input[type="submit"]`, inheriting the identical padding, orange brand colors (`#e67e22`), hover transitions (`#cf6d17`), and borders without code duplication.

### 📚 Lecture 20 Summary: Creating the footer section - Part-1
- **Semantic Footer Scaffolding**: Added a semantic `<footer>` container at the base of the page to organize secondary navigation, social links, and copyright text.
- **Dual-Column Footer Grid**: Implemented a two-column row using `.col.span_1_of_2` from the responsive grid system to position footer navigation links on the left and social channels on the right.
- **Footer Navigation List**: Structured an unordered list (`.footer-nav`) providing accessible anchor links to corporate pages including About Us, Blog, Press, and iOS/Android app downloads.
- **Social Network Channel Setup**: Integrated an unordered list (`.social-links`) containing brand Ionicons (`logo-facebook`, `logo-x`, `logo-google`, `logo-instagram`) to represent brand social channels.
- **Copyright Attribution Row**: Appended a secondary centered `.row` housing legal and copyright notice text (`&copy; 2015 by omnifood.All rights reserved`).

### 📚 Lecture 21 Summary: Creating the footer section - Part-2
- **Dark Footer Theme & Padding**: Styled `footer` with an elegant dark slate background (`#333`), scaled base font sizing (`80%`), and generous `50px` inner padding for clear separation.
- **Horizontal List Alignment & Floats**: Floated `.footer-nav` to the left and `.social-links` to the right, arranging list items inline (`display: inline-block`) with `20px` right margins.
- **Subtle Footer Link Typography**: Neutralized footer text links with dimmed gray coloring (`#888`), removed default anchor underline borders (`border: 0`), and transitioned smoothly to light gray (`#ddd`) on `:hover`.
- **Brand-Specific Social Hover States**: Configured authentic brand accent hover colors across all social network icons—Facebook (`#3b5998`), X (`white`), Google (`#dd4b39`), and Instagram (`#517fa4`).
- **Centered Copyright Notice**: Formatted legal copyright text (`footer p`) with centered text alignment, muted tone (`#888`), compact sizing (`90%`), and a top margin of `20px`.

### 📚 Lecture 22 Summary: Making webpage responsive - Part-1
- **Viewport Meta Configuration**: Embedded `<meta name="viewport" content="width=device-width, initial-scale=1.0">` into `index.html` to instruct mobile browsers to render at native device widths without artificial scaling.
- **Modular Queries Architecture**: Created `resources/css/queries.css` and linked it directly after `style.css` to manage responsive breakpoints independently while maintaining cascading order.
- **Horizontal Overflow Guard**: Applied `overflow-x: hidden;` to `html` and `body` in `style.css` to eliminate horizontal scroll glitches across narrowing viewport widths.
- **Desktop & Large Tablet Breakpoint (`max-width: 1200px`)**: Expanded `.hero-text-box` to `width: 100%` and added `2%` horizontal padding across `.row` containers and hero text to prevent clipping against screen borders.
- **Tablet Landscape Breakpoint (`max-width: 1023px`)**: Scaled base typography down to `18px`, tightened vertical spacing across all `section` elements to `60px 0`, and broadened `.long-copy` width to `80%` (`margin-left: 10%`) for better mobile readability.

### 📚 Lecture 23 Summary: Making webpage responsive - Part-2
- **Tablet Refinement Breakpoint (`max-width: 1023px`)**: Fine-tuned component proportions for landscape tablets by scaling down small icons (`.icon-small` to `17px`), expanding `.plan-box` to `100%` width, enlarging `.contact-form` to `80%` width, and adjusting vertical step margins.
- **Mobile Column Stacking Breakpoint (`max-width: 767px`)**: Transformed multi-column grids into single full-width stacks (`.col { width: 100%; margin: 0 0 4% 0; }`), reduced root font sizing to `16px`, tightened section padding to `30px 0`, and hid desktop navigation (`.main-nav { display: none; }`).
- **Mobile Steps & Step Badges**: Scaled numeric circular step counters down to `40px × 40px`, reduced step margins to `20px`, and constrained mobile app screen previews to `40%` width with centered alignment.
- **Float Containment Polish**: Added `overflow: hidden;` to `.works-step` in `style.css` to reliably clear floated circular step badges within compact mobile containers.
- **Small Smartphone Breakpoint (`max-width: 480px`)**: Expanded `.contact-form` to span `100%` full width and compressed section padding down to `25px 0` for compact handheld displays.

---

## 🛠️ Technologies Used

- **HTML5**: Semantic document structuring (`<header>`, `<nav>`, `<section>`, `<figure>`, `<blockquote>`, `<cite>`, `<form>`, `<input>`, `<select>`, `<textarea>`, `<footer>`, `<ul>`, `<script>`).
- **CSS3**: Parallax background attachment (`fixed`), gradient overlays, pseudo-elements (`::before`, `::after`), micro-clearfix patterns, form field normalization, brand hover transitions, and responsive typography.
- **Responsive Web Design**: Viewport meta tag configuration and custom media query breakpoints (`queries.css`).
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
│   │   │   ├── back-cust.jpg
│   │   │   └── hero-image.jpg
│   │   ├── queries.css
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
│   │   ├── berlin.jpg
│   │   ├── cust-1.jpg
│   │   ├── cust-2.jpg
│   │   ├── cust-3.jpg
│   │   ├── lisbon.jpg
│   │   ├── Logo.png
│   │   ├── london.jpg
│   │   ├── Phone.png
│   │   ├── playstore.png
│   │   └── san-francisco.jpg
│   └── js/
├── vendors/
│   ├── css/
│   │   ├── grid.css
│   │   └── normalize.css
│   ├── fonts/
│   └── js/
└── index.html
