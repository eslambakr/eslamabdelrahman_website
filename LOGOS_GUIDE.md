# Logo Implementation Guide

This guide explains where and how to add logos throughout your website.

## 📁 Folder Structure

Create a `logos/` folder in the same directory as your HTML files:

```
your-website/
├── index.html
├── publications.html
├── experience.html
├── education.html
├── ...
└── logos/
    ├── kaust-logo.png
    ├── adobe-logo.png
    ├── iclr-logo.png
    └── ...
```

## 🎯 Required Logos

### Conference Logos (Publications & News)
- `iclr-logo.png` - ICLR (International Conference on Learning Representations)
- `neurips-logo.png` - NeurIPS (Neural Information Processing Systems)
- `iccv-logo.png` - ICCV (International Conference on Computer Vision)
- `cvpr-logo.png` - CVPR (Computer Vision and Pattern Recognition)
- `emnlp-logo.png` - EMNLP (Empirical Methods in Natural Language Processing)
- `aaai-logo.png` - AAAI (Association for the Advancement of Artificial Intelligence)
- `eccv-logo.png` - ECCV (European Conference on Computer Vision)
- `wacv-logo.png` - WACV (Winter Conference on Applications of Computer Vision)
- `under-review.png` - For papers under review (use a generic "Under Review" icon or clock icon)

### Company Logos (Experience)
- `adobe-logo.png` - Adobe
- `valeo-logo.png` - Valeo
- `techibees-logo.png` - TechiBees
- `cairo-university-logo.png` - Cairo University (for research position)

### University Logos (Education)
- `kaust-logo.png` - King Abdullah University of Science and Technology
- `cairo-university-logo.png` - Cairo University

## 📐 Logo Specifications

### Recommended Dimensions
- **Size**: 200x200px to 400x400px (will auto-scale to fit containers)
- **Format**: PNG with transparent background preferred
- **Style**: Official logos in color or monochrome

### Where to Find Logos
1. **Official Sources**: 
   - Conference websites (usually in "Media Kit" or "About" sections)
   - Company press/media pages
   - University branding guidelines
2. **Design Resources**:
   - Wikimedia Commons (for many institutions)
   - Official brand portals
   - LinkedIn company pages (right-click logo, save image)

## 🔧 Implementation Details

### 1. Home Page - News Section

Each news item has a logo next to the date:

```html
<div class="news-item">
    <div class="news-date">
        <div class="date-text">Dec 2025</div>
        <div class="news-logo">
            <img src="logos/adobe-logo.png" alt="Adobe" class="news-logo-img">
        </div>
    </div>
    <div class="news-content">
        <h3>News Title</h3>
        <p>Description...</p>
    </div>
</div>
```

**Logo appears in**: 60x60px container (auto-scales)
**Files needed**: adobe-logo.png, iclr-logo.png, emnlp-logo.png, iccv-logo.png, kaust-logo.png, under-review.png

### 2. Publications Page - Conference Logos

Each publication card has a conference logo in the top-right corner:

```html
<div class="publication-item" data-author="first-author">
    <div class="pub-conference-logo">
        <img src="logos/iclr-logo.png" alt="ICLR" class="conf-logo-img">
    </div>
    <div class="pub-header-info">
        <!-- Rest of publication info -->
    </div>
</div>
```

**Logo appears in**: 50x50px container (auto-scales)
**Files needed**: All conference logos listed above

### 3. Experience Page - Company Logos

Each experience timeline card has a company logo in the top-right:

```html
<div class="timeline-content">
    <div class="company-logo">
        <img src="logos/adobe-logo.png" alt="Adobe" class="company-logo-img">
    </div>
    <div class="company-header">
        <!-- Company info -->
    </div>
</div>
```

**Logo appears in**: 50x50px container (auto-scales)
**Files needed**: adobe-logo.png, valeo-logo.png, cairo-university-logo.png, techibees-logo.png

### 4. Education Page - University Logos

Each education card has a university logo in the top-right:

```html
<div class="education-card">
    <div class="university-logo">
        <img src="logos/kaust-logo.png" alt="KAUST" class="university-logo-img">
    </div>
    <div class="degree-header">
        <!-- Degree info -->
    </div>
</div>
```

**Logo appears in**: 60x60px container (auto-scales)
**Files needed**: kaust-logo.png, cairo-university-logo.png

## 🎨 Logo Styling Tips

### If Logo Looks Too Small
The logos auto-scale to fit their containers. If a logo appears too small:
1. Ensure the logo has minimal whitespace around it
2. Use a square crop of the logo
3. For wide logos, crop to include just the icon/symbol

### If Logo Looks Pixelated
1. Use a higher resolution source (at least 200x200px)
2. Download the vector version (.svg or .eps) and convert to high-res PNG
3. Try PNG at 2x or 3x the display size

### If Logo Doesn't Match Style
1. Consider using monochrome versions for consistency
2. Adjust opacity in CSS if needed
3. Use official brand colors when available

## 🚀 Quick Setup Steps

1. **Create logos folder**:
   ```bash
   mkdir logos
   ```

2. **Download logos from official sources**

3. **Rename files** to match the exact names in the HTML:
   - `iclr-logo.png` (not `ICLR_Logo.png` or `iclr.png`)
   - Names are case-sensitive on some servers

4. **Test locally**: Open your website and check that all logos appear

5. **Upload with your website** when deploying

## 📝 Logo Checklist

Before deploying, verify you have:

### Essential Logos (Home Page)
- [ ] adobe-logo.png
- [ ] iclr-logo.png
- [ ] emnlp-logo.png
- [ ] iccv-logo.png
- [ ] kaust-logo.png
- [ ] under-review.png

### Publications (Based on your papers)
- [ ] iclr-logo.png
- [ ] neurips-logo.png
- [ ] iccv-logo.png
- [ ] emnlp-logo.png
- [ ] aaai-logo.png
- [ ] eccv-logo.png
- [ ] wacv-logo.png
- [ ] under-review.png

### Experience
- [ ] adobe-logo.png
- [ ] valeo-logo.png
- [ ] cairo-university-logo.png
- [ ] techibees-logo.png

### Education
- [ ] kaust-logo.png
- [ ] cairo-university-logo.png

## 🔄 Fallback if You Can't Find a Logo

If you cannot find an official logo for something:

1. **Use a text placeholder** temporarily:
   - Create a simple colored square with initials (e.g., "AR" for "Under Review")
   - Use Canva or PowerPoint to create simple logo placeholders

2. **Generic alternatives**:
   - Use a university seal/crest
   - Use conference icons from their website footer
   - Create text-based logos with conference acronyms

3. **Temporary solution**:
   Leave the img src pointing to the filename - broken images won't crash the site, you can add logos later

## 💡 Pro Tips

1. **Batch download**: Most conferences have media/press kits with multiple logo formats
2. **Consistent style**: Use all color logos or all monochrome for visual consistency
3. **Cache locally**: Keep a backup of all logos in case websites change
4. **Version control**: Keep original high-res versions separate from web-optimized versions
5. **Attribution**: If required by logo usage guidelines, add attribution in footer or about page

## ❓ Common Issues

**Q: Logo appears blurry**
A: Use 2x resolution (e.g., 100x100px for a 50x50px container)

**Q: Logo doesn't show up**
A: Check file path, check filename case, verify file exists

**Q: Logo is too large/small**
A: The containers auto-scale. Crop your logo to remove excess whitespace

**Q: Wrong logo displays**
A: Clear browser cache, verify correct filename in HTML

## 📧 Need Help?

If you need help finding specific logos or have questions about implementation, you can:
1. Check the official conference/company website
2. Search "[organization name] logo png transparent"
3. Check brand guidelines pages
4. Email the organization's media/PR department

Good luck with your logos! 🎨
