# 🎸 3/4Zwööölwe - Official Website

Modern, responsive website for the rock band 3/4Zwööölwe built with Astro, featuring mobile-first design and smooth animations.

## 🚀 Features

- **Mobile-First Design**: Fully responsive and optimized for all devices
- **Modern Animations**: Smooth transitions and engaging user interactions
- **TypeScript Typing Effect**: Dynamic slogan animation on the hero section
- **Component-Based Architecture**: Reusable components for Header, Footer, and Gigs
- **JSON Data Management**: Tour dates managed in a clean JSON format
- **SEO Optimized**: Proper meta tags and semantic HTML
- **Dark Theme**: Modern dark design with accent colors
- **Accessibility**: WCAG compliant with proper ARIA labels

## 🛠 Tech Stack

- **Framework**: [Astro](https://astro.build)
- **Styling**: CSS with modern features (Grid, Flexbox, Gradients)
- **Scripting**: JavaScript & TypeScript
- **Deployment**: GitHub Pages / Vercel
- **Version Control**: Git & GitHub

## 📁 Project Structure

```
src/
├── components/
│   ├── Header.astro        # Navigation with burger menu
│   ├── Footer.astro        # Footer with social links
│   └── Gigs.astro          # Tour dates component
├── data/
│   └── gigs.json           # Tour dates data
├── layouts/
│   └── Layout.astro        # Base layout template
├── pages/
│   ├── index.astro         # Home page with hero & about
│   ├── about.astro         # About page
│   ├── imprint.astro       # Impressum
│   └── privacy.astro       # Datenschutz
└── styles/
    └── global.css          # Global styles
```

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ and npm installed
- Basic knowledge of Astro and Astro components

### Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/3-4-zwoelwe-website.git
cd 3-4-zwoelwe-website
```

2. Install dependencies:

```bash
npm install
```

3. Start the development server:

```bash
npm run dev
```

Visit `http://localhost:3000` to see the site in development mode.

## 📝 Managing Tour Dates

Tour dates are managed in `src/data/gigs.json`. Each gig entry includes:

```json
{
  "id": 1,
  "date": "2024-03-15",
  "time": "20:00",
  "venue": "Rockclub Magdeburg",
  "city": "Magdeburg",
  "ticket_url": "https://tickets.example.com",
  "sold_out": false
}
```

Simply add, edit, or remove entries and the website will automatically update.

## 🎨 Customization

### Slogans

Edit the slogans array in `src/pages/index.astro` to change the typing effect text:

```javascript
const slogans = [
  'Unleash the Rock',
  'Your custom slogan here',
  // ...
];
```

### Colors

The main colors can be customized in the CSS variables throughout the stylesheets:

- Primary: `#ff006e` (Pink)
- Secondary: `#14b8a6` (Teal)
- Background: `#0a0a0a` (Dark)

### Band Information

Update band information in:
- `src/pages/about.astro` - About page content
- `src/pages/index.astro` - Home page about section
- `src/components/Header.astro` - Band name and navigation

## 🚀 Deployment

### Deploy to Vercel

1. Push your code to GitHub
2. Connect your GitHub repository to Vercel
3. Vercel will automatically build and deploy on every push

### Deploy to GitHub Pages

Add to `astro.config.mjs`:

```javascript
export default defineConfig({
  site: 'https://yourusername.github.io',
  base: '/repository-name'
});
```

Then run:

```bash
npm run build
git add dist/
git commit -m "Deploy"
git push
```

## 📦 Build

To create a production build:

```bash
npm run build
```

Preview the production build locally:

```bash
npm run preview
```

## 🔧 Development Tips

- Use `npm run dev` for hot-reload during development
- Components are located in `src/components/` and can be imported into pages
- Pages are automatically routed based on filenames in `src/pages/`
- Use TypeScript for type safety in scripts
- CSS is scoped to each component for better maintainability

## 📄 Legal Pages

The website includes:
- **Impressum** (`/imprint`) - Legal notice
- **Datenschutz** (`/privacy`) - Privacy policy

Remember to update these with actual band information!

## 🎓 Learning Resources

- [Astro Documentation](https://docs.astro.build)
- [Astro Discord Community](https://astro.build/chat)
- [Responsive Web Design](https://web.dev/responsive-web-design-basics/)

## 📧 Support

For questions or issues, contact the band or the web development team.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Credits

Designed and developed by [r3webdesign](https://r3webdesign.de)

---

**Rock on!** 🎸🎵
