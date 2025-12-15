# Build Instructions

## Prerequisites

Node.js version 18 or higher is required.

## Installation

```bash
npm install
```

## Development

To run the development server:

```bash
npm run dev
```

Open http://localhost:3000 in your browser.

## Production Build

To create a static export:

```bash
npm run build
```

This will generate a static site in the `out` folder.

## Deployment

The `out` folder contains all static files and can be:
- Served from any web server
- Uploaded to static hosting (Netlify, Vercel, S3, etc.)
- Deployed as static HTML/CSS/JS

No server-side code is required. The entire application is pre-rendered to static HTML.

## File Structure

```
sentinel-demo/
├── src/
│   ├── app/                          # Next.js App Router pages
│   │   ├── layout.tsx                # Root layout with navigation
│   │   ├── page.tsx                  # Landing page
│   │   ├── governance-overview/      # Section 1
│   │   ├── risk-surfaces/            # Section 2
│   │   ├── sell-sequence/            # Section 3
│   │   ├── governance-artifacts/     # Section 4
│   │   ├── research-alignment/       # Section 5
│   │   └── what-this-is-not/         # Section 6
│   └── components/                   # Reusable components
│       ├── Navigation.tsx
│       ├── PageHeader.tsx
│       └── Disclaimer.tsx
├── next.config.js                    # Static export configuration
└── package.json
```

## Notes

- This is a static demonstration interface
- No backend or database required
- No user accounts or authentication
- No data processing or analytics
- All content is pre-rendered at build time
