+++
title = "Building My Portfolio Blog with Hugo"
date = "2025-09-19"
author = "kiteflinty"
cover = "hello.jpg"
description = "How I built my personal portfolio site as a blog using Hugo"
tags = ["Hugo", "Static Site Generator", "Web Development", "Portfolio"]
+++

# Why Hugo?

I wanted a **fast, lightweight, and customizable** way to showcase my projects, thoughts, and ideas. My search led me to static site generators, and **Hugo** immediately stood out. Unlike traditional content management systems like WordPress, which rely on databases and a heavy backend, Hugo generates a complete set of static HTML files. This approach makes sites incredibly fast, secure, and easy to host.

Here's what sold me on Hugo:

  * **Blazing-fast builds:** It can render a large site with thousands of pages in seconds, a massive time-saver.
  * **Markdown-based content:** Writing blog posts and project descriptions in Markdown feels natural and lets me focus on the content itself without worrying about complex editors.
  * **Flexibility and themes:** There's a huge collection of high-quality, free themes available, and they're all highly customizable. If I wanted to build something from scratch, Hugo's templating system makes that straightforward, too.
  * **Simple hosting:** Because the output is just a folder of static files, you can host a Hugo site for free on services like GitHub Pages, Netlify, or Vercel.

-----

# Setting Up the Blog

Getting started with Hugo was a breeze. After installing it on my machine, I created the core structure for my site with a single command:

```bash
hugo new site portfolio-blog
```

This command created a new directory named `portfolio-blog` with all the necessary folders like `content`, `layouts`, `static`, and `config.toml`.

Next, I needed to pick a theme. I browsed the official [Hugo Themes website](https://themes.gohugo.io/) and chose one that was clean and modern. To add it to my project, I used git:

```bash
cd portfolio-blog
git init
git submodule add https://github.com/the-theme-repo/the-theme-name.git themes/the-theme-name
```

I then updated my `config.toml` file to tell Hugo which theme to use.

```toml
baseURL = "https://example.org/"
languageCode = "en-us"
title = "My Awesome Portfolio"
theme = "the-theme-name"
```

-----

# Creating Content

Now for the fun part: adding my content. I created my first blog post using the command line:

```bash
hugo new posts/building-my-portfolio-with-hugo.md
```

This created a new Markdown file inside the `content/posts` folder with some basic metadata (front matter) at the top. All I had to do was fill in the title, date, description, and start writing.

To see my changes in real time, I ran the Hugo server:

```bash
hugo server -D
```

This command started a local web server, and I could view my site in my browser at `http://localhost:1313`. The `-D` flag is important as it ensures that draft posts are also rendered. As I edited my Markdown files, the changes instantly appeared in the browser, making the development process incredibly fast and efficient.

-----

# The Final Result

The process of building my portfolio blog with Hugo was a fantastic experience. I now have a professional-looking site that's **fast, secure, and incredibly easy to maintain**. I can quickly write new blog posts, showcase new projects, and have full control over the design without the overhead of a complex database or server-side code. If you're looking for a simple yet powerful way to build your next website, I highly recommend giving Hugo a try.
