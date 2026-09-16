# Portfolio-clint

A single-page portfolio website built with **Next.js (App Router)** and **React**.  
The page is composed of reusable sections (hero, services, experience, projects, testimonials, contact/footer) with animated UI and smooth scrolling behavior.

## Tech Stack

- **Framework:** Next.js 15
- **UI:** React 19
- **Styling:** Tailwind CSS 4 (+ `tw-animate-css`)
- **Animation:** Framer Motion
- **Smooth Scrolling:** Lenis (`@studio-freight/lenis`)
- **Slider/Carousel:** Swiper
- **Icons:** `lucide-react`, `react-icons`
- **UI utility:** shadcn-style `Button` component with `class-variance-authority`

## Project Structure

- `/app/layout.js` – root layout and global providers
- `/app/page.js` – main page composition
- `/app/globals.css` – global styles and design tokens
- `/components/*` – portfolio sections and shared UI components
- `/public/*` – static assets (images/SVGs used by sections)

## Installation

```bash
npm install
```

## Available npm Scripts

From `package.json`:

- `npm run dev` – start development server (Turbopack)
- `npm run build` – create production build
- `npm run start` – run production server
- `npm run lint` – run Next.js ESLint checks

## Run Locally

```bash
npm run dev
```

Then open: `http://localhost:3000`

## Notes for Development

- This repository currently has **lint/build scripts** but no dedicated automated test script.
- Smooth scrolling is handled by Lenis in `components/LenisProvider.jsx`.
- Most section animations are implemented with Framer Motion and `whileInView` transitions.

## Deployment

Build first:

```bash
npm run build
```

Then run:

```bash
npm run start
```

You can deploy this Next.js app to any platform that supports Node.js (for example Vercel, VPS, or container-based hosting).
