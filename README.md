# Koda SSG 🚀

A modern, flexible static site generator built with Python. Koda SSG makes it easy to create beautiful static websites with powerful features like photo galleries, code highlighting, and more.

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Python Version](https://img.shields.io/badge/python-3.8+-blue.svg)
![Made with Love](https://img.shields.io/badge/Made%20with-❤️-red.svg)

## ✨ Features

- 📝 **Markdown Support**: Write content in Markdown with YAML frontmatter
- 🎨 **Multiple Themes**: 6 responsive, modern themes included
- 🖼️ **Photo Galleries**: Built-in gallery support with captions and layouts
- 💬 **Comments**: GitHub Discussions integration via Giscus
- 🔍 **Search**: Built-in search functionality
- 📡 **RSS Feed**: Automatic feed generation
- 📑 **Pagination**: Smart pagination for blogs and galleries
- 🏷️ **Taxonomy**: Categories and tags support
- ✨ **Syntax Highlighting**: Beautiful code highlighting with Pygments

## 🚀 Quick Start

### Installation

```bash
# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # Linux/Mac
# or
.\venv\Scripts\activate  # Windows

# Install Koda SSG
pip install koda-ssg
```

### Create Your First Site

```bash
# Create new site
koda new my-site
cd my-site

# Add content in content/posts/hello.md
---
title: Hello World
date: 2024-03-15
categories: blog
tags: first, hello
---

Hello, World!

# Build site
koda build

# Start development server
koda serve
```

Visit `http://localhost:8000` to see your site!

## 📸 Gallery Support

Create beautiful photo galleries with ease:

1. Create gallery directory:
```bash
mkdir -p content/galleries/vacation
```

2. Add images and captions:
```yaml
# content/galleries/vacation/captions.yml
sunset.jpg: "Beautiful sunset over the mountains"
beach.jpg: "Perfect day at the beach"
```

3. Reference in your markdown:
```markdown
---
title: Vacation Photos
gallery: galleries/vacation
---

Check out our amazing vacation photos!
```

## 🎨 Themes

Koda comes with 6 beautiful themes:

- Minimal: Clean and simple
- Developer: Perfect for technical blogs
- Writer: Focus on typography
- Photo: Optimized for photography
- Docs: Documentation-focused
- Magazine: Rich media layout

Change themes with:
```bash
koda build --theme photo
```

## ⚙️ Configuration

Create `config.yml` in your site root:

```yaml
site_name: My Awesome Site
theme: minimal
author: Your Name
base_url: https://example.com
pagination:
  items_per_page: 10
comments:
  enabled: true
  giscus_repo: username/repo
  giscus_repo_id: your-repo-id
gallery:
  thumbnail_size: [300, 300]
  large_size: [1200, 1200]
```

## 📖 Documentation

For detailed documentation, check out:
- [Getting Started Guide](docs/getting-started.md)
- [Configuration Guide](docs/configuration.md)
- [Theme Development](docs/themes.md)
- [Gallery Guide](docs/galleries.md)
- [API Reference](docs/api.md)

## 🤝 Contributing

Contributions are welcome! Please read our [Contributing Guide](CONTRIBUTING.md) for details on:

- Code style
- Development setup
- Submitting pull requests
- Bug reporting
- Feature requests

## 🔧 Development

Set up development environment:

```bash
# Clone repository
git clone https://github.com/stephenfinnegan/koda-ssg.git
cd koda-ssg

# Create virtual environment
python -m venv venv
source venv/bin/activate

# Install dependencies
pip install -e ".[dev]"

# Run tests
pytest
```

## 🧪 Testing

Run the test suite:

```bash
# Run all tests
pytest

# Run with coverage
pytest --cov=koda_ssg

# Run specific test file
pytest tests/test_gallery.py
```

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👥 Community

- [GitHub Discussions](https://github.com/stephenfinnegan/koda-ssg/discussions)
- [Issue Tracker](https://github.com/stephenfinnegan/koda-ssg/issues)

## 💖 Support

If you find Koda SSG helpful, please:
- Star the repository
- Report issues
- Submit pull requests
- Share with others

## 🙏 Acknowledgments

Special thanks to:
- All our contributors
- The Python community
- Open source projects that inspired us

---

Built with ❤️ by [Stephen Finnegan](https://github.com/stephenfinnegan)
