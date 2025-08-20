# Hugo Portfolio Website

A modern, responsive portfolio website built with Hugo and the Blowfish theme.

## Features

- 🎨 Modern, responsive design
- 🌙 Dark/Light mode toggle
- 📱 Mobile-friendly
- 🚀 Fast loading with Hugo
- 📝 Blog support
- 💼 Project showcase
- 📧 Contact page
- 🔍 Search functionality

## Quick Start

### Prerequisites

- [Hugo Extended](https://gohugo.io/installation/) (v0.112.0 or later)
- [Git](https://git-scm.com/)

### Local Development

1. Clone this repository:

   ```bash
   git clone https://github.com/yourusername/portfolio.git
   cd portfolio
   ```

2. Install the theme:

   ```bash
   git submodule update --init --recursive
   ```

3. Start the development server:

   ```bash
   hugo server -D
   ```

4. Open your browser to `http://localhost:1313`

### Customization

1. **Personal Information**: Update `config/_default/languages.en.toml` with your details
2. **Profile Image**: Add your photo as `static/img/avatar.jpg`
3. **Social Links**: Update the links in the languages config
4. **Content**: Add your projects, blog posts, and update the about page
5. **Colors**: Modify the color scheme in `config/_default/params.toml`

### Adding Content

#### Blog Posts

```bash
hugo new posts/my-new-post.md
```

#### Projects

```bash
hugo new projects/my-project.md
```

### Deployment

This site is configured for GitHub Pages deployment. To deploy:

1. Push to your main branch
2. Enable GitHub Pages in repository settings
3. Set source to "GitHub Actions"
4. The site will automatically build and deploy

## Project Structure

```
├── config/
│   └── _default/
│       ├── hugo.toml          # Main Hugo config
│       ├── languages.en.toml  # Language and author config
│       ├── menus.en.toml      # Navigation menus
│       └── params.toml        # Theme parameters
├── content/
│   ├── about.md               # About page
│   ├── contact.md             # Contact page
│   ├── posts/                 # Blog posts
│   └── projects/              # Project showcases
├── static/
│   └── img/                   # Images and assets
├── themes/
│   └── blowfish/              # Blowfish theme
└── .github/
    └── workflows/
        └── hugo.yml           # GitHub Actions deployment
```

## Customization Guide

### Changing Colors

Edit `config/_default/params.toml`:

```toml
colorScheme = "blowfish"  # or "custom"
```

### Adding Social Links

Update `config/_default/languages.en.toml`:

```toml
[params.author]
  links = [
    { github = "https://github.com/username" },
    { linkedin = "https://linkedin.com/in/username" },
    # Add more social links...
  ]
```

### Homepage Layout

Modify the homepage layout in `config/_default/params.toml`:

```toml
[homepage]
  layout = "profile"  # Options: page, profile, hero, card, background
```

## Resources

- [Hugo Documentation](https://gohugo.io/documentation/)
- [Blowfish Theme Docs](https://blowfish.page/)
- [Markdown Guide](https://www.markdownguide.org/)

## License

This project is open source and available under the [MIT License](LICENSE).
