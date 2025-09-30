# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static HTML website for "Jellydash", a puzzle platformer game landing page. The project consists of a single `index.html` file that serves as a marketing/landing page for the actual game hosted on CrazyGames.

## Architecture

- **Static Site**: No build system, package manager, or complex dependencies
- **Single File**: Everything is contained in `index.html`
- **Styling**: Uses Tailwind CSS via CDN
- **Deployment**: Simple file serving - any web server or GitHub Pages can host this

## Key Components

### HTML Structure (`index.html`)
- **Header**: Navigation with anchor links to page sections
- **Hero Section**: Main title and description with gradient text effects
- **Game Section**: Call-to-action with play button linking to CrazyGames
- **Features Section**: Three-column layout highlighting game benefits
- **About Section**: Detailed game description and instructions
- **Footer**: Copyright and attribution information

### Styling Approach
- **Tailwind CSS**: Framework loaded via CDN
- **Custom CSS**: Embedded styles for animations and special effects
- **Responsive Design**: Mobile-first approach with `md:` breakpoints
- **Visual Effects**: Float animations, pulse glow, gradient backgrounds

## Common Tasks

### Development
- **Local Development**: Open `index.html` directly in a browser or use a simple HTTP server
- **Live Preview**: Use any static site server like `python3 -m http.server` or `npx serve`
- **No Build Process**: Changes are immediately visible upon browser refresh

### Content Updates
- **Game Information**: Update text content in the relevant sections
- **Links**: Modify the CrazyGames URL in the play button (line 129)
- **Styling**: Adjust Tailwind classes or custom CSS as needed

### Deployment
- **Simple Upload**: Copy `index.html` to any web server
- **GitHub Pages**: Works out of the box with default settings
- **Netlify/Vercel**: Direct deployment without configuration

## File Structure

```
/
├── index.html          # Complete website source
└── .claude/            # Claude Code configuration
    └── settings.local.json
```

## Development Notes

- **No Dependencies**: All resources loaded from CDNs
- **SEO Optimized**: Meta tags, structured content, semantic HTML
- **Performance**: Lightweight, fast loading with minimal resources
- **Browser Compatibility**: Modern browser features, gracefully degrades