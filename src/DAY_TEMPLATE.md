# Day Template for Asset Pricing Theory Course

This template can be copied to create new day structures for the Asset Pricing Theory course.

## Day Structure

Each day should follow this standardized structure:

```
dayX/
└── lecture/
    ├── index.qmd                 # Main lecture file
    ├── index.html                # Rendered HTML version
    ├── index_files/              # Quarto-generated assets
    ├── 01-topic1.qmd             # Individual topic files
    ├── 01-topic1.html            # Rendered versions
    ├── 02-topic2.qmd
    ├── 02-topic2.html
    ├── 03-topic3.qmd
    ├── 03-topic3.html
    └── [additional topics...]
```

## File Templates

### Lecture index.qmd Template

```yaml
---
title: "Day X: [Topic Title]"
subtitle: "Asset Pricing Theory"
author: "Juan F. Imbet"
institute: "Paris Dauphine University-PSL"
date: "`r Sys.Date()`"
format:
  revealjs:
    theme: white
    css: ../../src/styles.css
    slide-number: true
    chalkboard: true
    preview-links: auto
    logo: ../../images/logo.png
    footer: "Asset Pricing Theory - Day X"
---

## Course Overview {.center}

::: {.financial-concept}
**Day X: [Topic Title]**

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

### Topic-specific .qmd Template

```yaml
---
title: "Topic: [Specific Topic]"
subtitle: "Day X - Asset Pricing Theory"
author: "Juan F. Imbet"
format:
  revealjs:
    theme: white
    css: ../../src/styles.css
    slide-number: true
---

## [Topic Title] {.center}

::: {.key-concept}
**Key Concept**: [Brief description]
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
- [Point 1]
- [Point 2]
:::

::: {.column}
**Mathematical Result**
- [Mathematical insight 1]
- [Mathematical insight 2]
:::
:::

## Theoretical Examples

::: {.financial-concept}
**Example**: [Example description]

[Example content with mathematical derivations]
:::
```

## Usage Instructions

1. Copy this template to create `dayX/` structure
2. Replace `X` with the appropriate day number
3. Replace `[Topic Title]` with the specific day topic
4. Fill in the specific content for each file
5. Test all links and navigation
6. Render Quarto files to HTML

## Quality Checklist

- [ ] All mathematical notation renders correctly
- [ ] Links between files work properly
- [ ] CSS styling applies consistently
- [ ] Navigation elements function correctly
- [ ] Learning objectives are measurable
- [ ] Theoretical content is rigorous and clear

---

*This template ensures consistency across all days of the Asset Pricing Theory course.*
