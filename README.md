# Personal Website

Welcome to my personal website built with Jekyll and hosted on GitHub Pages!

## 📋 Overview

This is a modern, fast, and responsive personal portfolio website. It includes:

- **Homepage**: Introduction and featured content
- **About Page**: Professional background and skills
- **Blog**: Articles and posts about technology and development
- **Projects**: Showcase of projects and open-source contributions
- **Contact**: Get in touch information

## 🚀 Features

- **Static Site Generator**: Built with Jekyll for speed and security
- **Responsive Design**: Works perfectly on desktop, tablet, and mobile
- **Light/Dark Mode Ready**: Styling supports both themes
- **Fast Performance**: Static HTML pages load quickly
- **SEO Optimized**: Built-in SEO tags and metadata
- **GitHub Pages Hosting**: Free hosting directly from this repository

## 🛠️ Getting Started

### Prerequisites

- Ruby (version 2.7 or higher)
- Bundler (install with `gem install bundler`)
- Git

### Local Development

1. Clone this repository:
```bash
git clone https://github.com/mikepham2000/mikepham2000.github.io.git
cd mikepham2000.github.io
```

2. Install dependencies:
```bash
bundle install
```

3. Start the local server:
```bash
bundle exec jekyll serve
```

4. Open your browser and navigate to `http://localhost:4000`

## 📝 Customization

### Edit Site Configuration

Update `_config.yml` with your information:

```yaml
title: "Your Name"
description: "Your site description"
baseurl: ""
url: "https://yourusername.github.io"

author: "Your Name"
author_email: "your.email@example.com"
github_username: "yourusername"
```

### Create Blog Posts

Add new files to the `_posts` directory with the format: `YYYY-MM-DD-post-title.md`

Example:
```markdown
---
layout: post
title: "My First Post"
date: 2024-01-15 10:00:00 -0500
categories: [Technology]
tags: [development]
---

Your post content here...
```

### Update Pages

Edit existing pages in the root directory:
- `index.md` - Homepage
- `about.md` - About page
- `blog.md` - Blog listing
- `projects.md` - Projects showcase
- `contact.md` - Contact information

### Customize Styling

Modify the CSS in `assets/css/style.css` to personalize the look and feel.

## 📂 Project Structure

```
.
├── _config.yml          # Site configuration
├── _layouts/            # HTML templates
├── _includes/           # Reusable components
├── _posts/              # Blog posts
├── _sass/               # Stylesheets (SCSS)
├── assets/              # Images, CSS, JavaScript
├── index.md             # Homepage
├── about.md             # About page
├── blog.md              # Blog page
├── projects.md          # Projects page
├── contact.md           # Contact page
└── Gemfile              # Ruby dependencies
```

## 🌐 Deployment

The site automatically deploys to GitHub Pages when you push to the `main` branch. The GitHub Actions workflow in `.github/workflows/jekyll.yml` handles the build and deployment.

### Enable GitHub Pages

1. Go to repository Settings
2. Navigate to Pages
3. Under "Build and deployment", select "GitHub Actions"
4. The site will be published at `https://yourusername.github.io`

## 💬 Adding a Contact Form

To enable the contact form, use one of these services:

### Option 1: Formspree
1. Go to [formspree.io](https://formspree.io)
2. Create a new form with your email
3. Update the form in `contact.md` with the action attribute

### Option 2: Netlify Forms
If you deploy with Netlify instead:
1. Add `netlify` attribute to the form
2. Forms will be collected in your Netlify dashboard

## 📊 Performance

This static site is optimized for performance:
- Fast load times (all HTML files)
- Lightweight CSS (~5KB)
- No external dependencies at runtime
- Cached assets on GitHub Pages CDN

## 🔐 Security

- No database vulnerabilities
- No server-side code to exploit
- Content versioned in Git
- HTTPS enabled by default on GitHub Pages

## 📚 Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [GitHub Pages Docs](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)
- [YAML Front Matter](https://jekyllrb.com/docs/front-matter/)

## 🤝 Contributing

Feel free to fork this repository and customize it for your own use!

## 📄 License

This project is open source and available under the MIT License.

---

**Built with ❤️ using Jekyll**
