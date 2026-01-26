# Landing Page Setup Documentation

## Overview

This document describes the setup of the atmospheric.reviews landing page using Astro and GitHub Pages.

## Initial Setup (Completed)

### 1. Node.js Version
- Required: Node.js 18 or higher
- Used: Node.js 22 via nvm
- Command: `source ~/.nvm/nvm.sh && nvm use 22`

### 2. Astro Installation
```bash
npm create astro@latest ./temp-astro -- --template minimal --install --no-git --typescript strict --skip-houston
```
- Template: minimal
- TypeScript: strict mode
- Installed in temp directory and moved to root

### 3. Project Configuration

**astro.config.mjs:**
```javascript
export default defineConfig({
  site: 'https://atmospheric.reviews',
});
```

**Key files created:**
- `src/pages/index.astro` - Main landing page
- `public/CNAME` - Custom domain configuration (atmospheric.reviews)
- `.github/workflows/deploy.yml` - GitHub Actions deployment workflow
- `package.json` - Dependencies and scripts
- `tsconfig.json` - TypeScript configuration

### 4. Custom Domain Setup

**CNAME file:**
- Location: `public/CNAME`
- Content: `atmospheric.reviews`
- Automatically copied to build output

**DNS Configuration (to be done at domain registrar):**
- Add A records pointing to GitHub Pages IPs:
  - 185.199.108.153
  - 185.199.109.153
  - 185.199.110.153
  - 185.199.111.153

### 5. GitHub Pages Configuration

**Repository Settings:**
- Go to Settings → Pages
- Source: **GitHub Actions** (not branch deployment)

**Deployment:**
- Automatic via GitHub Actions on push to main
- Workflow file: `.github/workflows/deploy.yml`
- Uses Node.js 20 for build
- Deploys `./dist` folder

## Landing Page Design

### Content Structure
- Header with title
- Intro section (highlighted with accent background)
- Four pillar sections (cards with hover effects)
- Responsive design
- Dark mode support (automatic based on system preference)

### Styling Features
- CSS custom properties for theming
- Mobile-first responsive design
- System font stack for performance
- Smooth transitions and hover effects
- Accessible color contrast

## Local Development

### Prerequisites
```bash
# Use Node.js 22 (or 18+)
source ~/.nvm/nvm.sh && nvm use 22
```

### Commands
```bash
# Install dependencies
npm install

# Start development server (localhost:4321)
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

### Development Workflow
1. Make changes to `src/pages/index.astro`
2. Hot reload automatically updates browser
3. Commit changes to git
4. Push to main branch
5. GitHub Actions automatically deploys

## File Structure
```
/
├── .claude/                    # Documentation
├── .github/
│   └── workflows/
│       └── deploy.yml         # Deployment automation
├── public/
│   ├── CNAME                  # Custom domain
│   ├── favicon.ico
│   └── favicon.svg
├── src/
│   └── pages/
│       └── index.astro        # Landing page
├── astro.config.mjs           # Astro configuration
├── package.json               # Dependencies
├── tsconfig.json              # TypeScript config
└── README.md                  # Project documentation
```

## Deployment Process

### Automatic Deployment
1. Push commits to main branch
2. GitHub Actions workflow triggers
3. Workflow installs dependencies
4. Builds site with `npm run build`
5. Uploads `dist/` folder
6. Deploys to GitHub Pages
7. Site live at https://atmospheric.reviews

### Manual Deployment
If needed, you can manually trigger the workflow:
- Go to Actions tab in GitHub
- Select "Deploy to GitHub Pages" workflow
- Click "Run workflow"

## Maintenance

### Updating Content
1. Edit `src/pages/index.astro`
2. Test locally with `npm run dev`
3. Commit and push changes
4. Deployment happens automatically

### Updating Dependencies
```bash
# Check for updates
npm outdated

# Update Astro
npm update astro

# Rebuild and test
npm run build
```

### Troubleshooting

**Build fails:**
- Check Node.js version (must be 18+)
- Run `npm ci` to clean install dependencies
- Check GitHub Actions logs

**DNS not resolving:**
- Wait up to 48 hours for propagation
- Verify A records at domain registrar
- Use `dig atmospheric.reviews` to check

**CNAME file missing in build:**
- Ensure `public/CNAME` exists
- Astro automatically copies public/ to dist/

## References

- Astro Documentation: https://astro.build
- GitHub Pages: https://docs.github.com/en/pages
- Project Repository: https://github.com/tgoerke/modular-reviews
- Live Site: https://atmospheric.reviews
