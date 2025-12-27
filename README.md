# Astro SPA Demo

This repository demonstrates Astro's SPA (Single Page Application) mode using the View Transition API. It showcases how to implement client-side navigation with the `ClientRouter` component for smooth, app-like page transitions without full page reloads.

![project status](https://img.shields.io/badge/status-work_in_progress-red?style=for-the-badge)
![live site](https://img.shields.io/badge/live_site-blue?style=for-the-badge)
![Lighthouse report](https://img.shields.io/badge/lighthouse-F44B21?style=for-the-badge&logo=lighthouse&logoColor=fff)

## Features

- **Client-side navigation** with the `ClientRouter` component from `astro:transitions`
- **Smooth page transitions** using the View Transition API
- **No full page reloads** between navigation
- **Automatic prefetching** for instant page loads
- **Preserved JavaScript state** during navigation

## Implementation

The demo includes three pages (Home, About, Contact) and a 404 page, all connected through a navigation menu. The `ClientRouter` component is added to the main layout, enabling SPA-style navigation throughout the site.

```astro
---
import { ClientRouter } from "astro:transitions";
---

<html lang="en">
  <head>
    <title>My Homepage</title>
    <ClientRouter />
  </head>
  <body>
    <h1>Welcome to my website!</h1>
  </body>
</html>
```

## Tech Stack

### Frontend

- **Framework**: [Astro 5](https://astro.build/)
- **Styling**: [Tailwind CSS 4](https://tailwindcss.com/)

### Backend

- **Hosting**: [Cloudflare Workers](https://workers.cloudflare.com/)

## How to Update

To check for outdated packages, run `npm outdated`.

```bash
# Update dependencies (this will rewrite package-lock.json and package.json)
npm update --save
npm install --save-exact --save-dev prettier@latest prettier-plugin-astro@latest prettier-plugin-tailwindcss@latest
```

## Dev Environment & Tools

- **System**: [Ubuntu](https://ubuntu.com/desktop)
- **Editor**: [VS Code](https://code.visualstudio.com/)
- **Formatter**: [Prettier](https://prettier.io/)
- **Linter**: [ESLint](https://eslint.org/)
- **AI assistant**: [GitHub Copilot](https://github.com/features/copilot)

## Copyright

© 2025 Johnny Gérard
