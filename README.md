# Assignment #1: HTML & CSS Basics

**Student:** Zhylgeldi Bolat  
**Group:** SE-2529  
**Theme:** Notion-inspired Monochrome Aesthetic (Black, Gray, White)

---

## 📌 Project Overview

This repository contains the complete, modular implementation of **Assignment #1 (Tasks 1 through 4)** for the Web Development course at Astana IT University. 

The project is designed with a clean, modern, and minimalist aesthetic inspired by **Notion**, using a strict monochrome palette (`#ffffff`, `#f7f7f5`, `#e9e9e7`, `#37352f`, `#2f3437`, `#000000`).

Every task is isolated in its own dedicated directory with organized stylesheets and assets, accessible via an interactive Notion-style dashboard on the main page and unified cross-task navigation bars.

---

## 📂 Project Structure

```text
frontend_lab_proj/
├── index.html                   # Main Notion Dashboard Hub & Task Launcher
├── styles.css                   # Hub Stylesheet
├── README.md                    # Project Documentation
├── assets/
│   └── images/
│       ├── profile.jpg          # Profile photo (Zhylgeldi Bolat)
│       └── tinkov.jpg           # Portrait of Oleg Tinkov
├── docs/
│   ├── assignment1_frontend.docx # Original Assignment Specification
│   └── notion_reference.png     # Notion visual design reference
├── task1/
│   ├── index.html               # Task 1: Personal Webpage & Profile Card
│   └── styles.css               # Task 1 Stylesheet (Selectors, Notion styles)
├── task2/
│   ├── index.html               # Task 2: Pure Div & Float Layout (No Flex/Grid)
│   └── styles.css               # Task 2 Stylesheet (Float columns, positioning)
├── exercise1/                   # Task 3: Tribute Page (Named exercise1 per spec)
│   ├── index.html               # Task 3: Tribute to Oleg Tinkov
│   ├── styles.css               # Task 3 Stylesheet (Google Fonts, gradients)
│   └── tinkov.jpg               # Portrait asset
└── task4/
    ├── index.html               # Task 4: Student Grades Table & Feedback Form
    └── styles.css               # Task 4 Stylesheet (Table nth-child, form styles)
```

---

## 🚀 Tasks Breakdown & Implementation Details

### 🏠 Home Dashboard (`index.html`, `styles.css`)
- Serves as the central entry point for GitHub Pages.
- Styled like a Notion workspace dashboard featuring the student profile, callout box, and interactive task cards with direct links to all tasks.

### 👤 Task 1: Introduction to HTML & CSS (`task1/`)
- **Profile Card:** Personal photograph, student name (*Zhylgeldi Bolat*), group (*SE-2529*), and DevOps/FinTech bio.
- **HTML Content:** Headings (`<h1>`, `<h2>`), 3 paragraphs, an unordered list (`<ul>`) with 4 core skills, an ordered list (`<ol>`) with 4 deployment steps, and social/contact links.
- **CSS Selectors Demonstrated:**
  - **Element Selectors:** `body`, `h1`, `h2`, `p`, `a`, `ul`, `ol`, `li`.
  - **Class Selectors:** `.profile-card`, `.profile-image`, `.badge-link`, `.navbar`.
  - **ID Selectors:** `#profile-section`, `#workflow-steps`.
- **CSS Styling:** Custom typography (`Inter`), margins, padding, image borders and radius, link hover effects.

### 📐 Task 2: Webpage Layout with Floats & Positioning (`task2/`)
- **Strict Constraint:** Built exclusively using `<div>` elements and CSS positioning/floats — **no Flexbox and no Grid**.
- **Layout Sections:**
  - **Header:** Website title and student info.
  - **Navigation Bar:** 4 navigation links styled via `display: inline-block` and hover states.
  - **Sidebar Menu (Left):** Floated left (`float: left; width: 28%`) with a list of navigation anchors.
  - **Main Content / Aside (Right):** Floated right (`float: right; width: 69%`) with headings and technical paragraphs.
  - **Clearfix:** Divider clearing floats (`clear: both;`) before the footer.
  - **Footer:** Bottom copyright bar.

### 🎖️ Task 3: Tribute Page — Oleg Tinkov (`exercise1/`)
- **Subject:** Tribute to **Oleg Tinkov**, serial entrepreneur and founder of Tinkoff Bank (first 100% branchless cloud bank in Eastern Europe).
- **Directory:** Placed inside `exercise1/` with its own `index.html` and `styles.css` as strictly requested by the assignment.
- **HTML Content:**
  - Headings: `<h1>` (Title), `<h2>` ("About Oleg Tinkov"), `<h3>` (Birth date & tagline).
  - 3 paragraphs summarizing his life, ventures, and fight against leukemia.
  - `<ol>` list of 5 key timeline milestones (1992–2020).
  - `<ul>` list of 4 major inventions and contributions.
  - Portrait (`<img>`) with descriptive `alt` attribute.
  - External links to Forbes and Foundation + styled "Learn more" button (`.btn`) to Wikipedia.
- **CSS Styling:**
  - Monochrome vertical gradient background.
  - Two Google Fonts linked in `<head>`: **Inter** (sans-serif) and **Lora** (serif).
  - Styled `.content` container (`max-width`, `margin: 0 auto`).
  - Image styled with `max-width`, `border-radius`, and `box-shadow`.

### 📊 Task 4: CSS Table and Form (`task4/`)
- **Part 1: Student Grades Table:**
  - 4 columns: *Student Name*, *Course / Subject*, *Score*, *Grade*.
  - Cell merging with both `rowspan` (merging student across multiple subjects) and `colspan` (cohort average summary row).
  - Background color on table header (`th`).
  - Borders on all cells and centered cell text (`text-align: center`).
  - Alternate row striping using `tbody tr:nth-child(even)` and `tbody tr:nth-child(odd)`.
  - Highlighted row styled with custom class `.highlight-row`.
  - Page heading styled with ID selector `#grades-table-heading`.
- **Part 2: Course Feedback Form:**
  - Fields: Text input (Name), email input (Email), select dropdown (Academic role), radio buttons (Recommendation), textarea (Comments), and submit button.
  - Centered fixed-width container (`#feedback-form-container`, `max-width: 520px`) with background, padding, and rounded corners.
  - Bold text for labels (`font-weight: 700`).
  - Consistent width and spacing across inputs, select, and textarea.
  - Styled submit button with hover transition and rounded corners.

---

## 🛠 Local Testing

Open `index.html` in your browser or run:

```bash
# Start a simple HTTP server
python3 -m http.server 8000
```
Then open `http://localhost:8000`.

---

## 🌐 GitHub Pages Deployment

1. Push to your repository:
   ```bash
   git push -u origin main
   ```
2. In your GitHub repository:
   - Go to **Settings** → **Pages**.
   - Under **Branch**, select `main` and `/ (root)`, then click **Save**.
3. Access the site via: `https://zh-bolat.github.io/frontend_lab_proj/`
