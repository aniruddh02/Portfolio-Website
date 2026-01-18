# 🚀 Aniruddh Tiwari - Engineering Portfolio

![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) 
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white) 
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) 
![Responsive](https://img.shields.io/badge/Responsive-Design-green?style=for-the-badge)

> A modern, data-driven portfolio website designed for engineering leaders and builders. Built with performance, accessibility, and ease of maintenance in mind.

---

## ✨ Features

*   **⚡ Zero Dependencies**: Built with pure HTML5, Vanilla CSS, and JavaScript. No build steps, no heavy frameworks.
*   **📄 Data-Driven Content**: All content (Projects, Articles, About Me, etc.) is managed via simple `.json` files in the `resources/` folder. Update your site without touching a line of HTML.
*   **🌓 Dynamic Dark Mode**: Features a professionally curated color theme that switches between a Clean Blue Light Mode and a Deep Midnight Blue Dark Mode.
*   **🎨 Customizable Theme**: Fully configurable color palette via `resources/theme.json`.
*   **📱 Fully Responsive**: Optimized for all devices, from mobile phones to large desktop screens.
*   **♿ Accessible**: Semantic HTML and ARIA best practices.

---

## 🛠️ Project Structure

The project is organized to separate code from content:

```
/
├── index.html          # The main skeleton and logic (DO NOT EDIT for content)
├── resources/          # 📝 ALL CONTENT LIVES HERE
│   ├── about.json      # Bio and expertise
│   ├── article.json    # Writings and publications
│   ├── banner.json     # Hero section configuration
│   ├── learning-resources.json # Videos, books, and courses
│   ├── profile.json    # Headshot and meta info
│   ├── projects.json   # Portfolio projects
│   └── theme.json      # 🎨 Color theme configuration
├── images/             # 🖼️ Asset directory
└── css/                # (Optional) Additional styles if needed
```

---

## 🚀 Quick Start

Since this is a static site, you don't need `npm install` or a build process.

1.  **Clone the repository**:
    ```bash
    git clone https://github.com/aniruddh02/Portfolio-Website.git
    ```

2.  **Run locally**:
    You can use any static file server. For example:
    *   **VS Code**: Right-click `index.html` and choose "Open with Live Server".
    *   **Python**: `python3 -m http.server 8000`
    *   **Node**: `npx serve .`

3.  **Deploy**:
    Push to **GitHub Pages**, **Vercel**, or **Netlify**. It works out of the box!

---

## ⚙️ Configuration & Content

### Updating Content
To update your portfolio, simply edit the JSON files in the `resources/` directory.

**Example: Adding a new Project (`resources/projects.json`)**
```json
{
  "section": { "title": "Projects", ... },
  "items": [
    {
      "icon": "⚡",
      "title": "My New Project",
      "description": "Description of what I built...",
      "link": "https://github.com/...",
      "linkText": "View Code"
    }
  ]
}
```

### Customizing the Look (`resources/theme.json`)
Want to change the brand colors? Edit `theme.json`:

```json
{
    "light": {
        "accent": "#1e40af",  // Main user interaction color
        "heroGradientStart": "#172554" // Header background
    },
    ...
}
```

---

## ❤️ Credits

Created with love by **Google Antigravity**.

*   **Icons**: [Google Fonts Material Symbols](https://fonts.google.com/icons)
*   **Font**: [Inter](https://fonts.google.com/specimen/Inter)
