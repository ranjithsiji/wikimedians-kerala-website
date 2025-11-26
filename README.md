# Wikimedians of Kerala User Group Website

Official website for Wikimedians of Kerala User Group built with Hugo and Bootstrap.

## About

This website serves as the central hub for the Wikimedians of Kerala community, showcasing our projects, activities, and providing resources for contributors.

## Technology Stack

- **Static Site Generator**: Hugo
- **CSS Framework**: Bootstrap 5
- **Fonts**: Google Fonts (Poppins)
- **Icons**: Font Awesome

## Features

- Modern, responsive design
- Modular component architecture with Hugo partials
- Sections: Home, About, Projects, Community, Activities, Blog, Contact
- Smooth animations and transitions
- Mobile-friendly navigation
- Blog functionality
- Social media integration

## Project Structure

```
├── config.toml              # Hugo configuration
├── content/                 # Content files
│   ├── about/
│   ├── projects/
│   ├── community/
│   ├── activities/
│   ├── contact/
│   └── blog/
├── layouts/
│   ├── _default/
│   │   ├── baseof.html     # Base template
│   │   ├── list.html       # List template
│   │   └── single.html     # Single page template
│   ├── partials/
│   │   ├── header.html     # Navigation header
│   │   ├── footer.html     # Footer
│   │   ├── hero.html       # Hero section
│   │   ├── about-section.html
│   │   ├── projects-section.html
│   │   ├── activities-section.html
│   │   ├── blog-section.html
│   │   └── contact-section.html
│   └── index.html          # Homepage template
├── static/
│   ├── css/
│   │   └── style.css       # Custom styles
│   ├── js/
│   │   └── main.js         # Custom JavaScript
│   └── images/             # Images directory
└── README.md
```

## Local Development

### Prerequisites

- Hugo (Extended version recommended)
- Git

### Installation

1. Clone the repository:
```bash
git clone https://github.com/ranjithsiji/wikimedians-kerala-website.git
cd wikimedians-kerala-website
```

2. Run Hugo development server:
```bash
hugo server -D
```

3. Open your browser and visit `http://localhost:1313`

## Building for Production

To build the static site for production:

```bash
hugo --minify
```

The generated files will be in the `public/` directory.

## Deployment

### GitHub Pages

1. Update `baseURL` in `config.toml` to your GitHub Pages URL
2. Build the site: `hugo --minify`
3. Deploy the `public/` directory to the `gh-pages` branch

Or use GitHub Actions for automatic deployment (see `.github/workflows/hugo.yml`)

### Other Hosting

The site can be deployed to any static hosting service:
- Netlify
- Vercel
- Cloudflare Pages
- AWS S3
- Google Cloud Storage

## Customization

### Content

- Edit content files in `content/` directory
- Add blog posts in `content/blog/`
- Update navigation menu in `config.toml`

### Styling

- Modify `static/css/style.css` for custom styles
- Update color variables in `:root` section
- Bootstrap classes can be used throughout the templates

### Images

- Add images to `static/images/` directory
- Reference in content using `/images/filename.jpg`
- Recommended: Optimize images before uploading

## Contact Form

The contact form uses Formspree. To activate:

1. Sign up at [formspree.io](https://formspree.io)
2. Create a form and get your form ID
3. Update the form action in `layouts/partials/contact-section.html`:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

## Contributing

We welcome contributions! Please:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

Content: [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)
Code: MIT License

## Links

- **Website**: https://ranjithsiji.github.io/wikimedians-kerala-website/
- **Meta Wiki**: https://meta.wikimedia.org/wiki/Wikimedians_of_Kerala
- **Facebook**: https://www.facebook.com/WikimediansKL
- **Twitter**: https://twitter.com/WikimediansKL
- **Instagram**: https://www.instagram.com/wikimedians_kerala/

## Support

For issues and questions:
- Open an issue on GitHub
- Contact: wikikerala@gmail.com

---

Made with ❤️ by Wikimedians of Kerala