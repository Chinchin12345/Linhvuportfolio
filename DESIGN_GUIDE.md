# Linh Vu Portfolio - Design Guide

## 🎨 Color Palette

```css
Primary Color (Dark):     #2c2c2c
Secondary Color (Light):  #f5f5f5
Accent Color (Gold):      #d4af37
Text Dark:                #1a1a1a
Text Light:               #666666
White:                    #ffffff
```

## 📝 Typography

### Font Families
- **Headings**: Playfair Display (Serif)
- **Body**: Inter (Sans-serif)

### Font Sizes
```
Hero Title:        40-72px (responsive)
Section Title:     36-56px (responsive)
Project Title:     32-48px (responsive)
Body Text:         16-18px
Small Text:        12-14px
```

### Font Weights
- Light: 300
- Regular: 400
- Medium: 500
- Semi-bold: 600
- Bold: 700

## 📐 Spacing & Layout

### Container
- Max Width: 1400px
- Padding: 40px (desktop), 20px (mobile)

### Section Padding
- Desktop: 120px vertical
- Tablet: 80px vertical
- Mobile: 60px vertical

### Grid Gaps
- Large: 80px
- Medium: 50px
- Small: 30px
- XSmall: 20px

## 🎭 Components

### Navigation
- Height: ~70px
- Fixed position
- Background: rgba(255, 255, 255, 0.98)
- Box Shadow: 0 2px 20px rgba(0,0,0,0.05)

### Buttons
```css
Primary Button:
- Background: #2c2c2c
- Color: #ffffff
- Padding: 16px 40px
- Border: 2px solid #2c2c2c
- Hover: Background #d4af37

Secondary Button:
- Background: transparent
- Color: #2c2c2c
- Padding: 16px 40px
- Border: 2px solid #2c2c2c
- Hover: Background #2c2c2c, Color #ffffff
```

### Project Sections
- Image Height: 600px (desktop), 400px (tablet), 300px (mobile)
- Number Font Size: 80px
- Alternating left/right layout
- Even sections: #f5f5f5 background
- Odd sections: #ffffff background

### TOTO Gallery
- 3 columns x 2 rows (desktop)
- 2 columns (tablet)
- 1 column (mobile)
- Image Height: 400px
- Gap: 20px

### About Section Images
- 2 columns x 3 rows
- Image Height: 190px
- Gap: 15px

### Contact Section
- Max Width: 900px
- Centered layout
- Divider: 60px width, 2px height, gold color
- List items: border-bottom 1px #e0e0e0
- Hover: border-color #d4af37

## 🎬 Animations & Effects

### Transitions
- Duration: 0.3s
- Easing: ease-in-out

### Hover Effects
- Images: scale(1.05-1.1)
- Cards: translateY(-5px to -10px)
- Links: underline animation from left to right

### Scroll Animations
- Fade in: opacity 0 → 1
- Slide up: translateY(30-50px) → 0
- Stagger delay: 0.1s per item

## 📱 Breakpoints

```css
Desktop:   1024px and above
Tablet:    768px - 1023px
Mobile:    767px and below
Small:     480px and below
```

## 🖼️ Image Guidelines

### Image Formats
- PNG for screenshots and graphics
- JPG for photos
- WebP recommended for web optimization

### Image Sizes
- Hero images: 1920x1080px
- Project images: 1400x900px minimum
- Gallery images: 800x600px minimum
- Thumbnails: 400x300px

## 📦 Project Structure

```
Cursor Port/
├── index.html              # Main HTML file
├── styles.css              # All CSS styles
├── script.js               # JavaScript functionality
├── assets/
│   └── images/            # All project images
│       ├── TOTO 1-6.png
│       └── [other images]
├── README.md              # Project documentation
└── DESIGN_GUIDE.md        # This file
```

## 🎯 Design Principles

1. **Minimalism**: Clean, uncluttered layouts
2. **Typography-focused**: Strong hierarchy with serif + sans-serif combination
3. **Elegant**: Gold accent color used sparingly
4. **Professional**: High-end portfolio aesthetic
5. **Responsive**: Mobile-first approach
6. **Smooth**: Subtle animations and transitions

## 🔧 Figma Import Guide

### Method 1: Manual Recreation (Recommended)
1. Use this design guide for colors, fonts, spacing
2. Screenshot each section as reference
3. Recreate in Figma with components

### Method 2: HTML to Figma Plugin
1. Install "html.to.design" plugin in Figma
2. Paste your website URL or HTML code
3. The plugin will convert to Figma frames

### Method 3: Screenshot + Trace
1. Take full-page screenshots
2. Import to Figma as reference
3. Trace and build components on top

## 📋 Sections Checklist

- [x] Navigation Bar
- [x] Hero Section
- [x] Project 01: AEON Shopping Mall
- [x] Project 02: Yatabe Arena (Toy Factory)
- [x] Project 03: TOTO Premium Showroom (6 images gallery)
- [x] Project 04: Toyota Dealership
- [x] Project 05: The Minato Residence Showroom
- [x] Project 06: Luxury Residential Interiors
- [x] Project 07: Hotel Suite Collection
- [x] Project 08: MEDRING Pediatric Dental
- [x] About Section (with TOTO images grid)
- [x] Contact Section
- [x] Footer

## 💡 Tips for Figma

1. **Auto Layout**: Use for responsive components
2. **Components**: Create reusable button, card components
3. **Variants**: For hover states and responsive versions
4. **Styles**: Set up color and text styles first
5. **Grids**: Use 12-column grid with 1400px container
6. **Constraints**: Set up for responsive behavior

---

Created by Linh Vu | 2026
