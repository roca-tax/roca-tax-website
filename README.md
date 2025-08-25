# Roca Tax Website

A professional, bilingual Hugo-based static website for Roca Tax, a tax preparation and accounting business in Rochester, NY.

## Features

- **Professional Business Design**: Clean, modern design tailored for accounting and tax services
- **Bilingual Support**: Full content in both English and Spanish
- **Responsive Layout**: Mobile-friendly design that works on all devices
- **Custom Hugo Theme**: Built specifically for Roca Tax with professional styling
- **SEO Optimized**: Proper meta tags and structured content
- **Fast Loading**: Static site generation for optimal performance

## Technology Stack

- **Hugo**: Static site generator
- **Bootstrap 5**: CSS framework for responsive design
- **Font Awesome**: Icon library
- **Google Fonts**: Typography (Inter + Playfair Display)
- **Custom CSS**: Professional business styling

## Site Structure

```
roca-tax-website/
├── content/                 # Content pages
│   ├── _index.md           # Home page
│   ├── about/              # About us page
│   ├── services/           # Services page
│   └── contact/            # Contact page
├── themes/                 # Custom theme
│   └── roca-tax-theme/     # Roca Tax theme
├── config.toml             # Hugo configuration
└── README.md               # This file
```

## Pages

### Home Page (`/`)
- Hero section with bilingual messaging
- Services overview
- Why choose us section
- Call-to-action

### Services (`/services/`)
- Comprehensive service listings
- Individual and business tax services
- Tax planning and consulting
- IRS problem resolution
- Bilingual content

### About Us (`/about/`)
- Company story and mission
- Team information
- Values and commitment
- Community involvement
- Bilingual content

### Contact (`/contact/`)
- Contact information
- Business hours
- Service areas
- What to bring to appointments
- Bilingual content

## Getting Started

### Prerequisites

- Hugo installed on your system
- Git for version control

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd roca-tax-website
   ```

2. Install Hugo (if not already installed):
   ```bash
   # On Ubuntu/Debian
   sudo apt install hugo
   
   # On macOS with Homebrew
   brew install hugo
   
   # On Windows with Chocolatey
   choco install hugo
   ```

3. Start the development server:
   ```bash
   hugo server -D
   ```

4. Open your browser and navigate to `http://localhost:1313`

### Building for Production

```bash
hugo --minify
```

The built site will be in the `public/` directory.

## Customization

### Colors and Styling

The theme uses CSS custom properties for easy customization. Main colors are defined in `themes/roca-tax-theme/assets/css/main.css`:

```css
:root {
    --primary-color: #2c3e50;      /* Dark blue */
    --secondary-color: #3498db;    /* Blue */
    --accent-color: #e74c3c;       /* Red */
    --success-color: #27ae60;      /* Green */
    --text-color: #2c3e50;         /* Dark text */
}
```

### Content Updates

- **Home page**: Edit `content/_index.md`
- **Services**: Edit `content/services/_index.md`
- **About**: Edit `content/about/_index.md`
- **Contact**: Edit `content/contact/_index.md`

### Configuration

Update `config.toml` to modify:
- Company information
- Contact details
- Business hours
- Service lists
- Menu structure

## Deployment

### Netlify (Recommended)

1. Connect your Git repository to Netlify
2. Set build command: `hugo --minify`
3. Set publish directory: `public`
4. Deploy automatically on Git push

### GitHub Pages

1. Build the site: `hugo --minify`
2. Push the `public/` directory to the `gh-pages` branch
3. Enable GitHub Pages in repository settings

### Traditional Web Hosting

1. Build the site: `hugo --minify`
2. Upload contents of `public/` directory to your web server

## Content Management

### Adding New Pages

```bash
hugo new page-name/_index.md
```

### Adding Blog Posts (if needed)

```bash
hugo new posts/post-title.md
```

### Markdown Front Matter

Each content file should include:

```yaml
---
title: "Page Title"
description: "Page description for SEO"
date: 2024-01-01
draft: false
---
```

## SEO and Performance

### SEO Features

- Meta descriptions for all pages
- Proper heading structure (H1, H2, H3)
- Alt text for images
- Semantic HTML structure
- Open Graph meta tags (can be added)

### Performance Features

- Static site generation
- Optimized CSS and JavaScript
- Responsive images
- Minimal external dependencies

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Internet Explorer 11+

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test locally with `hugo server`
5. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support or questions about the website:
- Email: info@roca.tax
- Phone: (585) 207-2221

## Roadmap

### Future Enhancements

- [ ] Blog section for tax tips and updates
- [ ] Online appointment booking system
- [ ] Client portal for document uploads
- [ ] Multi-language support for additional languages
- [ ] Advanced contact forms
- [ ] Integration with accounting software
- [ ] Mobile app for client communication

---

**Roca Tax** - Professional Tax Preparation & Accounting Services  
Rochester, NY | (585) 207-2221 | info@roca.tax 