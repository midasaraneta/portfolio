# Midas Angelo Araneta — Portfolio

A modern, responsive personal portfolio website for **Midas Angelo Araneta**, a Software QA Engineer focused on manual testing, supported automation testing, web and mobile QA, API validation, database checks, CMS validation, defect management, and Agile delivery.

This version of the portfolio is organized using a separated front-end structure:

- `index.html` for page content and structure
- `css/style.css` for custom styling and animations
- `js/script.js` for interactivity and browser behavior
- `assets/` for images, logos, and resume files

---

## 🌐 Live Demo

```text
https://midasaraneta.github.io/portfolio/
```

---

## 📌 About the Project

This portfolio was built to present my professional background, technical skills, QA experience, certifications, publication, and contact information in a clean and interactive single-page website.

The project was originally built as one HTML file and later separated into dedicated HTML, CSS, and JavaScript files to make the codebase easier to maintain, debug, update, and deploy.

---

## ✨ Features

- Fully responsive portfolio layout
- Clean single-page website structure
- Dark and light mode toggle
- Mobile drawer navigation
- Sticky transparent navbar
- Animated loader screen
- Scroll progress indicator
- Desktop cursor glow effect
- Reveal-on-scroll animations
- Animated statistics counters
- Dynamic rotating professional title
- Interactive project category filtering
- Professional and freelance experience tabs
- Read More / Read Less content toggles
- Resume download button
- Contact form integration using FormSubmit
- GitHub Pages-ready deployment setup

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Website structure and content |
| CSS3 | Custom styling and animations |
| Tailwind CSS CDN | Utility-first styling and responsive layout |
| JavaScript | Interactivity and dynamic behavior |
| Font Awesome | Icons |
| Google Fonts | Typography |
| FormSubmit | Contact form handling |
| GitHub Pages | Static website hosting |

---

## 📂 Project Structure

```text
portfolio/
├── index.html
├── README.md
└── assets/
    ├── logo.png
    ├── profile.png
    ├── evoke-logo.png
    ├── kooapps-logo.png
    ├── upwork-logo.png
    ├── oreilly-logo.png
    └── Midas_Araneta_Resume.pdf
```

---

## 📄 File Responsibilities

### `index.html`

Contains the main website structure and content, including:

- Header and navigation
- Hero section
- About section
- Skills section
- Experience timeline
- Project showcase
- Publications
- Certifications
- Contact form
- Footer

It also includes external CDN links for Tailwind CSS, Google Fonts, and Font Awesome.

### `css/style.css`

Contains custom styling that is not handled directly by Tailwind utility classes, such as:

- Glassmorphism card styling
- Custom animations
- Loader animation
- Cursor glow effect
- Grid background
- Custom scrollbar
- Reveal animation styles
- Theme-specific custom styles

### `js/script.js`

Contains all portfolio interactivity, including:

- Loader behavior
- Navbar scroll behavior
- Back-to-top button
- Dark/light mode toggle
- Mobile drawer open and close behavior
- Active navigation highlighting
- Scroll reveal animations
- Statistics counter animation
- Dynamic title rotation
- Project filtering
- Contact form feedback
- Read More / Read Less toggles
- Professional and freelance experience tab switching

### `assets/`

Stores static files used by the website, including:

- Logo
- Profile image
- Company logos
- Certification logos
- Resume PDF

---

## 📖 Main Sections

### Home

Introduces the portfolio owner with a hero section, availability badge, social links, profile image, floating expertise badges, and resume button.

### About

Summarizes QA experience, professional background, key strengths, and focus areas.

### Skills & Tools

Displays technical skills grouped by category:

- Testing Types
- Tools & Platforms
- AI Tools & Productivity
- Code & Development
- Data Validation
- Management & Agile

### Experience

Uses a tab layout to switch between:

- Professional Experience
- Freelance Experience

### Projects

Includes an interactive project showcase with category filters:

- All
- Content Management System
- Web & Mobile
- API & Database
- QA Process
- Internship

### Publications

Highlights the academic research publication related to machine learning and controlled environment plant monitoring.

### Certifications

Displays professional certifications with verification links.

### Contact

Includes contact information and a contact form powered by FormSubmit.

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/midasaraneta/portfolio.git
```

### 2. Open the project folder

```bash
cd portfolio
```

### 3. Open the website locally

You can open `index.html` directly in your browser.

For a better development experience, use the **Live Server** extension in Visual Studio Code.

Example local URL:

```text
http://127.0.0.1:5500/index.html
```

---

## 🔗 Required File Links

Make sure these links exist in `index.html`:

```html
<link href="css/style.css" rel="stylesheet">
<script src="js/script.js" defer></script>
```

The `css/style.css` file should be inside the `css` folder.

The `js/script.js` file should be inside the `js` folder.

---

## ⚠️ GitHub Pages Asset Path Reminder

Use relative paths for assets:

```html
<img src="assets/logo.png" alt="Logo">
```

Avoid paths that start with `/`:

```html
<img src="/assets/logo.png" alt="Logo">
```

For GitHub Pages project sites, `/assets/logo.png` may break because it points to the domain root instead of the repository folder.

Correct:

```html
<link rel="icon" type="image/png" href="assets/logo.png">
```

Avoid:

```html
<link rel="icon" type="image/png" href="/assets/logo.png">
```

Also remember that GitHub Pages is case-sensitive. File names must match exactly.

Example:

```text
upwork-logo.png
```

is different from:

```text
UpWork-Logo.png
```

---

## 📤 Deployment

This project can be deployed using **GitHub Pages**.

### 1. Push changes to GitHub

```bash
git status
git add .
git commit -m "Update portfolio"
git push
```

### 2. Enable GitHub Pages

Go to your GitHub repository:

```text
Settings → Pages
```

Set the deployment source:

```text
Source: Deploy from a branch
Branch: main
Folder: /root
```

After saving, the portfolio will be published at:

```text
https://midasaraneta.github.io/portfolio/
```

GitHub Pages may take a few minutes to update.

---

## 🔄 Updating the Portfolio

After editing your HTML, CSS, JavaScript, images, or resume file, run:

```bash
git status
git add .
git commit -m "Describe your changes"
git push
```

Example:

```bash
git add .
git commit -m "Improve portfolio layout and separated file structure"
git push
```

---

## 🧪 Testing Checklist Before Pushing

Before pushing updates, check the following:

- Navigation links work correctly
- Mobile menu opens and closes
- Dark/light mode toggle works
- Resume button opens or downloads the resume
- Images and logos load correctly
- Project filters work
- Experience tabs switch correctly
- Read More / Read Less buttons work
- Contact form fields are visible
- Footer links display correctly
- No broken image paths
- No console errors in browser DevTools

---

## 🐞 Common Issues and Fixes

### CSS is not loading

Check this line in `index.html`:

```html
<link href="css/style.css" rel="stylesheet">
```

Make sure the file exists here:

```text
css/style.css
```

### JavaScript is not working

Check this line before the closing `</body>` tag or inside the `<head>` with `defer`:

```html
<script src="js/script.js" defer></script>
```

Make sure the file exists here:

```text
js/script.js
```

### Images are not showing on GitHub Pages

Use relative paths:

```html
<img src="assets/profile.png" alt="Profile">
```

Do not use:

```html
<img src="/assets/profile.png" alt="Profile">
```

### Resume button is not working

Check that the resume file exists in the assets folder:

```text
assets/Midas_Araneta_Resume.pdf
```

Then make sure the link uses:

```html
<a href="assets/Midas_Araneta_Resume.pdf" target="_blank" download>
```

### Git says everything is up to date

That means there are no new committed changes to push. Save your files first, then run:

```bash
git status
git add .
git commit -m "Update portfolio"
git push
```

---

## 📬 Contact

**Midas Angelo Araneta**  
Software QA Engineer | Dev QA Tester | Manual Tester

- LinkedIn: [linkedin.com/in/midasaraneta](https://www.linkedin.com/in/midasaraneta/)
- GitHub: [github.com/midasaraneta](https://github.com/midasaraneta/)
- Email: [midas.inquire@gmail.com](mailto:midas.inquire@gmail.com)

---

## 📄 License

This project is for personal portfolio use.

You may use this structure as a reference for your own portfolio, but please replace the content, images, resume, and personal details with your own information.
