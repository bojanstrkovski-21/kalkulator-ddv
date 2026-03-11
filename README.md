# 🧮 ДДВ Калкулатор

A modern VAT (DDV) calculator for North Macedonia built with Astro.js and styled with the Everforest color theme.

## Features

- ✅ Calculate VAT with two rates: 18% (standard) and 5% (reduced)
- ✅ Add VAT to base amount
- ✅ Extract VAT from total amount
- ✅ Real-time calculations
- ✅ Clean, modern UI with Everforest Medium Dark theme
- ✅ Fully responsive design
- ✅ Static site - perfect for GitHub Pages

## Getting Started

### Prerequisites

- Node.js 18+ installed
- npm or yarn

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/kalkulator-ddv.git
cd kalkulator-ddv
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

4. Open your browser at `http://localhost:4321`

## Building for Production

```bash
npm run build
```

The static files will be generated in the `dist/` folder.

## Deploying to GitHub Pages

### Setup

1. Go to your GitHub repository settings
2. Navigate to **Pages** section
3. Under **Source**, select **GitHub Actions**

### Automatic Deployment

The project includes a GitHub Actions workflow that automatically builds and deploys to GitHub Pages when you push to the `main` branch.

### Update Configuration

Before deploying, update the `site` and `base` in `astro.config.mjs`:

```javascript
export default defineConfig({
  site: 'https://yourusername.github.io',
  base: '/kalkulator-ddv',
});
```

Replace `yourusername` with your GitHub username.

## Project Structure

```
kalkulator-ddv/
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Pages deployment
├── src/
│   ├── pages/
│   │   └── index.astro         # Main calculator page
│   └── styles/
│       └── global.css          # Everforest theme styles
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

## VAT Rates in North Macedonia

- **18%** - Standard rate for most goods and services
- **5%** - Reduced rate for basic food products, medicines, books, agricultural products

## Technologies Used

- [Astro.js](https://astro.build/) - Static site generator
- TypeScript - Type-safe scripting
- CSS3 - Styling with Everforest color palette
- GitHub Actions - CI/CD for deployment

## License

MIT

## Author

Made with ❤️ for North Macedonia
