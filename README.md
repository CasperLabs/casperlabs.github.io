# The Casperlabs Blog

This repository contains the source for our statically generated blog. The site is generated using [Jekyll](https://jekyllrb.com/), a static site generator, and hosted on Github Pages automatically.

Posts are written in Markdown or HTML, and are added to the blog when the author creates a pull request and it is approved. The blog supports images, tables and LaTeX equations.

## Workflow

The post author creates a Markdown file under `_posts/` with the filename format `YYYY-MM-DD-title-of-your-blog-post.md`. [Here is an example](https://raw.githubusercontent.com/CasperLabs/casperlabs.github.io/master/_posts/2019-12-17-tps-considered-harmful.md).

To see the generated post without constantly committing changes and waiting for GitHub to rebuild the whole site, the author can run Jekyll locally. Make sure you have [Ruby](https://www.ruby-lang.org/en/) and [Bundler](https://bundler.io/) installed. Then go to the project directory and run the following command on your terminal

```
bundle install
```

After the necessary packages are installed, Jekyll can be run with the livereload feature, which refreshes the browser as changes are saved:

```
bundle exec jekyll serve --livereload
```

This generates the site, and serves it under https://localhost:4000/. Just navigate to that URL and go to the page you are editing. The easiest is to have the editor and the browser tab side by side. Then the author can edit and view the post simultaneously without leaving the editor.
