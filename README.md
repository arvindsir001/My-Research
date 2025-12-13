# Academic Personal Website

A clean, professional academic website template inspired by modern research portfolio designs. Built with pure HTML/CSS for easy deployment on GitHub Pages.

## Features

- 📱 Fully responsive design
- 🎨 Clean, academic aesthetic with elegant typography
- 📄 Multiple pages: Home, About, Publications
- 🔗 Social media integration
- ⚡ Fast loading with no dependencies
- 🎯 SEO-friendly structure

## Quick Start

1. **Fork this repository** or create a new GitHub repository

2. **Enable GitHub Pages:**
   - Go to repository Settings
   - Navigate to Pages section
   - Select "Deploy from branch"
   - Choose "main" branch and "/" (root) folder
   - Click Save

3. **Customize your content:**
   - Edit `index.html`, `about.html`, and `publications.html`
   - Replace placeholder text with your information
   - Update social media links and email addresses

4. **Add your images:**
   - Create an `images` folder in the repository
   - Add your profile photo as `profile.jpg`
   - Add research thumbnails (e.g., `research1.jpg`, `pub2025-1.jpg`)
   - Add your institution logo as `institution-logo.png`

5. **Access your site:**
   - Your website will be available at: `https://yourusername.github.io/`
   - Or if using a custom repository name: `https://yourusername.github.io/repository-name/`

## File Structure

```
.
├── index.html          # Home page with introduction and spotlight research
├── about.html          # About page with detailed bio, education, awards
├── publications.html   # Publications list organized by year
├── styles.css          # Main stylesheet
├── README.md          # This file
└── images/            # Directory for all images
    ├── profile.jpg
    ├── institution-logo.png
    ├── research1.jpg
    ├── pub2025-1.jpg
    └── ...
```

## Customization Guide

### Personal Information

Update all instances of placeholder text:
- Replace "Your Name" with your actual name
- Update email addresses
- Add your social media handles (GitHub, Twitter, LinkedIn, ORCID)
- Update institution names and positions

### Images

Recommended image sizes:
- **Profile photo**: 560×560px (280×280px displayed)
- **Research thumbnails**: 600×400px
- **Publication images**: 400×300px
- **Institution logo**: 240×120px (transparent background recommended)

### Colors

The site uses CSS variables for easy color customization. Edit `styles.css`:

```css
:root {
    --primary-color: #1a1a1a;      /* Main text color */
    --link-color: #0066cc;         /* Link color */
    --link-hover: #004499;         /* Link hover color */
    --bg-color: #ffffff;           /* Background */
}
```

### Typography

The site uses:
- **Crimson Pro** for headings (serif)
- **Source Sans 3** for body text (sans-serif)

To change fonts, update the Google Fonts import in the `<head>` section of each HTML file.

### Adding Publications

To add a new publication in `publications.html`:

```html
<div class="publication-item">
    <div class="pub-image">
        <img src="images/your-paper.jpg" alt="Paper title">
    </div>
    <div class="pub-content">
        <h3>Your Paper Title</h3>
        <p class="pub-authors"><strong>Your Name</strong>, Co-Authors</p>
        <p class="pub-venue"><em>Conference Name 2025</em></p>
        <div class="pub-links">
            <a href="#" class="btn-paper">PDF</a>
            <a href="#" class="btn-code">Code</a>
        </div>
    </div>
</div>
```

### Adding Updates

Add news items in `index.html` under the Updates section:

```html
<div class="update-item">
    <strong>[Month Year]</strong> Brief description of the update.
</div>
```

## Advanced Customization

### Adding New Pages

1. Create a new HTML file (e.g., `teaching.html`)
2. Copy the header and footer from an existing page
3. Add a navigation link in all pages:
   ```html
   <a href="teaching.html">Teaching</a>
   ```

### Custom Domain

To use a custom domain:
1. Purchase a domain from a registrar
2. Add a `CNAME` file to your repository with your domain name
3. Configure DNS settings at your registrar
4. Follow [GitHub's custom domain guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## License

This template is free to use for academic and personal websites. No attribution required, but appreciated!

## Credits

- Inspired by academic portfolio websites
- Typography: Google Fonts (Crimson Pro, Source Sans 3)
- Built with semantic HTML5 and modern CSS

## Support

For issues or questions:
1. Check the customization guide above
2. Review the HTML/CSS comments in the code
3. Search GitHub Issues
4. Create a new issue if needed

## Tips for Success

- **Keep it updated**: Regularly add new publications and updates
- **Optimize images**: Compress images for faster loading
- **Mobile-first**: Test on mobile devices
- **Accessibility**: Use descriptive alt text for images
- **SEO**: Update page titles and meta descriptions
- **Backups**: Keep your source files backed up

---

Built with ❤️ for researchers and academics
