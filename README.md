# Atmospheric Computing Research Proposal

Atmospheric computing is an emerging paradigm that describes the interconnection of previously isolated computing islands and cloud infrastructures that store data. This interconnection is enabled by emerging open social protocols such as ATProto, which provide the fabric for a decentralized yet interoperable ecosystem.

These interconnected but independent islands of data and compute resources, together with their corresponding user-facing applications, collectively form what we call the **Atmosphere**.

Atmospheric computing combines a protocol-mediated approach with **networked publics** to create an environment attractive to researchers, technologists, and users who seek more tangible and meaningful interactions in the digital space.

**We propose four main pillars:**

1. **Atmospheric Reviews** will address the challenge of evaluating research and technology within the Atmosphere by adopting modular review techniques and workflows. Building on our work with ATScience, we aim to establish a proven, rigorous process for scientific peer review adapted to this new computational paradigm.
2. **Atmospheric Computer** will establish a tilde-style community for creative computing practitioners, inspired by aesthetic.computer, fostering experimental and artistic approaches to atmospheric computing.
3. **ATScience** leverages ATProto to create open, democratic, researcher-owned infrastructure for scholarly communication. By empowering science communities to maintain full control of their content and relationships while collaborating across interoperable applications, this pillar prevents vendor lock-in and fosters innovation in research tools, demonstrating how decentralized protocols can transform scholarly discourse and accelerate discovery.
4. **Tilde-Style Communities** conceptualizes tildes as networked publics, with the understanding that the precise meaning of "tilde style" will evolve over time as these communities mature. [tilde.style](http://tilde.style/) serves as infrastructure for building a social layer for smallweb communities based on ATProto.

---

## Website

This repository contains the landing page for atmospheric.reviews, built with [Astro](https://astro.build).

### About Astro

Astro is a modern static site generator that delivers fast, content-focused websites. It features:
- Zero JavaScript by default for optimal performance
- Support for multiple UI frameworks (React, Vue, Svelte, etc.)
- Built-in optimizations for images, fonts, and assets
- Excellent developer experience with hot module reloading

### Local Development

**Prerequisites:**
- Node.js 18 or higher
- npm or your preferred package manager

**Setup and run:**

```bash
# Install dependencies
npm install

# Start development server
npm run dev
```

The site will be available at `http://localhost:4321`

**Other useful commands:**

```bash
# Build for production
npm run build

# Preview production build locally
npm run preview

# Run Astro CLI commands
npm run astro -- --help
```

### Project Structure

```
/
├── src/
│   └── pages/
│       └── index.astro    # Landing page
├── public/
│   └── CNAME              # Custom domain configuration
├── .github/
│   └── workflows/
│       └── deploy.yml     # GitHub Pages deployment
└── package.json
```

### Deployment

The site is automatically deployed to GitHub Pages via GitHub Actions when changes are pushed to the main branch. The workflow builds the site and publishes it to https://atmospheric.reviews.
