# Professional Portfolio Website

A modern, dark-themed portfolio website with sidebar navigation, built with HTML, CSS, and JavaScript.

## Features

- **Dark Theme Design** - Modern minimalist dark aesthetic with neon accents
- **Sidebar Navigation** - Fixed sidebar navigation for easy access to all sections
- **Fully Responsive Design** - Works seamlessly on desktop, tablet, and mobile devices
- **Smooth Animations** - Scroll-triggered animations and transitions
- **Interactive Elements** - Animated skill bars, project cards, and counter animations
- **Contact Form** - Functional contact form with validation
- **Monospace Typography** - Unique code-inspired typography using JetBrains Mono
- **Card-Based Layout** - Modern card-based design for projects and experience

## Sections

1. **Hero Section** - Eye-catching introduction with call-to-action buttons
2. **About** - Personal introduction and statistics
3. **Experience** - Professional timeline with work history
4. **Skills** - Technical skills with progress bars and tags
5. **Projects** - Showcase of featured projects
6. **Contact** - Contact form and social media links

## Quick Start

1. Open `index.html` in your web browser
2. Customize the content with your personal information
3. Update colors, fonts, and styling in `styles.css`
4. Modify interactive features in `script.js`

## Customization Guide

### 1. Update Personal Information

#### In `index.html`:

**Hero Section:**
```html
<span class="name">Henrik Gerard Velnom</span>
<p class="hero-subtitle">Your Professional Title</p>
<p class="hero-description">Your personal description</p>
```

**About Section:**
- Update the about text with your personal story
- Modify statistics (years of experience, projects, etc.)

**Experience Section:**
- Update timeline items with your work history
- Add or remove experience entries
- Update dates, titles, companies, and descriptions

**Skills Section:**
- Update skill names and proficiency levels (data-width attribute)
- Modify skill categories and tags

**Projects Section:**
- Update project cards with your actual projects
- Add project images, descriptions, and links
- Update technology tags

**Contact Section:**
- Update email, phone, and location
- Add your social media links
- Configure form submission endpoint

### 2. Update Colors and Styling

#### In `styles.css`:

**CSS Variables** (at the top of the file):
```css
:root {
    --primary-color: #6366f1;      /* Main brand color */
    --secondary-color: #8b5cf6;     /* Secondary color */
    --text-primary: #1f2937;         /* Main text color */
    --text-secondary: #6b7280;      /* Secondary text color */
    --bg-primary: #ffffff;          /* Main background */
    --bg-secondary: #f9fafb;        /* Secondary background */
}
```

### 3. Update Social Media Links

#### In `index.html`:

Find all social media links and update the `href` attributes:
```html
<a href="https://linkedin.com/in/yourprofile" aria-label="LinkedIn">
<a href="https://github.com/yourusername" aria-label="GitHub">
<a href="https://twitter.com/yourhandle" aria-label="Twitter">
```

### 4. Add Your Photo

Replace the placeholder in the About section:
- Option 1: Add an `<img>` tag with your photo
- Option 2: Replace the `.image-placeholder` div with your image

### 5. Configure Contact Form

The contact form currently shows a success message. To make it functional:

1. **Backend Integration:**
   - Set up a backend endpoint to handle form submissions
   - Update the form action in `script.js`:
   ```javascript
   contactForm.addEventListener('submit', async (e) => {
       e.preventDefault();
       const formData = new FormData(contactForm);
       const response = await fetch('YOUR_API_ENDPOINT', {
           method: 'POST',
           body: formData
       });
       // Handle response
   });
   ```

2. **Email Service (Alternative):**
   - Use services like Formspree, EmailJS, or Netlify Forms
   - Update the form action attribute accordingly

### 6. Add Project Images

Replace the gradient backgrounds in project cards with actual images:
```html
<div class="project-image" style="background-image: url('path/to/image.jpg');">
```

### 7. Update Skill Levels

In the Skills section, modify the `data-width` attribute:
```html
<div class="skill-progress" data-width="90"></div>
```
Values range from 0-100 (percentage).

## File Structure

```
portfolio/
├── index.html          # Main HTML file
├── styles.css          # All CSS styles
├── script.js           # JavaScript functionality
└── README.md           # This file
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance Tips

1. **Optimize Images:**
   - Use WebP format when possible
   - Compress images before adding to projects
   - Use appropriate image sizes

2. **Minify Assets:**
   - Minify CSS and JavaScript for production
   - Consider using a build tool like Webpack or Vite

3. **Lazy Loading:**
   - Add `loading="lazy"` to images
   - Implement lazy loading for animations

## Deployment

### Option 1: GitHub Pages
1. Push your code to a GitHub repository
2. Go to Settings > Pages
3. Select your branch and deploy

### Option 2: Netlify
1. Drag and drop your folder to Netlify
2. Or connect your GitHub repository

### Option 3: Vercel
1. Install Vercel CLI
2. Run `vercel` in your project directory

### Option 4: Traditional Hosting
1. Upload all files via FTP
2. Ensure `index.html` is in the root directory

## Customization Checklist

- [ ] Update name and title
- [ ] Replace placeholder content with your information
- [ ] Update experience timeline
- [ ] Modify skills and proficiency levels
- [ ] Add your projects with descriptions
- [ ] Update social media links
- [ ] Add your photo
- [ ] Configure contact form
- [ ] Update color scheme (if desired)
- [ ] Add project images
- [ ] Test on multiple devices
- [ ] Deploy to hosting platform

## Additional Features You Can Add

- **Blog Section** - Add a blog or articles section
- **Testimonials** - Add client testimonials
- **Certifications** - Showcase your certifications
- **Resume Download** - Add a downloadable resume button
- **Dark Mode** - Implement a dark/light theme toggle
- **Language Switcher** - Add multi-language support
- **Analytics** - Integrate Google Analytics or similar
- **Animations** - Add more advanced animations with libraries like GSAP

## Support

For customization help or questions, refer to:
- HTML documentation: [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML)
- CSS documentation: [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS)
- JavaScript documentation: [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

## License

This portfolio template is free to use and modify for personal or commercial projects.

---

**Note:** Remember to update all placeholder content with your actual information before deploying your portfolio!

