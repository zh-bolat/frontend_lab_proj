# Assignment #1: HTML & CSS Basics

**Student:** Zhylgeldi Bolat  
**Group:** SE-2529  
**Theme:** Notion-inspired Monochrome Aesthetic (Black, Gray, White)

---

## 📌 Project Overview

This repository contains the complete implementation of **Assignment #1 (Tasks 1 through 4)** for the Web Development course at Astana IT University. The project is designed with a clean, modern, and minimalist aesthetic inspired by **Notion**, using a strict monochrome color palette (`#ffffff`, `#f7f7f5`, `#e9e9e7`, `#37352f`, `#2f3437`, `#000000`).

All pages include a unified top navigation bar linking seamlessly across all tasks.

---

## 📂 Project Structure

```text
├── index.html                   # Task 1: Personal Webpage & Profile Card
├── styles.css                   # Task 1 Stylesheet
├── profile.jpg                  # Profile photo (Zhylgeldi Bolat)
├── task2.html                   # Task 2: Pure Div & Float-based Layout (No Flexbox / Grid)
├── task2.css                    # Task 2 Stylesheet
├── exercise1/
│   ├── index.html               # Task 3: Tribute Page (Oleg Tinkov)
│   ├── styles.css               # Task 3 Stylesheet (Google Fonts, styling)
│   └── tinkov.jpg               # Portrait of Oleg Tinkov
├── task4.html                   # Task 4: Student Grades Table & Feedback Form
├── task4.css                    # Task 4 Stylesheet
└── README.md                    # Project documentation & instructions
```

---

## 🚀 Tasks Breakdown & Implementation Details

### Task 1: Introduction to HTML & CSS (`index.html`, `styles.css`)
- **Profile Card:** Includes personal photograph, name (*Zhylgeldi Bolat*), group (*SE-2529*), and a summary of DevOps / FinTech background (Vanessa Automation, OneScript, Docker, Kubernetes).
- **HTML Structure:** Structured with `<h1>`, `<h2>`, 3 descriptive paragraphs, an unordered list (`<ul>`) with 4 items, an ordered list (`<ol>`) with 4 sequential pipeline steps, an image with `alt`, and links (`<a>`).
- **CSS Selectors Demonstrated:**
  - **Element Selectors:** `body`, `h1`, `h2`, `p`, `a`, `ul`, `ol`, `li`.
  - **Class Selectors:** `.profile-card`, `.profile-image`, `.badge-link`, `.navbar`, etc.
  - **ID Selectors:** `#profile-section`, `#workflow-steps`.
- **CSS Styling:** Custom font stack (`Inter`), border radius, hover effects on links, clean spacing with margins/padding.

### Task 2: Webpage Layout using Floats & Positioning (`task2.html`, `task2.css`)
- **Strict Constraint:** Built exclusively using `<div>` elements, CSS floats, and positioning — **zero Flexbox and zero Grid**.
- **Layout Sections:**
  - **Header:** Site title and subtitle.
  - **Navigation Bar:** 4 navigation links styled using `display: inline-block` and hover effects.
  - **Sidebar Menu (Left):** Floated left (`float: left; width: 28%`) with navigation links.
  - **Main Content / Aside (Right):** Floated right (`float: right; width: 69%`) with headings and paragraphs.
  - **Clearfix:** Divider clearing floats (`clear: both;`) before the footer.
  - **Footer:** Bottom copyright bar.

### Task 3: Tribute Page (`exercise1/index.html`, `exercise1/styles.css`)
- **Subject:** Tribute to **Oleg Tinkov**, serial entrepreneur, founder of Tinkoff Bank (branchless digital banking pioneer), and founder of the Tinkov Family Foundation.
- **Boilerplate & Folder:** Standard HTML boilerplate placed in `exercise1/` directory.
- **HTML Content:**
  - `<h1>` main heading and `<h2>` "About Oleg Tinkov".
  - `<h3>` birth date and tagline.
  - 3 paragraphs summarizing his life, inventions, and fight against leukemia.
  - `<ol>` chronology of 5 milestone events (1992–2020).
  - `<ul>` list of 4 key inventions and contributions.
  - Portrait image (`<img>`) with descriptive `alt` attribute.
  - External links (`<a>`) to Forbes and Foundation + styled "Learn more" button (`.btn`) linking to Wikipedia.
- **CSS Styling:**
  - Subtle vertical background gradient.
  - Two Google Fonts linked in `<head>`: **Inter** (clean sans-serif for UI) and **Lora** (elegant serif for headings).
  - Styled `.content` container with `max-width` and `margin: 0 auto`.
  - Image styled with `max-width`, `border-radius`, and `box-shadow`.
  - Button hover effects with smooth transitions.

### Task 4: CSS Table and Form (`task4.html`, `task4.css`)
- **Part 1: Student Grades Table:**
  - 4 columns: *Student Name*, *Course / Subject*, *Score*, *Grade*.
  - Cell merging with both `rowspan` (merging multiple courses for a student) and `colspan` (cohort summary row).
  - Background color on table header (`th`).
  - Borders on all cells and centered cell text (`text-align: center`).
  - Alternate row striping using `tbody tr:nth-child(even)` and `tbody tr:nth-child(odd)`.
  - One highlighted row styled with `.highlight-row`.
  - ID selector `#grades-table-heading` applied to page heading.
- **Part 2: Feedback Form:**
  - Fields: Text input (name), email input (email), select dropdown (academic role), radio buttons (course recommendation), textarea (comments), and submit button.
  - Centered container (`#feedback-form-container`) with fixed `max-width: 520px`, padding, background, and rounded corners.
  - Bold text for labels (`font-weight: 700`).
  - Consistent dimensions and spacing for all inputs.
  - Submit button with hover background color transition and rounded corners.

---

## 🛠 How to Run Locally

You can open the project directly in any web browser without needing a backend server:

```bash
# Clone the repository
git clone <repository-url>
cd ass_final

# Open in browser (Linux)
xdg-open index.html

# Or start a lightweight local HTTP server
python3 -m http.server 8000
```
Then navigate to `http://localhost:8000` in your web browser.

---

## 🌐 Deployment to GitHub Pages

1. Push this repository to GitHub:
   ```bash
   git remote add origin https://github.com/zh-bolat/<repo-name>.git
   git branch -M main
   git push -u origin main
   ```
2. In the GitHub repository settings:
   - Navigate to **Settings** → **Pages**.
   - Under **Build and deployment** / **Source**, select `Deploy from a branch`.
   - Choose `main` branch and `/ (root)` folder, then click **Save**.
3. The site will be published at `https://zh-bolat.github.io/<repo-name>/`.
