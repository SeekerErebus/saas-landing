# FlowStack -- SaaS Landing Page Template

A modern, conversion-focused SaaS landing page template built with Astro and Tailwind CSS. Themed as "FlowStack," a fictional project management tool, but easily re-skinned for any SaaS product.

![Screenshot](screenshot.png)

[![Astro](https://img.shields.io/badge/Astro-5.x-BC52EE?logo=astro&logoColor=white)](https://astro.build)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.x-06B6D4?logo=tailwindcss&logoColor=white)](https://tailwindcss.com)
[![Responsive](https://img.shields.io/badge/Responsive-Mobile_First-10B981)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## Features

- **Full landing page layout** -- Nav, Hero, Features, Social Proof, Pricing, FAQ, Footer
- **Animated hero section** -- gradient orbs, dot-grid background, pulsing beta badge, and a browser-chrome product mockup
- **Feature cards** -- 4 features with inline SVG icons and hover border effects
- **Social proof section** -- logo bar (6 company names) + 3 testimonial cards with star ratings and avatars
- **Three-tier pricing** -- Free / Pro / Enterprise with a monthly/annual toggle that updates prices in real-time
- **FAQ accordion** -- 6 questions with expand/collapse animation and icon rotation
- **Newsletter signup** -- email capture form in the footer
- **Full footer** -- 4-column link grid (Product, Company, Resources, Legal) with social icons (X, GitHub, LinkedIn)
- **Mobile navigation** -- hamburger menu with smooth toggle and auto-close on link tap
- **Indigo/violet accent palette** -- dark surface with indigo-500 as the primary accent
- **Open Graph & Twitter meta** -- social sharing tags on every page
- **Backdrop blur nav** -- fixed navigation with glassmorphism effect
- **Static output** -- pre-rendered HTML, deploys anywhere (Vercel, Netlify, Cloudflare Pages)
- **Zero JavaScript frameworks** -- vanilla JS for pricing toggle, FAQ accordion, and mobile menu only

## Tech Stack

| Layer       | Technology                                                         |
| ----------- | ------------------------------------------------------------------ |
| Framework   | [Astro 5.x](https://astro.build) (static output)                  |
| Styling     | [Tailwind CSS 4](https://tailwindcss.com) via `@tailwindcss/vite`  |
| Fonts       | Google Fonts (Inter)                                               |
| Language    | TypeScript                                                         |

## Project Structure

```
saas-landing/
├── public/
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── Nav.astro          # Fixed glassmorphism navbar + mobile menu
│   │   ├── Hero.astro         # Hero with gradient effects + product mockup
│   │   ├── Features.astro     # 4-card feature grid with SVG icons
│   │   ├── SocialProof.astro  # Logo bar + testimonial cards
│   │   ├── Pricing.astro      # 3-tier pricing with billing toggle
│   │   ├── FAQ.astro          # Accordion FAQ section
│   │   └── Footer.astro       # Newsletter form + link columns + socials
│   ├── layouts/
│   │   └── Layout.astro       # Base HTML shell with OG tags
│   ├── pages/
│   │   └── index.astro        # Single-page landing
│   └── styles/
│       └── global.css         # Tailwind 4 theme (surface/accent palette)
├── astro.config.mjs
├── tsconfig.json
└── package.json
```

## Quick Start

```bash
# Clone the repository
git clone https://github.com/SeekerErebus/saas-landing.git
cd saas-landing

# Install dependencies
npm install

# Start the dev server
npm run dev
```

The site will be running at `http://localhost:4321`.

## Commands

| Command           | Action                                      |
| :---------------- | :------------------------------------------ |
| `npm install`     | Install dependencies                        |
| `npm run dev`     | Start dev server at `localhost:4321`         |
| `npm run build`   | Build production site to `./dist/`           |
| `npm run preview` | Preview the production build locally         |

## Customization

1. **Branding** -- Replace "FlowStack" and the lightning bolt logo in `Nav.astro` and `Footer.astro`
2. **Colors** -- Edit the `@theme` block in `src/styles/global.css` to swap the indigo accent for your brand color
3. **Features** -- Update the `features` array in `Features.astro` with your product's selling points
4. **Pricing** -- Modify the `plans` array in `Pricing.astro` with your tiers, prices, and feature lists
5. **Testimonials** -- Replace the quotes, names, and titles in `SocialProof.astro`
6. **FAQ** -- Edit the `faqs` array in `FAQ.astro` with your own questions and answers
7. **Footer links** -- Update the `columns` array in `Footer.astro` to match your site structure
8. **Newsletter** -- Wire the footer form action to your email provider (Buttondown, ConvertKit, etc.)

## Live Demo

[View Live Demo](#) <!-- Replace with deployed URL -->

## License

MIT
