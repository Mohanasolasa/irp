# IRP LMS — Educational Learning Management System Recreation

A pixel-perfect, fully responsive recreation of the official **IRP LMS** platform website built strictly using fundamental **HTML5** and **CSS3**.

---

## 🚀 Live Preview & Quick Start

### Opening in VS Code / Local Browser
No build tools, bundlers, or package managers are required.

1. **Directly in Browser:**
   - Double-click `index.html` to open the Home page in any modern web browser.
   - Alternatively, open with VS Code and use the **Live Server** extension (`Go Live`).
2. **Multi-page Navigation:**
   - `index.html` → Home Page
   - `courses.html` → Courses Page (9 Video Tutorials)
   - `contact.html` → Contact Us Page (Contact Details & Message Form)

---

## 🛠️ Technology Stack

This project strictly adheres to fundamental web standards without external libraries:

- **HTML5**: Semantic tags (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`, `<form>`, `<input>`, `<select>`, `<textarea>`, `<button>`).
- **CSS3**: Modern layouts using **CSS Flexbox** and **CSS Grid**, custom properties (CSS variables), responsive media queries, and smooth micro-interactions.
- ❌ **No JavaScript**: 100% pure HTML & CSS as per project specification.
- ❌ **No Frameworks**: No Bootstrap, Tailwind CSS, React, Angular, or Vue.
- ❌ **No Backend/Database**: Pure frontend presentation.

---

## 🎨 Design System & CSS Variables

The website strictly follows the official IRP LMS color tokens defined in `style.css`:

```css
:root {
  --primary-navy: #003366;       /* Primary brand headings and titles */
  --primary-orange: #FE781E;     /* Call-to-action buttons, badges, active accents */
  --secondary-blue: #5F9FE0;     /* Supporting badges, focus rings, hover borders */
  --light-blue-bg: #E2F2FD;      /* Hero sections and info panel backgrounds */
  --white: #FFFFFF;              /* Card backgrounds, base canvas */
  --light-blue-border: #D6E9FF;  /* Card outlines and section dividers */
}
```

---

## 📁 Project Structure

```text
irp-lms/
│
├── index.html      # Home Page (Hero + 5-step Learning Journey)
├── courses.html    # Courses Page (Hero + 9 YouTube Video Embeds + Explore Banner)
├── contact.html    # Contact Page (Hero + Info Panel + Contact Form)
├── style.css       # Unified, modular CSS stylesheet
└── README.md       # Project documentation and specifications
```

---

## 📄 Page Breakdown & Features

### 1. Navigation Bar (Reusable Component)
- **Left:** Graduation Cap Logo (`irp_lms_navbar_icon_rc0f9k.png`) alongside bold navy **IRP LMS** branding.
- **Center:** Navigation links (`Home`, `Courses`, `Contact Us`).
- **Active State:** Orange text color and solid orange bottom underline (`var(--primary-orange)`).
- **Right:** Orange outlined **Sign In** button with hover transition (visual only).
- **Mobile Responsive:** Seamlessly stacks and wraps on tablet and mobile viewports with zero horizontal scrolling.

---

### 2. Home Page (`index.html`)
- **Hero Section:**
  - Badge: `LEARN • BUILD • GET PLACED`
  - Headline: `Welcome to IRP LMS Platform` with **"IRP LMS"** highlighted in orange.
  - Subtitle: *"Your step-by-step learning journey to build skills, gain confidence and get placed in your dream job."*
  - CTA Button: `Explore Courses →` linking to `courses.html`.
  - Artwork: High-resolution *"Climbing Towards Success"* illustration.
  - Container: Rounded light-blue container (`var(--light-blue-bg)` with `var(--light-blue-border)`).
- **Your Learning Journey Section:**
  - Subtitle: *"Follow these steps to build your skills and get ready for placement."*
  - Five step cards arranged in **5 columns on desktop**:
    1. **Learn:** Take structured courses and build concepts.
    2. **Practice:** Solve problems and improve your skills.
    3. **Build Projects:** Work on real-world projects for your portfolio.
    4. **Prepare:** Get interview ready with mock sessions and guidance.
    5. **Get Placed:** Apply to drives and achieve your career goals.
  - White card background, rounded corners, light blue border, and circular orange step counters.

---

### 3. Courses Page (`courses.html`)
- **Hero Section:**
  - Category: `OUR COURSES`
  - Headline: `Learn by Watching Video Tutorials` with **"Video Tutorials"** in orange.
  - Description: *"Watch high-quality video tutorials and learn new skills at your own pace."*
  - Artwork: Minimalist E-learning banner with graduation cap.
- **Video Tutorial Grid (9 Courses):**
  - Responsive Grid: **4 cards per row on desktop**, 2 per row on tablet, 1 per row on mobile.
  - Aspect ratio: `16:9` responsive video containers (`aspect-ratio: 16 / 9`).
  - Embedded YouTube tutorials:
    1. **HTML Crash Course:** Learn HTML fundamentals and build your first webpage.
    2. **CSS Crash Course:** Master styling, layouts, and responsive web design.
    3. **JavaScript Crash Course:** Learn JavaScript fundamentals and client-side interactivity.
    4. **React Crash Course:** Learn component-based UI development using React.
    5. **Python Crash Course:** Understand Python programming fundamentals.
    6. **Java Crash Course:** Learn Java and object-oriented programming.
    7. **Spring Boot Crash Course:** Build REST APIs and backend applications using Spring Boot.
    8. **Hibernate Crash Course:** Learn Java ORM and database persistence.
    9. **Django Crash Course:** Build Python web applications using Django.
- **Explore More Courses Banner:**
  - Light blue card with 9-dot grid SVG icon.
  - Title: *"Explore More Courses"*
  - Description: *"Discover more courses and expand your skills with our learning resources."*
  - CTA Button: `View All Courses →`

---

### 4. Contact Page (`contact.html`)
- **Hero Section:**
  - Category: `GET IN TOUCH`
  - Headline: `Contact Us` with **"Us"** in orange.
  - Description: *"We're here to help! Whether you have a question, feedback, or just want to say hello — reach out to us."*
  - Artwork: Minimalist E-learning banner.
- **Two-Column Contact Layout:**
  - **Left: Contact Information Panel** (Light Blue Background)
    - Heading: `Get in Touch`
    - Subtitle: *"We'd love to hear from you! Fill out the form and our team will get back to you as soon as possible."*
    - Orange subheadings with SVG icons:
      - **Email Us:** `support@irplms.com` (clickable `mailto:` link)
      - **Call Us:** `+91 98765 43210` (clickable `tel:` link)
      - **Our Office:** `123, Tech Park, 2nd Floor, Bangalore, Karnataka – 560001`
  - **Right: Contact Form Card** (White Card with Subtle Shadow)
    - Heading: `Send Us a Message`
    - Supporting text: *"We'll get back to you within 24 hours."*
    - Form Fields:
      - **Full Name** (`text` input, required) & **Email Address** (`email` input, required) — side-by-side on desktop.
      - **Subject** (`select` dropdown, required): *General Inquiry*, *Course Information*, *Technical Support*, *Feedback*, *Other*.
      - **Message** (`textarea`, required, full width).
      - **Send Message** (full-width orange CTA submit button).

---

## 📱 Responsive Breakpoints

- **Desktop (> 1024px):**
  - Max container width: `1200px`.
  - Horizontal navbar with centered links and right-aligned Sign In.
  - 5-column Learning Journey grid.
  - 4-column Course video grid.
  - 2-column Contact layout (Info Panel + Form).
- **Tablet (768px – 1024px):**
  - 3-column / 2-column Learning Journey grid.
  - 2-column Course video grid.
  - Adjusted spacing, font sizes, and hero alignment.
- **Mobile (< 768px):**
  - Single-column stacked layouts for all sections.
  - Hero image stacked beneath headline and CTA.
  - 1-column Learning Journey cards.
  - 1-column Course video cards.
  - Full-width inputs and stacked form fields.
  - Adaptive navigation with touch-friendly links.
  - Zero horizontal overflow (`overflow-x: hidden`).

---

## ✅ Quality Checklist

- [x] Semantic HTML5 markup throughout all pages
- [x] Clean, organized CSS with custom property tokens
- [x] Responsive on desktop, tablet, and mobile devices
- [x] Exact color palette matching specifications
- [x] Reusable navbar with active link indicator on every page
- [x] 9 YouTube video embeds with 16:9 ratio and fullscreen enabled
- [x] Visual contact form with required validation attributes
- [x] Accessible form labels and iframe titles
- [x] Zero JavaScript, frameworks, or backend dependencies

