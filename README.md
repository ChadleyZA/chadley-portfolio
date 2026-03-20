# Chadley De Rose — Portfolio

Personal portfolio built with [Astro](https://astro.build). Dark minimal aesthetic with DM Mono + Syne fonts.

## Project Structure

```
chadley-portfolio/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── Nav.astro
│   │   ├── Hero.astro
│   │   ├── About.astro
│   │   ├── Skills.astro
│   │   ├── Projects.astro
│   │   ├── Experience.astro
│   │   ├── Certifications.astro
│   │   ├── Contact.astro
│   │   └── Footer.astro
│   ├── layouts/
│   │   └── BaseLayout.astro
│   ├── pages/
│   │   └── index.astro
│   └── styles/
│       └── global.css
├── astro.config.mjs
└── package.json
```

## Getting Started

```bash
# Install dependencies
npm install

# Start dev server (localhost:4321)
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Customising

### Update project links
Edit `src/components/Projects.astro` — find the `projects` array and replace `demo` and `code` with your real URLs.

### Add/remove skills
Edit `src/components/Skills.astro` — update the `skillGroups` array.

### Update contact form
The form currently shows a success message on submit. To wire it to a real backend, replace the script in `Contact.astro` with a fetch to your API endpoint or a service like [Formspree](https://formspree.io).

## Deployment

### Netlify (recommended)
1. Push to GitHub
2. Connect repo on [netlify.com](https://netlify.com)
3. Build command: `npm run build`
4. Publish directory: `dist`

### Vercel
1. Push to GitHub
2. Import on [vercel.com](https://vercel.com)
3. Framework preset: Astro
4. Deploy

## Tech Stack
- [Astro 4](https://astro.build)
- Vanilla CSS with CSS custom properties
- DM Mono + Syne (Google Fonts)
- Zero JavaScript frameworks — islands only where needed
