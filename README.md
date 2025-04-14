# AI Tools Directory Website 🤖

A comprehensive directory of AI tools and resources featuring a responsive 3-column grid layout.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization Guide](#customization-guide)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Resources & Support](#resources--support)

## Overview

AI Tools is a curated directory website showcasing various artificial intelligence tools and resources. The website features a clean, responsive design with a 3-column grid layout, making it easy for users to discover and explore AI tools.

## Features

- 📱 Responsive 3-column grid layout
- 🔍 Search functionality
- 🏷️ Category filtering
- 💨 Fast loading times
- 🎨 Customizable styling
- 📊 SEO optimized
- 🔄 Easy content updates

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Git

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/ai-tools-directory.git

# Navigate to project directory
cd ai-tools-directory

# Install dependencies
npm install

# Start development server
npm run dev
```

## Directory Structure

```
ai-tools-directory/
├── src/
│   ├── components/
│   │   ├── Header.js
│   │   ├── Footer.js
│   │   ├── ToolCard.js
│   │   └── CategoryFilter.js
│   ├── data/
│   │   ├── tools.json
│   │   └── categories.json
│   ├── styles/
│   │   └── main.css
│   └── pages/
│       └── index.js
├── public/
│   └── images/
├── package.json
└── README.md
```

## Customization Guide

### Adding/Editing Directory Items

1. Navigate to `src/data/tools.json`
2. Add new tools using the following format:

```json
{
  "id": "unique-id",
  "name": "Tool Name",
  "description": "Tool description",
  "category": "category-slug",
  "url": "https://toolturl.com",
  "image": "/images/tool-image.png"
}
```

### Modifying Category Labels

1. Open `src/data/categories.json`
2. Edit or add categories:

```json
{
  "ai-chatbots": {
    "name": "AI Chatbots",
    "description": "Conversational AI tools"
  }
}
```

### Updating Hero Section

1. Locate `src/components/Header.js`
2. Modify the hero content:

```jsx
<div className="hero">
  <h1>Your New Title</h1>
  <p>Your new description</p>
</div>
```

### Customizing Colors and Styling

1. Navigate to `src/styles/main.css`
2. Update the CSS variables:

```css
:root {
  --primary-color: #3498db;
  --secondary-color: #2ecc71;
  --text-color: #333333;
  --background-color: #ffffff;
}
```

## Deployment

### Vercel Deployment

1. Connect your GitHub repository to Vercel
2. Configure build settings:
   - Build Command: `npm run build`
   - Output Directory: `out`
3. Deploy

### Netlify Deployment

```bash
# Install Netlify CLI
npm install netlify-cli -g

# Deploy to Netlify
netlify deploy
```

## Custom Domain Setup

1. Purchase a domain from your preferred registrar
2. Add domain in your deployment platform:
   - Go to project settings
   - Navigate to domains section
   - Add custom domain
3. Configure DNS settings:
   ```
   A Record: @ -> deployment-platform-ip
   CNAME: www -> yourdomain.com
   ```

## Troubleshooting

### Common Issues

1. **Build Errors**
   - Clear cache: `npm run clean`
   - Delete node_modules: `rm -rf node_modules`
   - Reinstall dependencies: `npm install`

2. **Image Loading Issues**
   - Verify image path in tools.json
   - Ensure images are in public directory
   - Check image format (supported: jpg, png, webp)

3. **Category Filter Not Working**
   - Check category slugs match in both tools.json and categories.json
   - Clear browser cache
   - Verify JavaScript console for errors

## Resources & Support

- [Documentation Wiki](https://github.com/yourusername/ai-tools-directory/wiki)
- [Issue Tracker](https://github.com/yourusername/ai-tools-directory/issues)
- [Contributing Guidelines](CONTRIBUTING.md)

### Community
- [Discord Community](https://discord.gg/aitools)
- [Twitter](https://twitter.com/aitools)
- Email Support: support@aitools.com

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Made with ❤️ by [Your Name]