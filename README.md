# Eslam Abdelrahman - Professional Academic Website

A modern, professional multi-page website designed to showcase your research, experience, and academic achievements.

## 🌟 Features

- **Modern Design**: Clean, professional aesthetic with smooth animations and card lift effects
- **Fully Responsive**: Optimized for desktop, tablet, and mobile devices
- **Multi-Page Structure**: Separate pages for different content sections
- **Interactive Elements**: Hover effects, smooth transitions, and animated components
- **SEO-Friendly**: Proper HTML structure and meta tags
- **Fast Loading**: Optimized CSS and minimal dependencies

## 📁 File Structure

```
├── index.html          # Home page with hero section and highlights
├── publications.html   # Complete list of publications organized by year
├── experience.html     # Professional experience timeline
├── education.html      # Academic background
├── service.html        # Teaching and academic service
├── awards.html         # Awards and recognition
├── contact.html        # Contact information and social links
├── styles.css          # Main stylesheet with all animations
├── script.js           # JavaScript for interactions and animations
└── README.md          # This file
```

## 🎨 Design Features

### Typography
- **Headings**: Playfair Display (serif) - elegant and professional
- **Body**: IBM Plex Sans - modern and readable
- Custom font weights and sizes for hierarchy

### Color Scheme
- **Primary**: Deep blue (#1a365d) - professional and trustworthy
- **Accent**: Warm orange (#d97706) - energetic and attention-grabbing
- **Text**: Carefully chosen grays for optimal readability
- **Backgrounds**: Light gradients for subtle depth

### Interactive Elements
- **Clickable highlight cards** on home page (Education, Publications, Recognition)
- **Conference/institution logos** throughout the site
- **Filter buttons** on publications page (First Author vs Collaborations)
- **Smooth hover effects** on all cards

### Animations
- Fade-in on scroll for content sections
- Lift-up effect on cards (hover)
- Smooth page transitions
- Timeline animations
- Navigation bar effects

## 🚀 How to Use

### Option 1: GitHub Pages (Recommended)
1. Create a new repository on GitHub
2. Upload all files to the repository
3. Go to Settings → Pages
4. Select main branch as source
5. Your site will be live at `https://yourusername.github.io/repository-name`

### Option 2: Custom Domain
1. Upload files to your web hosting service
2. Point your domain to the hosting
3. Access via your custom domain

### Option 3: Local Preview
1. Download all files to a folder
2. Open `index.html` in a web browser
3. All pages will work locally

## ✏️ Customization Guide

### Adding Your Photo
Replace the placeholder SVG in `index.html` (line ~60) with:
```html
<img src="your-photo.jpg" alt="Eslam Abdelrahman" style="width: 100%; border-radius: 50%;">
```

### Adding Logos
Create a `logos/` folder and add your institution/conference logos:
- **Conference logos**: iclr-logo.png, neurips-logo.png, iccv-logo.png, emnlp-logo.png, aaai-logo.png, wacv-logo.png, eccv-logo.png, under-review.png
- **Company logos**: adobe-logo.png, valeo-logo.png, techibees-logo.png
- **University logos**: kaust-logo.png, cairo-university-logo.png
- Recommended size: 200x200px (will auto-scale to fit)
- Format: PNG with transparent background works best

### Using the Publication Filter
The publications page has three filter buttons:
- **All Papers**: Shows everything
- **First Author**: Shows only papers where you're the first/lead author
- **Collaborations**: Shows papers where you're a co-author
- Counts update automatically based on `data-author` attribute in HTML

### Updating Publications
1. Open `publications.html`
2. Find the year section or create a new one
3. Copy an existing publication card structure
4. Update the details (title, authors, venue, links)

### Changing Colors
Open `styles.css` and modify the CSS variables at the top:
```css
:root {
    --primary-color: #1a365d;  /* Change main color */
    --accent-color: #d97706;   /* Change accent color */
    /* ... other variables ... */
}
```

### Adding New Pages
1. Create a new HTML file
2. Copy the structure from an existing page
3. Update the navigation in all pages to include the new link
4. Add your content in the main section

### Updating Links
Search for placeholder links (marked with `#`) and replace with actual URLs:
- Paper links
- Project websites
- Code repositories
- Demo links

## 📝 Content Updates

### Home Page (index.html)
- Hero title and subtitle
- Statistics (publications, venues, years)
- About section
- Featured publications
- News timeline

### Publications (publications.html)
- All papers organized by year
- Venue badges and types
- Author lists (your name is highlighted)
- Links to papers, code, and demos

### Experience (experience.html)
- Professional positions
- Achievements and responsibilities
- Timeline layout with visual appeal

### Education (education.html)
- Degrees and institutions
- GPA and thesis information
- Advisors and recognition

### Service (service.html)
- Teaching experience
- Conference reviewing
- Workshop organization
- Community service

### Awards (awards.html)
- Recognition and honors
- Patent information
- Competition wins

### Contact (contact.html)
- Email and phone
- Office location
- Social media links
- Call-to-action section

## 🎯 Best Practices

1. **Keep It Updated**: Regularly add new publications and achievements
2. **Add Real Links**: Replace all `#` placeholder links with actual URLs
3. **Optimize Images**: If you add photos, compress them for faster loading
4. **Test Responsiveness**: Check the site on mobile devices
5. **Proofread**: Ensure all text is accurate and professional
6. **Analytics**: Consider adding Google Analytics to track visitors

## 🔧 Technical Details

- **No dependencies**: Pure HTML, CSS, and JavaScript
- **Cross-browser compatible**: Works on all modern browsers
- **Mobile-first**: Responsive design prioritizes mobile experience
- **Accessibility**: Semantic HTML and proper ARIA labels
- **Performance**: Minimal CSS/JS, optimized animations

## 📱 Responsive Breakpoints

- **Desktop**: 1200px and above
- **Tablet**: 768px - 1199px
- **Mobile**: Below 768px

## 🎨 Customization Tips

### To Make Cards More/Less Elevated
Adjust the hover transform in `styles.css`:
```css
.pub-card:hover {
    transform: translateY(-8px); /* Increase number for more lift */
}
```

### To Change Animation Speed
Modify transition variables:
```css
--transition-fast: 0.15s ease;
--transition-normal: 0.3s ease;
--transition-slow: 0.5s ease;
```

### To Add More Sections
Copy an existing section structure and modify the content:
```html
<section class="new-section">
    <div class="container">
        <div class="section-header">
            <span class="section-tag">Tag</span>
            <h2 class="section-title">Title</h2>
        </div>
        <!-- Your content -->
    </div>
</section>
```

## 📞 Support

For questions or issues with the website:
- Review the code comments in each file
- Check browser console for JavaScript errors
- Ensure all files are in the same directory

## 🎉 Ready to Launch!

Your professional academic website is ready to impress recruiters and collaborators. All pages are complete with your actual information from your CV. Simply:

1. Add your photo to the home page
2. Replace placeholder links with actual URLs
3. Upload to your hosting/GitHub
4. Share your new website!

Good luck with your internship applications! 🚀
