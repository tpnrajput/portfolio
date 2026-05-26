# Tapan Jadav | Personal Portfolio Website

Welcome to the repository for my professional portfolio website! This site is designed to showcase my experience as a Computer Engineer and Full-Stack Laravel Developer, highlighting the projects I've built, the technologies I use, and how to connect with me.

---

## Features

- **Modern Glassmorphic UI:** A visually stunning, dark-mode design built using modern CSS styling (translucent cards, blur backdrops, and glowing borders).
- **Fully Responsive Layout:** Optimized to look beautiful on all screen sizes, from small mobile devices (down to 380px) to iPads and large desktop monitors.
- **Interactive Project Cards:** Real-world project showcases (e.g., Order Manager) with proportional, non-stretching images and direct navigation links.
- **Dynamic Experience Tabs:** Interactive tabs detailing my professional journey, roles, and key contributions.
- **Single Page App (SPA) Routing:** Powered by React Router DOM, allowing users to transition between pages (like Home and About) instantly without page reloads.
- **SEO & Performance Optimized:** Implements meta tags, social graphs (Open Graph & Twitter Cards), critical asset preloading, and lazy loading for faster page loads.

---

## Tech Stack

This project is built using modern, industry-standard frontend technologies:

* **Framework:** React.js (version 18) with TypeScript for type-safety and robust development.
* **Styling:** Tailwind CSS for fast, utility-first layout styling and CSS Variables for dynamic design tokens.
* **Animations:** Framer Motion for smooth animations and transitions.
* **Icons:** Lucide React for consistent and modern SVG iconography.
* **Build Tool:** Vite for fast local development and optimized production bundles.

---

## How it Works (For Freshers & Non-Techs)

If you are new to React development, here is a quick breakdown of how this portfolio is structured and how data flows:

```
[User Browser]
      │
      ▼
┌──────────────┐
│  index.html  │  ◄─── Loaded first; contains SEO meta tags and page setup.
└──────┬───────┘
       │ Loads
       ▼
┌──────────────┐
│  main.tsx    │  ◄─── The entrypoint file; mounts React into the index.html.
└──────┬───────┘
       │ Renders
       ▼
┌──────────────┐
│   App.tsx    │  ◄─── Configures the routing (Home Page vs. About Page).
└──────┬───────┘
       ├──────────────────────────────┐
       ▼ (if path is "/")             ▼ (if path is "/about")
┌──────────────┐               ┌──────────────┐
│  Index.tsx   │ (Home Page)   │  About.tsx   │ (About Page)
└──────┬───────┘               └──────┬───────┘
       │                               │
       ├─► HeroSection.tsx             ├─► Personal Journey
       ├─► ExperienceSection.tsx       ├─► Education Cards
       ├─► SkillsSection.tsx           └─► Hobbies & Interests
       ├─► ProjectsSection.tsx
       └─► Footer.tsx
```

1. **Single Source of Truth (`src/data/portfolio.ts`):** All details (projects, experiences, skills, social links) are stored in a single text file. To update the website, you simply edit this data file, and the changes automatically reflect throughout the pages.
2. **Modular Components:** Each section (like the Hero image, the Project list, or the Navigation bar) is written as an isolated component under `src/components/`, making the code modular and easy to maintain.

---

## Getting Started

Follow these simple steps to run the portfolio website locally on your computer.

### Prerequisite
You need to have **Node.js** (version 18 or above) installed on your system. You can download it from [nodejs.org](https://nodejs.org/).

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/portfolio.git
   cd portfolio
   ```

2. **Install the dependencies:**
   This downloads all the code packages and libraries (like React, Tailwind, and Framer Motion) required to run the project.
   ```bash
   npm install
   ```

3. **Run the local development server:**
   This starts the project locally. Open the URL shown in your terminal (usually `http://localhost:5173/`) in your browser to view the site.
   ```bash
   npm run dev
   ```

4. **Build for production:**
   This compiles, optimizes, and bundles the application code into the `dist/` folder, ready to be served by any web hosting provider.
   ```bash
   npm run build
   ```

---

## Deployment

This website can be easily deployed to modern cloud hosting platforms like **Vercel**, **Netlify**, or **GitHub Pages**:

### Deploying to Vercel
1. Sign in to your [Vercel account](https://vercel.com/).
2. Click **New Project** and import this GitHub repository.
3. Vercel will automatically detect that it is a Vite project and configure the correct build settings:
   - **Build Command:** `npm run build`
   - **Output Directory:** `dist`
4. Click **Deploy**, and your portfolio will be live in less than a minute!

---

## Contact & Social Links

Feel free to connect with me for opportunities or collaboration:

- **LinkedIn:** [Tapan Jadav](https://www.linkedin.com/in/tapan-jadav)
- **GitHub:** [github.com/tapanjadav](https://github.com/tapanjadav)
- **Email:** [contact@conversantech.com](mailto:contact@conversantech.com)
