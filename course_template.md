# Course Template: Creating a Quarto-Based Academic Course Website

This template provides a complete guide to setting up a new academic course using Quarto, based on the Asset Pricing Theory course structure. Use this as your starting point for creating a new course project.

## Project Overview

This template creates a modern, interactive course website with:
- **Quarto-powered rendering** for slides and documentation
- **Reveal.js slides** for engaging presentations
- **Responsive HTML website** with navigation
- **Mathematical notation** support via LaTeX/KaTeX
- **Code execution** and interactive elements
- **Professional styling** and branding

## Quick Start Setup

### 1. Create New Repository
```bash
# Create a new directory for your course
mkdir your-course-name
cd your-course-name

# Initialize git repository
git init
```

### 2. Install Dependencies
```bash
# Install Quarto (if not already installed)
# Download from: https://quarto.org/docs/get-started/

# Verify installation
quarto --version
```

### 3. Initialize Project Structure
Create the following directory structure:

```
your-course-name/
├── _quarto.yml              # Project configuration
├── index.qmd               # Main course landing page
├── README.md               # Project documentation
├── LICENSE                 # License file
└── src/                    # All source materials
    ├── assets/
    │   ├── styles.css      # Custom CSS styling
    │   └── images/         # Course images and logos
    ├── templates/
    │   └── DAY_TEMPLATE.md # Template for new lectures
    └── lectures/           # Course content by day
        ├── day0/
        │   └── lecture/
        │       └── index.qmd
        └── [additional days...]
```

## Configuration Files

### _quarto.yml (Project Configuration)
```yaml
project:
  type: website
  title: "Your Course Title"
  output-dir: "_site"

website:
  title: "Your Course Title"
  description: "Course description"
  site-url: "https://yourusername.github.io/your-course-repo"
  repo-url: "https://github.com/yourusername/your-course-repo"

  navbar:
    title: "Your Course Title"
    left:
      - text: "Home"
        href: index.html
      - text: "Course Days"
        menu:
          - text: "Day 0: Introduction"
            href: src/lectures/day0/lecture/index.qmd
          # Add more days as needed
    right:
      - icon: github
        href: "https://github.com/yourusername/your-course-repo"

format:
  html:
    theme:
      - cosmo
      - src/assets/styles.css
    toc: true
    toc-depth: 3
    number-sections: true
    number-depth: 3
    code-fold: false
    code-tools: true
    citations-hover: true
    footnotes-hover: true

  revealjs:
    theme: white
    css: src/assets/styles.css
    slide-number: true
    chalkboard: true
    preview-links: auto
    transition: slide
    background-transition: fade
    hash-type: number
    controls: true
    progress: true
    center: false

execute:
  freeze: auto
  cache: true

editor: visual
```

### index.qmd (Main Landing Page)
```yaml
---
title: "Your Course Title"
subtitle: "Course Subtitle"
author: "Your Name"
institute: "Your Institution"
format:
  html:
    css: src/assets/styles.css
    toc: false
---

## Welcome to [Course Title]

[Course description and overview]

## Course Information

- **Instructor**: Your Name
- **Email**: your.email@institution.edu
- **Institution**: Your Institution
- **Duration**: [Duration]
- **Prerequisites**: [Prerequisites]

## Learning Objectives

[Course learning objectives]

## Course Schedule

[Course schedule and topics]

## Getting Started

1. Start with [Day 0](src/lectures/day0/lecture/index.qmd)
2. Follow the course progression

## Resources

- [Course Repository](https://github.com/yourusername/your-course-repo)
- [Additional Resources]
```

### README.md (Project Documentation)
```markdown
# Your Course Title

[Course description]

## Course Information

- **Instructor**: Your Name
- **Institution**: Your Institution
- **Prerequisites**: [Prerequisites]

## Project Structure

- `src/` - All source files for course content
  - `lectures/` - Daily lecture materials
  - `assets/` - Styles and images
- `_quarto.yml` - Quarto project configuration
- `index.qmd` - Main course index page

## How to Use This Repository

### Rendering Content

```bash
# Render the entire project
quarto render

# Render specific files
quarto render src/lectures/day1/lecture/index.qmd --to revealjs
quarto render src/lectures/day1/lecture/index.qmd --to html
```

## Technical Requirements

- [Quarto](https://quarto.org/) for rendering
- LaTeX for mathematical notation (included with Quarto)

## Setup Instructions

1. Install Quarto
2. Clone this repository
3. Render content: `quarto render`
```

## Lecture Structure Template

### Daily Lecture Structure
Each day should follow this structure:

```
src/lectures/dayX/
└── lecture/
    ├── index.qmd          # Main lecture overview
    ├── 01-topic1.qmd      # Individual topics
    ├── 02-topic2.qmd
    └── [additional topics]
```

### Lecture index.qmd Template
```yaml
---
title: "Day X: Topic Title"
subtitle: "Your Course Title"
author: "Your Name"
institute: "Your Institution"
date: "`r Sys.Date()`"
format:
  revealjs:
    theme: white
    css: ../../../assets/styles.css
    slide-number: true
    chalkboard: true
    preview-links: auto
    logo: ../../../assets/images/logo.png
    footer: "Your Course Title - Day X"
---

## Course Overview {.center}

::: {.financial-concept}
**Day X: Topic Title**

[Brief description of the day's content]
:::

## Learning Objectives

By the end of this session, you will be able to:

- [Learning objective 1]
- [Learning objective 2]
- [Learning objective 3]

## Outline

1. [Topic 1](01-topic1.html)
2. [Topic 2](02-topic2.html)
3. [Topic 3](03-topic3.html)

---

[Additional content sections...]
```

### Topic-Specific Template
```yaml
---
title: "Topic: Specific Topic"
subtitle: "Day X - Your Course Title"
author: "Your Name"
format:
  revealjs:
    theme: white
    css: ../../../assets/styles.css
    slide-number: true
---

## Topic Title {.center}

::: {.key-concept}
**Key Concept**: Brief description
:::

## Mathematical Framework

[Mathematical content with LaTeX]

$$
[Key equation]
$$

## Economic Intuition

::: {.two-columns}
::: {.column}
**Intuitive Explanation**
- Point 1
- Point 2
:::

::: {.column}
**Mathematical Result**
- Mathematical insight 1
- Mathematical insight 2
:::
:::

## Theoretical Examples

::: {.financial-concept}
**Example**: Example description

[Example content with mathematical derivations]
:::
```

## Custom Styling

### src/assets/styles.css
```css
/* Custom styles for your course */
.financial-concept {
  background-color: #f8f9fa;
  border-left: 4px solid #007bff;
  padding: 1rem;
  margin: 1rem 0;
}

.key-concept {
  background-color: #e9ecef;
  border: 2px solid #6c757d;
  padding: 1rem;
  margin: 1rem 0;
  font-weight: bold;
}

.two-columns {
  display: flex;
  gap: 2rem;
}

.column {
  flex: 1;
}

/* Additional styling as needed */
```

## Deployment and Publishing

### GitHub Pages Deployment
1. Push your repository to GitHub
2. Go to repository Settings > Pages
3. Set source to "Deploy from a branch"
4. Select "gh-pages" branch (or main with /docs folder)
5. Enable GitHub Actions for automated deployment

### Automated Rendering
Create `.github/workflows/deploy.yml`:

```yaml
name: Deploy Quarto site

on:
  push:
    branches: main

jobs:
  build-deploy:
    runs-on: ubuntu-latest
    steps:
      - name: Check out repository
        uses: actions/checkout@v4

      - name: Set up Quarto
        uses: quarto-dev/quarto-actions/setup@v2

      - name: Render and Publish
        uses: quarto-dev/quarto-actions/publish@v2
        with:
          target: gh-pages
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

## Best Practices

### Content Organization
- Keep mathematical notation consistent
- Use clear, hierarchical structure
- Include learning objectives for each section
- Provide both intuition and rigor

### Technical Best Practices
- Test all links and navigation
- Ensure mathematical rendering works
- Optimize images and assets
- Use semantic HTML and accessible design

### Maintenance
- Regularly update dependencies
- Test rendering on different devices
- Keep documentation current
- Backup important materials

## Customization Checklist

- [ ] Update course title and description
- [ ] Replace instructor information
- [ ] Customize color scheme and branding
- [ ] Add course-specific images and logos
- [ ] Modify learning objectives
- [ ] Update prerequisites
- [ ] Configure repository URLs
- [ ] Set up deployment workflow

## Getting Help

- [Quarto Documentation](https://quarto.org/)
- [Reveal.js Documentation](https://revealjs.com/)
- [GitHub Pages Guide](https://pages.github.com/)

---

*This template is based on the Asset Pricing Theory course structure. Customize it for your specific course needs.*
