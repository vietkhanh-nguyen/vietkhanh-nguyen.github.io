# Personal Website of Nguyen Viet Khanh

Welcome to my personal website repository! This website showcases my projects, publications, and professional profile, and serves as a portfolio for my work in autonomous systems, smart aerospace, and robotics.

## 🚀 Features

* **About Me**: Learn about my research interests and professional background.
* **Publications**: Browse my research papers and articles, with links to full-text PDFs where available.
* **Projects**: Explore my work on robotics, automation, and smart systems.
* **Blog**: Posts about my insights, research updates, and tutorials.
* **Contact**: Easy way to reach me for collaboration, questions, or networking.

## 🛠 Tech Stack

* **Static Site Generator**: Jekyll
* **Theme**: [Academicpages](https://academicpages.github.io)
* **Languages**: HTML, CSS, Markdown, Liquid (Jekyll templating)
* **Hosting**: GitHub Pages

## 💾 Repository Structure

```
.
├── _config.yml        # Jekyll configuration file
├── _includes/         # Reusable HTML components
├── _layouts/          # Layout templates
├── _posts/            # Blog posts
├── _pages/            # About, Projects, Publications pages
├── assets/            # CSS, JS, images
└── README.md          # Project documentation
```

## ⚡ Installation & Local Development

1. **Clone the repository**

```bash
git clone https://github.com/vietkhanh-nguyen/vietkhanh-nguyen.github.io.git
cd vietkhanh-nguyen.github.io
```

2. **Install dependencies**
   Make sure you have Ruby and Bundler installed:

```bash
bundle install
```

3. **Serve locally**

```bash
bundle exec jekyll serve -l -H localhost
```

Visit `http://localhost:4000` to see your website.

## 🔖 Contributing

This is my personal website, so contributions are limited to myself. However, feedback or suggestions via GitHub issues are welcome!

## 📜 License

Content is available under [MIT License](LICENSE). Feel free to fork and adapt for personal use.

## Fix bug video not display
'''bash
ffmpeg -i <your video>.mp4 -movflags faststart <new name>.mp4
'''
