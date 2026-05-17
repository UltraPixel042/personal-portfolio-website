# 🌐 Wannawat's Personal Portfolio Website

A personal portfolio website built to showcase my skills, projects, and contact information. Designed with a clean, modern UI supporting both light and dark modes.

---

## ✨ Features

- 🌙 **Dark / Light Mode** toggle
- 📱 **Responsive design** — mobile hamburger menu + desktop nav
- 🔗 **Smooth anchor navigation** to each section
- 💼 Sections: Hero · About Me · Skills · Projects · Contact · Footer

---

## 🛠️ Tech Stack

| Technology | Role |
|---|---|
| [Vue 3](https://vuejs.org/) | UI Framework (Composition API) |
| [Vite](https://vite.dev/) | Build tool & dev server |
| [Tailwind CSS v4](https://tailwindcss.com/) | Utility-first styling |
| [Bootstrap Icons](https://icons.getbootstrap.com/) | SVG icon set (inline) |

---

## 📁 Project Structure

```
wannawat-web/
├── public/
│   └── wannawat-circle-removebg.png   # Profile image
├── src/
│   ├── components/
│   │   ├── Navbar.vue          # Top navigation bar (responsive)
│   │   ├── Hero.vue            # Landing / intro section
│   │   ├── AboutMe.vue         # Education, interests, languages
│   │   ├── Skills.vue          # Frontend & tools skill bars
│   │   ├── Projects.vue        # Project list with GitHub links
│   │   ├── Contact.vue         # Contact info (email, GitHub, etc.)
│   │   ├── Footer.vue          # Footer with social links
│   │   ├── ProfileDropdown.vue # Profile dropdown menu
│   │   └── DarkModeToggle.vue  # Dark/light mode switch
│   ├── composables/
│   │   └── useDarkMode.js      # Dark mode state composable
│   ├── App.vue
│   ├── main.js
│   └── style.css
├── index.html
├── package.json
└── vite.config.js
```

---

## 🚀 Getting Started

### Prerequisites

- Node.js ≥ 18
- npm ≥ 9

### Installation

```sh
npm install
```

### Development Server

```sh
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

### Production Build

```sh
npm run build
```

---

## 👤 Author

**Wannawat Siriarkanay**
- GitHub: [@UltraPixel042](https://github.com/UltraPixel042)
- Email: wannawat2005@gmail.com
- LinkedIn: [วรรณวัฒน์ ศิริอาคเนย์](https://www.linkedin.com/in/%E0%B8%A7%E0%B8%A3%E0%B8%A3%E0%B8%93%E0%B8%A7%E0%B8%B1%E0%B8%92%E0%B8%99%E0%B9%8C-%E0%B8%A8%E0%B8%B4%E0%B8%A3%E0%B8%B4%E0%B8%AD%E0%B8%B2%E0%B8%84%E0%B9%80%E0%B8%99%E0%B8%A2%E0%B9%8C-a4390a231/)

---

© 2025 Wannawat · Built with Vue.js + Tailwind CSS
