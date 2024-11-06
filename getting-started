# Getting Started with Koda SSG

Welcome to Koda SSG! This guide will help you create your first static site with Koda SSG.

## Prerequisites

Before starting, ensure you have:
- Python 3.8 or newer installed
- pip (Python package manager)
- Basic knowledge of Markdown

## Installation

### 1. Set Up Python Environment

```bash
# Create a new directory for your site
mkdir my-site
cd my-site

# Create a virtual environment
python -m venv venv

# Activate virtual environment
# On Linux/Mac:
source venv/bin/activate
# On Windows:
.\venv\Scripts\activate
```

### 2. Install Koda SSG

```bash
pip install koda-ssg
```

## Creating Your First Site

### 1. Initialize a New Site

```bash
# Create a new Koda site
koda init my-first-site
cd my-first-site
```

This creates a basic site structure:
```
my-first-site/
├── content/
│   ├── posts/
│   └── pages/
├── static/
│   ├── css/
│   └── images/
└── config.yml
```

### 2. Configure Your Site

Edit `config.yml`:

```yaml
site_name: My Awesome Site
theme: minimal
author: Your Name
base_url: https://example.com
pagination:
  items_per_page: 10
comments:
  enabled: false
```

### 3. Add Content

Create your first post in `content/posts/hello.md`:

```markdown
---
title: Hello, World!
date: 2024-03-15
categories: blog
tags: first, hello
---

# Welcome to My Site

This is my first post using Koda SSG!
```

### 4. Build Your Site

```bash
# Build the site
koda build

# Start development server
koda serve
```

Visit `http://localhost:8000` to see your site!

## Adding a Photo Gallery

### 1. Create Gallery Structure

```bash
# Create gallery directory
mkdir -p content/galleries/vacation
```

### 2. Add Images and Captions

Add your images to the gallery directory, then create `content/galleries/vacation/captions.yml`:

```yaml
beach.jpg: "Beautiful day at the beach"
sunset.jpg: "Stunning sunset over the mountains"
```

### 3. Create Gallery Page

Create `content/posts/vacation.md`:

```markdown
---
title: Summer Vacation
date: 2024-03-15
gallery: galleries/vacation
---

Check out the photos from our summer vacation!
```

## Customizing Your Site

### 1. Choose a Theme

Available themes:
- minimal (default)
- developer
- writer
- photo
- docs
- magazine

Change themes using:

```bash
koda build --theme photo
```

### 2. Configure Theme Settings

Each theme has customizable options in `config.yml`:

```yaml
theme: photo
theme_settings:
  color_scheme: dark
  sidebar: right
  show_author: true
```

## Common Tasks

### Adding a New Post

```markdown
---
title: My New Post
date: 2024-03-15
categories: blog
tags: example, guide
---

Your post content here.
```

### Creating Pages

Add pages in `content/pages/`:

```markdown
---
title: About Me
menu: main
order: 1
---

Information about yourself.
```

### Managing Assets

Place static files in `static/`:
- CSS in `static/css/`
- Images in `static/images/`
- JavaScript in `static/js/`

## Next Steps

1. **Explore Features**:
   - Add categories and tags
   - Configure comments
   - Set up RSS feed
   - Enable search

2. **Customize Design**:
   - Modify theme templates
   - Add custom CSS
   - Create new layouts

3. **Deploy Your Site**:
   - Build for production
   - Deploy to hosting service

## Troubleshooting

### Build Errors

```bash
# Clean build directory
koda clean

# Rebuild with verbose output
koda build --verbose
```

### Development Server Issues

```bash
# Check port availability
koda serve --port 8080

# Enable debug mode
koda serve --debug
```

## Getting Help

- Check our [Documentation](docs/)
- Open an [Issue](issues/)
- Join our [Discussions](discussions/)

## Command Reference

```bash
# Create new site
koda init SITE_NAME

# Build site
koda build [--theme THEME]

# Start development server
koda serve [--port PORT]

# Clean build directory
koda clean

# Generate new post
koda new post "Post Title"

# Create new gallery
koda new gallery "Gallery Name"
```

Remember to:
1. Always work in a virtual environment
2. Keep your content organized
3. Commit changes regularly
4. Back up your content

Happy publishing with Koda SSG! 🎉
