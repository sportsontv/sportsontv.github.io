# SportsOnTV Website

Source code for [sportsontv.app](https://sportsontv.app) - the marketing and legal pages for the SportsOnTV mobile app.

## Pages

- `/` - Landing page
- `/privacy` - Privacy Policy
- `/terms` - Terms of Service

## Local Development

### Prerequisites

- [mise](https://mise.jdx.dev/) (manages Node.js and pnpm versions)

### Setup

```sh
# Install tools (Node.js, pnpm)
mise install

# Install dependencies
pnpm install

# Start dev server at localhost:4321
pnpm dev
```

### Commands

| Command        | Action                                   |
| :------------- | :--------------------------------------- |
| `pnpm dev`     | Start local dev server at `localhost:4321` |
| `pnpm build`   | Build production site to `./dist/`       |
| `pnpm preview` | Preview production build locally         |

## Deployment

The site is automatically deployed to GitHub Pages when changes are pushed to `main`. The GitHub Actions workflow handles building and deployment.

## Project Structure

```
src/
├── components/    # Reusable UI components (Header, Footer, Hero)
├── layouts/       # Page layouts (BaseLayout, LegalLayout)
├── pages/         # Routes (index, privacy, terms)
└── styles/        # Global CSS
public/
├── CNAME          # Custom domain config
├── favicon.svg    # Site favicon
└── robots.txt
```
