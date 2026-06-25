# Excellence Academy School Website

A modern, fully-functional school website built with HTML, CSS, and JavaScript. This website serves as a comprehensive digital presence for an educational institution.

## 📋 Features

### Pages Included

1. **Home (index.html)**
   - Eye-catching hero section
   - Feature highlights
   - Statistical achievements
   - Call-to-action sections

2. **About (about.html)**
   - School history and story
   - Mission, vision, and values
   - Leadership team information
   - Key achievements and awards

3. **Programs (programs.html)**
   - Early Childhood Education
   - Elementary School Programs
   - Middle School Programs
   - High School Programs
   - Special initiatives (IB, STEM, Arts, Sports)

4. **Contact (contact.html)**
   - Contact form with validation
   - Multiple contact information
   - Office hours
   - Frequently Asked Questions (FAQ)
   - Map placeholder section
   - Social media links

### Key Features

- **Responsive Design**: Fully responsive layout that works seamlessly on desktop, tablet, and mobile devices
- **Modern UI/UX**: Clean, professional design with smooth animations and transitions
- **Form Validation**: Client-side form validation with user-friendly error messages
- **Smooth Navigation**: Sticky navigation bar with smooth scrolling
- **Interactive Elements**: Hover effects, animated counters, scroll animations
- **Accessibility**: Semantic HTML structure for better accessibility
- **Fast Performance**: Optimized CSS and JavaScript for quick load times

## 🎨 Design Elements

- **Color Scheme**:
  - Primary: #2c3e50 (Dark Blue)
  - Secondary: #3498db (Light Blue)
  - Accent: #e74c3c (Red)

- **Typography**: Segoe UI, Tahoma, Geneva, Verdana, sans-serif
- **Animations**: Smooth fade-in effects, hover transformations
- **Shadows**: Subtle box shadows for depth

## 📱 Responsive Breakpoints

- Desktop: Full layout
- Tablet: Adjusted grid layouts
- Mobile: Single column layouts, compact navigation

## 🚀 Getting Started

### Prerequisites
- No server required - works with any web server
- Supported browsers: Chrome, Firefox, Safari, Edge

### Installation

1. Clone the repository
```bash
git clone https://github.com/Swarup2024web/school-website.git
cd school-website
```

2. Open in a web browser
```bash
# Simply open index.html in your browser
open index.html
```

Or use a local server:
```bash
# Using Python 3
python -m http.server 8000

# Using Python 2
python -m SimpleHTTPServer 8000

# Using Node.js (if installed)
npx http-server
```

Then navigate to `http://localhost:8000` in your browser.

## 📁 File Structure

```
school-website/
├── index.html          # Home page
├── about.html          # About page
├── programs.html       # Programs page
├── contact.html        # Contact page
├── style.css           # Styling
├── script.js           # Interactive features
└── README.md           # This file
```

## 🛠️ Customization

### Modify School Information
Edit the following files to customize content:
- **School Name**: Update "Excellence Academy" in all HTML files
- **Contact Info**: Edit contact details in `contact.html` and footer sections
- **Content**: Modify text in respective HTML pages

### Update Colors
Edit the CSS variables in `style.css`:
```css
:root {
    --primary-color: #2c3e50;
    --secondary-color: #3498db;
    --accent-color: #e74c3c;
    /* ... other variables ... */
}
```

### Add More Programs
Edit the `programs.html` file and add more program cards following the existing structure.

### Connect Form to Backend
In `script.js`, modify the `submitForm()` function to integrate with your backend:
```javascript
function submitForm(data) {
    // Send data to your backend API
    fetch('https://your-api.com/contact', {
        method: 'POST',
        body: JSON.stringify(data)
    })
    .then(response => response.json())
    .then(data => console.log('Success:', data));
}
```

## 🔄 Form Integration

The contact form currently simulates submission. To make it functional:

1. **Backend Option**: Set up a backend service (Node.js, Python, PHP, etc.) to receive form data
2. **Email Service**: Use services like:
   - Mailgun
   - SendGrid
   - AWS SES
   - Formspree (for static sites)

3. **Update the form action**:
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

## 📊 Analytics Integration

To add analytics, include tracking code in the pages:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

## 🔐 Security Considerations

- Validate all form inputs server-side
- Use HTTPS for all external requests
- Sanitize user input to prevent XSS attacks
- Implement CSRF protection for forms
- Keep dependencies updated

## 📱 Social Media Integration

Update social media links in `contact.html` footer section:

```html
<a href="https://facebook.com/yourpage" class="social-link">Facebook</a>
<a href="https://twitter.com/yourhandle" class="social-link">Twitter</a>
<a href="https://instagram.com/yourprofile" class="social-link">Instagram</a>
<a href="https://linkedin.com/company/yourpage" class="social-link">LinkedIn</a>
```

## 🌐 Deployment

### Netlify
1. Push code to GitHub
2. Connect GitHub repository to Netlify
3. Deploy automatically on push

### GitHub Pages
1. Push code to GitHub
2. Go to Settings > Pages
3. Select main branch as source
4. Site will be available at `username.github.io/school-website`

### Other Hosting
- Vercel
- AWS S3
- Heroku
- DigitalOcean

## 📧 Contact & Support

For questions or suggestions, please contact:
- Email: info@excellenceacademy.com
- Phone: +1 (555) 123-4567

## 📄 License

This project is open source and available under the MIT License.

## 🙏 Credits

Created with ❤️ for educational institutions worldwide.

---

**Last Updated**: June 2024

**Version**: 1.0.0

**Status**: Active Development

For updates and improvements, visit the [GitHub Repository](https://github.com/Swarup2024web/school-website)