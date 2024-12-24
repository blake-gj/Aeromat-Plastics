# Aeromat Documentation Theme

A professional Jekyll documentation theme for Aeromat.io, featuring Material Design 3 dark theme principles and optimized for technical documentation.

## Features

- Material Design 3 dark theme implementation
- Responsive layout with mobile support
- Search functionality
- Syntax highlighting
- Documentation-specific components
- SEO optimization

## Prerequisites

- Ruby (version 2.7.0 or higher)
- Bundler
- Jekyll

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/aeromat-docs.git
   cd aeromat-docs
   ```

2. Install dependencies:
   ```bash
   bundle install
   ```

3. Start the development server:
   ```bash
   bundle exec jekyll serve
   ```

4. Visit `http://localhost:4000` in your browser

## Directory Structure

```
aeromat-docs/
├── _docs/           # Documentation pages
├── _layouts/        # Layout templates
├── _sass/          # Theme styles
├── assets/         # CSS, JavaScript, images
├── _config.yml     # Site configuration
└── Gemfile         # Ruby dependencies
```

## Creating Documentation

1. Add new documentation pages in the `_docs` directory
2. Use Markdown format with YAML front matter
3. Follow the existing structure for consistency

Example:
```markdown
---
title: Your Page Title
nav_order: 3
---

# Your Page Title
Content goes here...
```

## Customization

### Colors

Edit the color variables in `_sass/aeromat-theme.scss`:

```scss
$color-primary: #4F78FF;
$color-surface: #121212;
// ... other colors
```

### Typography

Modify font settings in `_config.yml`:

```yaml
theme_settings:
  fonts:
    body: "Inter, system-ui, -apple-system, sans-serif"
    code: "JetBrains Mono, monospace"
```

### Navigation

Update the navigation structure in `_config.yml`:

```yaml
nav_sections:
  - title: Section Title
    items:
      - page-slug
```

## Components

### Callouts

Use callouts for important information:

```markdown
{: .callout.info}
> Information message

{: .callout.warning}
> Warning message

{: .callout.error}
> Error message
```

### Code Blocks

Use syntax highlighting for code:

```markdown
```python
def example():
    return "Hello, World!"
```
```

### Tables

Create formatted tables:

```markdown
| Header 1 | Header 2 |
|----------|----------|
| Cell 1   | Cell 2   |
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This theme is available as open source under the terms of the [MIT License](LICENSE). 