# Onur Çelebi - Professional Academic Website

A modern, responsive academic website showcasing research, publications, and professional experience in economics, econometrics, and AI applications.

## 🌟 Features

- **Professional Academic Design**: Clean, modern interface optimized for academic professionals
- **Fully Responsive**: Mobile-first design that works perfectly on all devices
- **SEO Optimized**: Complete with meta tags, structured data (JSON-LD), and sitemap
- **Accessibility Compliant**: WCAG AA standards with semantic HTML and proper ARIA labels
- **Performance Optimized**: Lighthouse score 95+ across all categories
- **Dark/Light Theme**: Built-in theme toggle with user preference memory
- **GitHub Pages Ready**: No backend dependencies, deploys instantly

## 📁 Site Structure

```
/
├── index.html          # Homepage with hero, about, and contact
├── research.html       # Research areas and methodology
├── publications.html   # Academic publications and metrics
├── projects.html       # Software projects and technical skills
├── teaching.html       # Teaching experience and courses
├── blog.html          # Academic blog and insights
├── cv.html            # Comprehensive curriculum vitae
├── 404.html           # Custom error page
├── style.css          # Complete design system
├── sitemap.xml        # SEO sitemap
├── robots.txt         # Search engine directives
└── assets/            # Images and favicons
```

## 🚀 Quick Start

### For Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/onurcelebi96/onurcelebi96.github.io.git
   cd onurcelebi96.github.io
   ```

2. **Start a local server**
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   
   # Using PHP
   php -S localhost:8000
   ```

3. **Open in browser**
   ```
   http://localhost:8000
   ```

### For Deployment

The site is automatically deployed via GitHub Pages. Any push to the `main` branch will trigger a new deployment.

**Live URL**: https://onurcelebi96.github.io/

## 🎨 Design System

### Color Palette
- **Dark Theme**: Professional night mode with cyan/purple accents
- **Light Theme**: Clean academic look with indigo accents
- **Semantic Colors**: Consistent success, warning, and info states

### Typography
- **Primary Font**: Inter (body text)
- **Display Font**: Space Grotesk (headings)
- **Monospace**: JetBrains Mono (code)

### Components
- **Cards**: Elevated panels with hover animations
- **Buttons**: Primary, secondary, and ghost variants
- **Badges**: Status indicators for publications and projects
- **Timeline**: Chronological display for experience and education
- **Grid System**: Responsive layouts (2, 3, 4 column)

## 📝 Content Management

### Adding Publications

Edit `publications.html` to add new academic papers:

```html
<article class="publication">
  <h3 class="publication-title">Your Paper Title</h3>
  <p class="publication-authors"><strong>Çelebi, O.</strong> & Co-author</p>
  <p class="publication-venue">Journal Name, Vol. X, No. Y, Year</p>
  <p>Brief description of the research...</p>
  <div class="publication-links">
    <a href="link-to-paper" class="btn btn-primary">📄 Read Paper</a>
    <span class="badge badge-success">Published</span>
  </div>
  <div class="tags">
    <span>Tag1</span><span>Tag2</span>
  </div>
</article>
```

### Adding Blog Posts

Add new blog entries to `blog.html`:

```html
<article class="blog-card">
  <div class="blog-card-image">🔬</div>
  <div class="blog-card-content">
    <div class="blog-card-date">Month DD, YYYY</div>
    <h3 class="blog-card-title">Post Title</h3>
    <div class="blog-card-excerpt">Brief excerpt...</div>
    <div class="tags">
      <span>Category</span>
    </div>
  </div>
</article>
```

### Adding Projects

Update `projects.html` for new software projects:

```html
<div class="card">
  <h3>🔍 Project Title</h3>
  <p>Project description...</p>
  <div class="tags">
    <span>Technology</span>
  </div>
  <div class="card-actions">
    <a href="github-link" class="btn btn-primary">View Code</a>
    <span class="badge badge-success">Active</span>
  </div>
</div>
```

## 🛠️ Customization

### Changing Colors

Edit the CSS variables in `style.css`:

```css
:root {
  --brand: #7dd3fc;      /* Primary accent */
  --brand-2: #c084fc;    /* Secondary accent */
  --bg: #0f1116;         /* Background */
  --panel: #171b23;      /* Card background */
  --text: #ecf0f7;       /* Text color */
  --muted: #b1b7c6;      /* Muted text */
}
```

### Adding New Pages

1. Create new HTML file following the existing template structure
2. Add navigation link to all existing pages
3. Update `sitemap.xml` with the new URL
4. Test responsive behavior and accessibility

### Modifying Layout

The design uses CSS Grid and Flexbox for layouts:
- `.grid-2`, `.grid-3`, `.grid-4` for responsive grids
- `.section` for consistent vertical spacing
- `.container` for content width constraints

## 🔍 SEO & Analytics

### Included SEO Features
- **Meta Tags**: Title, description, keywords for every page
- **Open Graph**: Facebook/LinkedIn sharing optimization
- **Twitter Cards**: Twitter sharing optimization
- **Structured Data**: JSON-LD for search engines
- **Sitemap**: XML sitemap for search crawlers
- **Canonical URLs**: Prevent duplicate content issues

### Analytics Setup
The site includes Plausible Analytics (privacy-focused):

```html
<script defer data-domain="onurcelebi96.github.io" src="https://plausible.io/js/script.js"></script>
```

Replace with your preferred analytics solution.

## ♿ Accessibility

### Compliance Features
- **Semantic HTML**: Proper heading hierarchy and landmarks
- **ARIA Labels**: Screen reader support for interactive elements
- **Keyboard Navigation**: Full site navigation without mouse
- **Focus Indicators**: Visible focus states for all interactive elements
- **Color Contrast**: WCAG AA compliant color combinations
- **Skip Links**: Quick navigation for screen readers

### Testing Accessibility
```bash
# Install accessibility testing tools
npm install -g @axe-core/cli

# Run accessibility audit
axe --url http://localhost:8000
```

## 🚀 Performance

### Optimization Features
- **Optimized Images**: WebP format with fallbacks
- **Font Loading**: Preconnected font resources
- **CSS Minification**: Compressed stylesheets
- **Lazy Loading**: Images load when needed
- **Caching Headers**: Optimized for GitHub Pages

### Performance Testing
```bash
# Install Lighthouse CLI
npm install -g lighthouse

# Run performance audit
lighthouse http://localhost:8000 --output html --output-path report.html
```

## 🔧 Browser Support

- **Modern Browsers**: Chrome 88+, Firefox 84+, Safari 14+, Edge 88+
- **Mobile**: iOS Safari 14+, Chrome Mobile 88+
- **Fallbacks**: Graceful degradation for older browsers

## 📱 Responsive Breakpoints

```css
/* Mobile First Approach */
@media (max-width: 520px)  { /* Mobile */ }
@media (max-width: 640px)  { /* Small tablets */ }
@media (max-width: 768px)  { /* Tablets */ }
@media (max-width: 860px)  { /* Small desktop */ }
@media (max-width: 1024px) { /* Desktop */ }
```

## 🐛 Troubleshooting

### Common Issues

**Theme not persisting**
- Check if localStorage is enabled in browser
- Verify script is loading without errors

**Images not loading**
- Ensure correct file paths (case-sensitive on GitHub Pages)
- Check if images are in the correct format

**Mobile menu not working**
- Verify JavaScript is enabled
- Check console for script errors

### Development Tools

```bash
# Validate HTML
npx html-validate *.html

# Check links
npx broken-link-checker http://localhost:8000

# Optimize images
npx imagemin-cli assets/*.{jpg,png} --out-dir=assets/optimized
```

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

While this is a personal website, suggestions and improvements are welcome:

1. Fork the repository
2. Create a feature branch
3. Submit a pull request with detailed description

## 📞 Contact

**Onur Çelebi**
- Email: celebionur@protonmail.ch
- LinkedIn: [linkedin.com/in/onurcelebi96](https://www.linkedin.com/in/onurcelebi96/)
- GitHub: [github.com/onurcelebi96](https://github.com/onurcelebi96)
- X (Twitter): [@onr_clb](https://x.com/onr_clb)

---

Built with ❤️ for the academic community. Combines modern web standards with professional design to create an accessible, performant, and SEO-optimized academic presence.
