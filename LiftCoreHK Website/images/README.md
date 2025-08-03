# Image Organization Guide

This folder is organized to help you manage your LiftCore website images efficiently.

## 📁 Folder Structure

```
images/
├── hero/           # Hero section images
├── products/       # Product images (elevators)
├── services/       # Service-related images
├── company/        # Company/team images
└── README.md       # This guide
```

## 🎯 Recommended Image Types

### Hero Images (`hero/`)
- **hero-bg.jpg** - Background image for hero section
- **elevator-hero.jpg** - Main elevator showcase image
- **office-building.jpg** - Commercial building with elevators

### Product Images (`products/`)
- **smart-elevator-1.jpg** - Smart elevator interior
- **smart-elevator-2.jpg** - Smart elevator exterior
- **home-elevator-1.jpg** - Home elevator installation
- **home-elevator-2.jpg** - Home elevator interior
- **elevator-controls.jpg** - Control panel/system
- **elevator-shaft.jpg** - Technical elevator components

### Service Images (`services/`)
- **consultation.jpg** - Professional consultation meeting
- **installation.jpg** - Elevator installation process
- **maintenance.jpg** - Maintenance and repair work
- **modernization.jpg** - Elevator modernization project
- **engineering.jpg** - Engineering and planning

### Company Images (`company/`)
- **team-photo.jpg** - Company team photo
- **office.jpg** - Office/location photos
- **certificates.jpg** - Company certificates and awards
- **partners.jpg** - Partner company logos
- **jimmy-lau.jpg** - Jimmy Lau's professional photo

## 📏 Image Specifications

### Recommended Sizes:
- **Hero images**: 1920x1080px (16:9 ratio)
- **Product images**: 800x600px (4:3 ratio)
- **Service images**: 600x400px (3:2 ratio)
- **Company images**: 400x400px (1:1 ratio for team photos)

### File Formats:
- **JPG/JPEG**: For photographs and complex images
- **PNG**: For images with transparency
- **WebP**: For better compression (modern browsers)
- **SVG**: For logos and simple graphics

## 🚀 How to Use Images in the Website

### 1. Replace Hero Background
```html
<!-- In index.html, find the hero section -->
<section class="hero" style="background-image: url('images/hero/hero-bg.jpg');">
```

### 2. Add Product Images
```html
<!-- In the products section -->
<div class="product-card">
    <img src="images/products/smart-elevator-1.jpg" alt="Smart Elevator">
    <!-- rest of content -->
</div>
```

### 3. Add Service Images
```html
<!-- In the services section -->
<div class="service-card">
    <img src="images/services/consultation.jpg" alt="Professional Consultation">
    <!-- rest of content -->
</div>
```

### 4. Add Company Images
```html
<!-- In the about section -->
<div class="company-image">
    <img src="images/company/team-photo.jpg" alt="LiftCore Team">
</div>
```

## 📝 Image Naming Convention

Use descriptive, lowercase names with hyphens:
- ✅ `smart-elevator-interior.jpg`
- ✅ `jimmy-lau-portrait.jpg`
- ✅ `office-building-exterior.jpg`
- ❌ `IMG_001.jpg`
- ❌ `elevator photo.png`

## 🎨 Image Optimization Tips

1. **Compress images** before uploading (use tools like TinyPNG)
2. **Use appropriate formats** (JPG for photos, PNG for graphics)
3. **Keep file sizes under 500KB** for web performance
4. **Use descriptive alt text** for accessibility
5. **Consider responsive images** for different screen sizes

## 🔧 Quick Integration

Once you upload images, you can quickly integrate them by:

1. **Hero background**: Replace the CSS gradient with your image
2. **Product cards**: Add images above the product descriptions
3. **Service cards**: Add images alongside the icons
4. **About section**: Add team/company photos
5. **Contact section**: Add Jimmy Lau's photo

## 📱 Responsive Images

For better mobile experience, consider providing multiple sizes:
- `image-large.jpg` (1200px+)
- `image-medium.jpg` (768px+)
- `image-small.jpg` (320px+)

## 🎯 Next Steps

1. **Upload your images** to the appropriate folders
2. **Update the HTML** to reference your images
3. **Test the website** to ensure images load correctly
4. **Optimize images** if needed for better performance

---

**Note**: All images should be high-quality and professionally represent LiftCore's brand and services. 