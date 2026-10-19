# Shiki Coffee
A responsive website for **Shiki Coffee**, a student-founded coffee shop built around quality, sustainability, and community. This project turns a product idea into a functional front-end web app, built as a demo for a front-end design interview.

> **Note:** This project is not hosted live. Run it locally using the steps below.

## Purpose
Students need a quick way to learn about the café, see what is on offer, and find out how to visit. The site aims to be:
- **Clear:** the key information is visible within seconds of landing
- **Mobile-first:** most students will browse on their phones
- **Maintainable:** built from small, reusable components

## Tech stack
| Area | Choice |
|---|---|
| UI | React 19 with TypeScript |
| Routing | React Router 7 |
| Styling | Tailwind CSS 4 |
| Build tool | Vite 8 |
| Fonts | Raleway and Meow Script (Google Fonts) |
| Formatting | oxfmt |
| Tooling | Node 22, pnpm (versions pinned in `.mise.toml`) |

## Getting started
**Prerequisites:** Node.js 22 and pnpm. If you use [mise](https://mise.jdx.dev), run `mise install` and it will set up both automatically.

```bash
# 1. Clone the repo
git clone https://github.com/leez-genasi/demo.git
cd demo

# 2. Install dependencies
pnpm install

# 3. Start the dev server
pnpm dev
```

Then open the local URL printed in the terminal (usually http://localhost:5173).

### Other scripts

| Command | What it does |
|---|---|
| `pnpm dev` | Start the development server |
| `pnpm build` | Create a production build in `dist/` |
| `pnpm preview` | Preview the production build locally |
| `pnpm format` | Format the codebase with oxfmt |

## Project structure

```
demo/
├── public/          # Static assets (favicon, images)
├── src/             # Application source (entry point: main.tsx)
├── index.html       # HTML shell, fonts and meta tags
├── vite.config.ts   # Vite configuration
├── tsconfig.json    # TypeScript configuration
└── package.json
```

## Pages
| Page | Purpose |
|---|---|
| Home | First impression: rand message and main call-to-action |
| Menu | A quick look at what the cafe has to offer in terms of refreshments |
| About Us | Tell the café's story | 

## Design decisions
- **Typography:** Raleway for readable body text, Meow Script as a friendly accent for the brand
- **Layout:** mobile-first, scaling up to desktop with Tailwind responsive utilities
- **Components:** small and reusable so new pages and sections are quick to add
- **Data driven:** Reused data is compiled in a file that serves as the local database so it can be easily edited if required

## Possible next steps

- Proper database or content-management system integration so staff can update content without code changes
- Live outlet monitoring system
- Analytics charts for popular items or peak hours
- Ingredient showcase to enhance branding
