# Run

## 本地开发
```bash
# install jekyll: https://jekyllrb.com/docs/installation/macos/
bundle install
bundle add webrick

bundle exec jekyll serve
# Open it in your browser: http://localhost:4000
```

## Docker 部署
```bash
# 构建并运行 Docker 容器
docker-compose up --build

# 或者使用 Docker 命令
docker build -f deployment/Dockerfile -t jekyll-tailpages .
docker run -p 8080:80 jekyll-tailpages

# 访问网站: http://localhost:8080
```

# About

Tailpages (Tailwind + Github Pages) is a Jekyll website template based on TailwindCSS, which can be hosted by Github for free. You can visit the demo site at [https://harrywang.me/](https://harrywang.me/).

Key features are:

- Minimalist design inspired by the [indigo template](https://github.com/sergiokopplin/indigo)
- Elegant typography via [TailwindCSS Typography plugin](https://tailwindcss.com/docs/typography-plugin) and [Inter font](https://rsms.me/inter/)
- Markdown support for content authoring (static pages and blogs)
- Code highlighting and styling via [highlight.js](https://highlightjs.org/) (see [code example](http://harrywang.me/tailpages/2022/02/07/code.html))
- Latex support via [MathJax](https://www.mathjax.org/) (see an [example](http://harrywang.me/tailpages/2022/02/09/latex.html))
- Table of Contents support via [jekyll-toc](https://github.com/allejo/jekyll-toc) (see an [example](http://harrywang.me/tailpages/toc))

### Tutorials
- No-code Tutorial: this tutorial shows how you can use Tailpages template to quickly setup your website and blogs without coding, which you can access at [medium](https://harrywang.medium.com/introducing-tailpages-tailwind-github-pages-89903c52d3ec) or [blog](https://harrywang.me/tailpages-tutorial-nocode).
- Technical Tutorial: this tutorial shows how to setup the development environment for Tailpages from scratch, which you can access at [medium](https://harrywang.medium.com/developing-tailpages-a-jekyll-template-based-on-tailwind-css-b8b51e60e25b) or [blog](https://harrywang.me/tailpages-tutorial-technical). 
