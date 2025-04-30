# Hong Kong - Local Business Directory 🏢

> Discover the best local businesses in Hong Kong - A comprehensive directory website featuring local establishments, services, and venues across Hong Kong.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Netlify Status](https://api.netlify.com/api/v1/badges/your-netlify-badge/deploy-status)](https://app.netlify.com/sites/your-site/deploys)

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

This directory website showcases local businesses in Hong Kong using a responsive 3-column grid layout. The site is built with HTML5, CSS3, and vanilla JavaScript, ensuring fast loading times and easy customization.

## Features

- 📱 Responsive 3-column grid layout
- 🔍 Search functionality
- 🏷️ Category filtering
- 📍 Location-based sorting
- 💼 Business profiles with contact information
- 🖼️ Image gallery support
- 📱 Mobile-friendly design
- 🔗 Social media integration

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- Git
- Text editor (VS Code recommended)

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/hk-business-directory.git

# Navigate to project directory
cd hk-business-directory

# Install dependencies
npm install

# Start development server
npm run dev
```

## Directory Structure

```
hk-business-directory/
├── assets/
│   ├── images/
│   ├── css/
│   └── js/
├── data/
│   └── businesses.json
├── components/
│   ├── header.html
│   └── footer.html
├── pages/
├── index.html
└── README.md
```

## Customization Guide

### Adding/Editing Directory Items

1. Open `data/businesses.json`
2. Add new business entry using the following format:

```json
{
  "id": "unique-id",
  "name": "Business Name",
  "category": "Restaurant",
  "address": "123 Nathan Road, TST",
  "phone": "+852 1234 5678",
  "website": "https://example.com",
  "description": "Business description",
  "image": "assets/images/business-name.jpg"
}
```

### Modifying Category Labels

1. Open `assets/js/categories.js`
2. Edit the category array:

```javascript
const categories = [
  "Restaurants",
  "Retail",
  "Services",
  "Entertainment"
  // Add more categories
];
```

### Updating Hero Section

1. Navigate to `index.html`
2. Locate the hero section:

```html
<section class="hero">
  <h1>Your Title Here</h1>
  <p>Your subtitle here</p>
  <!-- Modify as needed -->
</section>
```

### Customizing Colors and Styling

1. Open `assets/css/style.css`
2. Modify the CSS variables:

```css
:root {
  --primary-color: #2c3e50;
  --secondary-color: #3498db;
  --text-color: #333;
  --background-color: #f5f6fa;
}
```

## Deployment

### Netlify Deployment

1. Create a Netlify account
2. Connect your GitHub repository
3. Configure build settings:
   - Build command: `npm run build`
   - Publish directory: `dist`
4. Click "Deploy"

### Manual Deployment

```bash
# Build project
npm run build

# Deploy to your server
scp -r dist/* user@your-server:/path/to/public_html
```

## Custom Domain Setup

1. Purchase domain from preferred registrar
2. Add DNS records:
   ```
   A Record: @ points to your-server-ip
   CNAME: www points to your-netlify-site.netlify.app
   ```
3. Configure SSL certificate

## Troubleshooting

### Common Issues

1. **Images not loading**
   - Check file paths in `businesses.json`
   - Verify image format (JPG/PNG supported)
   - Ensure images are in `assets/images`

2. **Search not working**
   - Clear browser cache
   - Check console for JavaScript errors
   - Verify `businesses.json` format

3. **Layout issues**
   - Update to latest version
   - Clear browser cache
   - Check CSS media queries

## Resources & Support

- 📖 [Documentation Wiki](https://github.com/yourusername/hk-business-directory/wiki)
- 🐛 [Issue Tracker](https://github.com/yourusername/hk-business-directory/issues)
- 💬 [Community Forum](https://github.com/yourusername/hk-business-directory/discussions)
- 📧 Support: support@example.com

### Contributing

1. Fork repository
2. Create feature branch
3. Commit changes
4. Push to branch
5. Create Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Made with ❤️ in Hong Kong