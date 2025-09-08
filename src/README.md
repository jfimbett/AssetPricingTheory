# Source Directory (src/)

This directory contains all the source materials for the Asset Pricing Theory course.

## Directory Structure

```
src/
├── assets/                    # Static assets and styling
│   ├── styles.css            # Main CSS stylesheet for all course materials
│   └── images/               # Course images, logos, and visual assets
├── templates/                 # Templates for creating new content
│   └── DAY_TEMPLATE.md       # Template for creating new lecture days
└── lectures/                  # All course lectures organized by day
    ├── day0/                 # Course introduction
    ├── day1/                 # Fundamentals of Asset Pricing
    ├── day2/                 # Portfolio Choice and Static Models
    ├── day3/                 # Dynamic Asset Pricing
    ├── day4/                 # Fixed-Income and Derivatives
    ├── day5/                 # Market Frictions
    ├── day6/                 # Information and Microstructure
    ├── day7/                 # Intertemporal Risk
    ├── day8/                 # Macro-Finance
    └── day9/                 # Behavioral and Household Finance
```

## File Organization Principles

### Assets (`assets/`)
- **styles.css**: Centralized CSS for consistent styling across all materials
- **images/**: All visual assets including logos, diagrams, and illustrations
- Maintains consistent branding and visual identity

### Templates (`templates/`)
- **DAY_TEMPLATE.md**: Standard template for creating new lecture days
- Ensures consistency in structure and formatting
- Contains sample content and best practices

### Lectures (`lectures/`)
- Main course content organized by day
- Each day follows the template structure
- Theoretical materials in Quarto markdown format

## Navigation and Links

All internal links are relative to the repository root:
- From lecture files: Use `../../../` to reach root level
- Consistent path structure for easy maintenance

## Content Development Workflow

1. **Create new day**: Copy template from `templates/DAY_TEMPLATE.md`
2. **Place in lectures/**: Create `dayX/lecture/` structure
3. **Update paths**: Ensure CSS and navigation links are correct
4. **Add content**: Develop theoretical materials following template
5. **Test rendering**: Use `quarto render` to verify output

## Styling Guidelines

- Use the centralized `assets/styles.css` for all styling
- Maintain consistent mathematical notation
- Follow the established color scheme (#2596be primary blue)
- Ensure responsive design for different screen sizes

---

*This organization ensures maintainability, consistency, and professional presentation of the Asset Pricing Theory course materials.*
