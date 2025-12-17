# Experience Page Logos - Setup Guide

## 📍 Where Are The Logos?

The logos are **already coded into your experience.html file**. They're in the HTML but you need to add the actual image files.

## 🔍 Finding Them in the Code

Look for this code in your `experience.html` (appears 4 times, once per job):

```html
<div class="timeline-content">
    <div class="company-logo">
        <img src="logos/adobe-logo.png" alt="Adobe" class="company-logo-img">
    </div>
    <div class="company-header">
        <div>
            <h3 class="company-name">Adobe</h3>
            ...
```

**This code is at these locations:**
1. **Line ~140** - Adobe logo
2. **Line ~175** - Valeo logo  
3. **Line ~210** - Cairo University logo
4. **Line ~245** - TechiBees logo

## 🎨 Visual Position

The logos appear in the **top-right corner** of each experience card, like this:

```
┌─────────────────────────────────────────────────┐
│                                    [LOGO] ◄─── Here!
│  Company Name                                   │
│  Role Title                                     │
│                                                 │
│  Description and achievements...                │
│                                                 │
└─────────────────────────────────────────────────┘
```

## ✅ What You Need To Do

### Step 1: Create logos folder
In the same directory as your HTML files, create:
```
logos/
```

### Step 2: Add these 4 image files
Download/create and save these files:

1. **logos/adobe-logo.png**
   - Adobe's logo (red "A" symbol)
   - Download from: https://www.adobe.com/about-adobe/press-resources.html

2. **logos/valeo-logo.png**
   - Valeo's logo (blue oval with "Valeo")
   - Download from: https://www.valeo.com/en/media/

3. **logos/cairo-university-logo.png**
   - Cairo University seal/logo
   - Search: "Cairo University logo PNG"

4. **logos/techibees-logo.png**
   - TechiBees company logo
   - You may need to create this or use a generic tech startup icon

### Step 3: Image Requirements
- **Format**: PNG (transparent background preferred)
- **Size**: 200x200px or larger (will auto-scale to 50x50px)
- **Square ratio**: Best results with equal width/height

### Step 4: File Structure
Your final structure should look like:

```
your-website/
├── index.html
├── experience.html
├── education.html
├── publications.html
├── styles.css
├── script.js
└── logos/
    ├── adobe-logo.png          ✓
    ├── valeo-logo.png           ✓
    ├── cairo-university-logo.png ✓
    └── techibees-logo.png       ✓
```

## 🧪 Testing

1. Open `experience.html` in your browser
2. You should see 4 logos in the top-right corner of each card
3. If you see a broken image icon (🖼️❌), the file path is wrong

## 🔧 Troubleshooting

**Logo doesn't appear:**
- Check filename exactly matches (case-sensitive!)
- Verify file is in `logos/` folder
- Make sure path is relative (no `/` at start)

**Logo appears but looks bad:**
- Logo too small? Use higher resolution source
- Logo stretched? Crop to square before adding
- Logo has white background? Use PNG with transparency

**Logo overlaps with text:**
- This is already fixed! There's 60px padding-right on company-header

## 💡 Quick Test

Want to test before adding real logos? Create a simple colored square:

1. Open any image editor (even MS Paint)
2. Create 200x200px image
3. Fill with a solid color
4. Save as `adobe-logo.png`
5. Place in `logos/` folder
6. Refresh page - you should see the colored square!

## 📏 Current Styling

The logos are styled to:
- Position: Absolute top-right
- Size: 50x50px container
- Background: White
- Border: Light gray
- Shadow: Subtle
- Padding: 0.5rem (keeps logo from touching edges)
- Border-radius: 8px (rounded corners)

This makes them look professional and consistent across all cards!

## ✅ You're Done When...

- [ ] `logos/` folder exists
- [ ] 4 logo files are in the folder
- [ ] Filenames exactly match (adobe-logo.png, valeo-logo.png, etc.)
- [ ] Open experience.html and see all 4 logos
- [ ] Logos look good and don't overlap with text

---

**The code is already there! You just need to add the image files.** 🎨
