# Images Directory

This directory contains all visual assets for the Asset Pricing Theory course.

## Directory Structure

```
images/
├── README.md                 # This file
├── logo/                     # Course and institutional logos
│   ├── dauphine-logo.png    # Paris Dauphine University logo
│   ├── course-logo.png      # Course-specific branding
│   └── favicon.ico          # Website favicon
├── diagrams/                 # Conceptual diagrams and charts
│   ├── asset-pricing-tree.svg
│   ├── capm-diagram.png
│   ├── sdf-illustration.svg
│   └── [topic-specific diagrams]
├── plots/                    # Example plots and visualizations
│   ├── efficient-frontier.png
│   ├── term-structure.png
│   └── [mathematical plots]
└── backgrounds/              # Slide backgrounds and templates
    ├── title-slide-bg.png
    └── section-bg.png
```

## Asset Guidelines

### Logos
- **Format**: PNG with transparent background preferred
- **Resolution**: Minimum 300 DPI for print, web-optimized versions available
- **Usage**: Follow institutional branding guidelines

### Diagrams
- **Format**: SVG preferred for scalability, PNG for complex illustrations
- **Style**: Consistent with course color scheme (#2596be primary)
- **Labels**: Use Merriweather font to match course materials

### Plots
- **Format**: PNG or SVG
- **Resolution**: High enough for projection (minimum 1920x1080)
- **Style**: Consistent matplotlib/seaborn styling

### Color Palette

Primary colors for the course:
- **Primary Blue**: #2596be
- **Secondary Blue**: #1f7a9a
- **Background**: #ffffff (white)
- **Text**: #000000 (black)
- **Accent Colors**: 
  - Info: #e3f2fd
  - Warning: #fff3cd
  - Success: #d4edda
  - Danger: #f8d7da

## File Naming Conventions

- Use lowercase with hyphens: `file-name.ext`
- Include day number for day-specific assets: `day01-capm-diagram.png`
- Use descriptive names: `efficient-frontier-example.png` not `plot1.png`
- Version control: `diagram-v2.svg` for updated versions

## Usage in Course Materials

### In Quarto Slides
```markdown
![Caption](../../images/diagrams/asset-pricing-tree.svg){width=80%}
```

### In HTML
```html
<img src="images/logo/course-logo.png" alt="Course Logo" class="course-logo">
```

### In CSS
```css
.slide-logo {
    background-image: url('../images/logo/dauphine-logo.png');
}
```

## Asset Creation Guidelines

### Mathematical Diagrams
- Use consistent mathematical notation
- Ensure readability at various sizes
- Include proper labels and legends
- Use course color scheme

### Economic Illustrations
- Focus on conceptual clarity
- Avoid unnecessary complexity
- Use standard economic notation
- Include clear axis labels and units

### Data Visualizations
- Follow best practices for data visualization
- Use appropriate chart types
- Include proper titles and legends
- Ensure accessibility (color blind friendly)

## Placeholder Files

The following placeholder files should be created:

1. **course-logo.png** - Main course branding
2. **dauphine-logo.png** - University logo
3. **asset-pricing-overview.svg** - Course overview diagram
4. **sdf-framework.svg** - Stochastic discount factor illustration
5. **portfolio-theory.png** - Portfolio optimization visualization
6. **term-structure-models.png** - Interest rate models comparison

## Copyright and Licensing

- All original course materials: MIT License (see main LICENSE file)
- Third-party images: Ensure proper licensing and attribution
- Institutional logos: Used with permission, follow branding guidelines
- Stock images: Use only royalty-free or properly licensed content

## Tools and Software

Recommended tools for creating course assets:
- **Vector Graphics**: Inkscape (free), Adobe Illustrator
- **Raster Graphics**: GIMP (free), Adobe Photoshop
- **Mathematical Diagrams**: TikZ/LaTeX, Python (matplotlib), R (ggplot2)
- **Charts and Plots**: Python (plotly, seaborn), R (ggplot2)

## Accessibility

Ensure all images include:
- **Alt text** for screen readers
- **High contrast** for visibility
- **Scalable formats** when possible
- **Color blind friendly** palettes

---

*This directory supports the visual elements of the Asset Pricing Theory Ph.D. course.*
