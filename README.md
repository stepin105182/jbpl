# Jayalakshmi Buildtech Pvt. Ltd. - Corporate Website

A modern, professional, and visually striking corporate website for Jayalakshmi Buildtech Pvt. Ltd., a leading telecom infrastructure company in India.

## Features

- **Modern Design**: Clean, professional UI with bold typography and smooth animations
- **Fully Responsive**: Optimized for desktop, tablet, and mobile devices
- **Smooth Interactions**: Scroll animations, parallax effects, and hover transitions
- **SEO Optimized**: Semantic HTML and meta tags for better search engine visibility
- **Performance**: Lazy loading, debounced scroll events, and optimized animations
- **Accessibility**: ARIA labels and reduced motion support

## Project Structure

```
api_qa/
├── index.html          # Main HTML file
├── styles.css          # Complete styling
├── script.js           # JavaScript interactions
├── README.md          # Documentation
└── static/
    ├── logo.svg        # Company logo (SVG - replace with your logo)
    └── logo.png        # Alternative logo format
```

## Sections Overview

### 1. **Navigation Bar**
- Fixed navigation with smooth scroll
- Mobile-responsive hamburger menu
- Active link highlighting based on scroll position
- Professional logo and company branding

### 2. **Hero Section**
- Full-screen hero with gradient background
- Compelling headline and supporting text
- Call-to-action buttons
- Scroll indicator with animation

### 3. **About Us**
- Company introduction and mission
- Key statistics (Projects, States, Satisfaction)
- Professional imagery placeholder
- Grid layout for optimal readability

### 4. **Core Expertise**
- 6 service cards with custom SVG icons
- Hover effects and animations
- Detailed descriptions of each service
- Icon-based grid layout

### 5. **Projects Executed**
- Timeline design with visual markers
- 5 major projects highlighted
- Project tags and highlight badges
- Smooth fade-in animations

### 6. **Why Choose Us**
- Checklist-style benefits
- Visual card with gradient background
- Hover interactions
- Two-column responsive layout

### 7. **Commitment Section**
- Bold statement section
- Gradient background
- Call-to-action button

### 8. **Footer**
- Company information
- Quick links navigation
- Contact details placeholder
- Professional multi-column layout

## Customization Guide

### Colors

Update the color scheme in `styles.css` (lines 11-19):

```css
:root {
    --primary-blue: #1e40af;
    --deep-blue: #1e3a8a;
    --accent-teal: #14b8a6;
    --accent-orange: #f97316;
    /* Add your custom colors */
}
```

### Typography

Change fonts in `styles.css` (lines 21-22) or update the Google Fonts link in `index.html`:

```css
:root {
    --font-primary: 'Inter', sans-serif;
    --font-heading: 'Poppins', sans-serif;
}
```

### Logo Replacement

Replace the dummy logo with your actual company logo:

1. **Recommended**: Save your logo as `static/logo.png` or `static/logo.svg`
2. The logo will automatically appear in the navigation bar
3. Recommended size: 60x60 pixels or 200x200 pixels (PNG), any size (SVG)
4. Transparent background recommended for best results

```html
<!-- In index.html, the logo is referenced here: -->
<img src="static/logo.svg" alt="Jayalakshmi Buildtech Logo" class="logo-image">
```

### Content

1. **Company Name**: Update in `index.html` - search for "JAYALAKSHMI BUILDTECH"
2. **Contact Information**: Update footer section with actual contact details
3. **Images**: Replace SVG placeholders with actual images
4. **Projects**: Add/remove timeline items in the Projects section
5. **Statistics**: Update numbers in the About section

### Adding Real Images

Replace the SVG placeholder in the About section:

```html
<!-- Replace this: -->
<div class="image-placeholder">
    <svg>...</svg>
</div>

<!-- With this: -->
<div class="about-image">
    <img src="path/to/your/image.jpg" alt="Description">
</div>
```

For optimal performance, use:
- WebP format for modern browsers
- JPEG for compatibility
- Recommended size: 800x600px
- Compress images before uploading

### Adding Background Images to Hero

Update the hero section in `styles.css`:

```css
.hero {
    background: linear-gradient(135deg, rgba(30, 58, 138, 0.9), rgba(30, 64, 175, 0.8)),
                url('path/to/hero-image.jpg') center/cover no-repeat;
}
```

## JavaScript Features

### 1. **Mobile Menu**
- Toggle navigation on mobile devices
- Automatic close on link click

### 2. **Scroll Effects**
- Navbar shadow on scroll
- Active navigation link highlighting
- Smooth scroll to sections

### 3. **Animations**
- Fade-in animations for cards and sections
- Counter animation for statistics
- Timeline reveal on scroll
- Parallax effect on hero section

### 4. **Scroll to Top Button**
- Auto-generated button
- Appears after scrolling 500px
- Smooth scroll to top

### 5. **Performance Optimizations**
- Debounced scroll events
- Intersection Observer API for lazy animations
- Reduced motion support

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Deployment

### Option 1: Simple Hosting
Upload all files to any web hosting service:
- GitHub Pages
- Netlify
- Vercel
- Traditional web hosting (cPanel, etc.)

### Option 2: GitHub Pages
1. Create a GitHub repository
2. Push all files to the repository
3. Go to Settings > Pages
4. Select branch and root folder
5. Your site will be live at `https://yourusername.github.io/repository-name`

### Option 3: Netlify
1. Drag and drop the entire folder to Netlify
2. Your site will be live instantly
3. Connect to GitHub for automatic deployments

## Performance Tips

1. **Optimize Images**
   - Use modern formats (WebP, AVIF)
   - Compress images (TinyPNG, ImageOptim)
   - Serve responsive images

2. **Minify Assets**
   - Minify CSS: Use cssnano or clean-css
   - Minify JavaScript: Use Terser or UglifyJS
   - Minify HTML: Use html-minifier

3. **Enable Caching**
   - Set proper cache headers
   - Use CDN for static assets

4. **Add Analytics**
   - Google Analytics
   - Microsoft Clarity
   - Plausible Analytics

## SEO Optimization

### Current Implementation
- Semantic HTML5 structure
- Meta description and keywords
- Proper heading hierarchy (H1, H2, H3)
- Alt text for images (when added)

### Additional Recommendations
1. Add Open Graph tags for social sharing
2. Include structured data (Schema.org)
3. Create a sitemap.xml
4. Add robots.txt
5. Submit to Google Search Console

### Example Open Graph Tags
Add to `<head>` section in `index.html`:

```html
<meta property="og:title" content="Jayalakshmi Buildtech - Telecom Infrastructure">
<meta property="og:description" content="Leading telecom infrastructure company in India">
<meta property="og:image" content="path/to/social-image.jpg">
<meta property="og:url" content="https://yourwebsite.com">
<meta property="og:type" content="website">
```

## Contact Form Integration

To add a working contact form, integrate with:

1. **Formspree**: Simple form backend
   ```html
   <form action="https://formspree.io/f/yourformid" method="POST">
   ```

2. **Netlify Forms**: Built-in form handling
   ```html
   <form name="contact" method="POST" data-netlify="true">
   ```

3. **Google Forms**: Free and simple
4. **Custom Backend**: PHP, Node.js, Python

## Maintenance

### Regular Updates
- Update copyright year (auto-updates via JavaScript)
- Add new projects to timeline
- Update statistics and achievements
- Refresh images and content

### Performance Monitoring
- Use Lighthouse for audits
- Monitor Core Web Vitals
- Test on real devices

## Support

For questions or customization requests:
- Email: info@jayalakshmibuildtech.in
- Review the code comments for guidance
- Check browser console for debugging

## Credits

- **Design**: Custom corporate design
- **Icons**: Custom SVG icons
- **Fonts**: Google Fonts (Inter, Poppins)
- **Animations**: CSS3 and Intersection Observer API

## License

Proprietary - All rights reserved by Jayalakshmi Buildtech Pvt. Ltd.

---

**Built with modern web technologies for optimal performance and user experience.**

For enterprise-grade hosting and maintenance, consult with a professional web development team.
