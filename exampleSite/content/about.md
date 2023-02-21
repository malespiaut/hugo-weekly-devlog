---
title: About weekly-devlog
author: Marc-Alexandre Espiaut
---

**weekly-devlog** is a fork of the *XMin* Hugo theme that aims to mimic the SEGA AM2's weekly-am2 devlog.
It also aims to keep things as minimal as possible to stay easy to use for both blog maintainers and readers.

# config.yaml

This example site can be modified to have permalinks defined for two sections, `post` and `note`, or more.
Links to pages under these directories will contain the date info, e.g., `https://siteurl/post/2016/02/14/a-plain-markdown-post/`.
This is optional, and it is up to your personal taste of URLs.

```yaml
permalinks:
  note: "/note/:year/:month/:day/:slug/"
  post: "/post/:year/:month/:day/:slug/"
```

You can define the menu through `menu.main`, e.g.,

```yaml
menu:
  main:
    - name: Home
      url: ""
      weight: 1
    - name: About
      url: "about/"
      weight: 2
    - name: Categories
      url: "categories/"
      weight: 3
    - name: Tags
      url: "tags/"
      weight: 4
    - name: Subscribe
      url: "index.xml"
```

Alternatively, you can add `menu: main` to the YAML metadata of any of your pages, so that these pages will appear in the menu.

The page footer can be defined in `.Params.footer`, and the text is treated as Markdown, e.g.,

```
params:
  footer: "&copy; [Yihui Xie](https://yihui.org) 2017 -- {Year}"
```

Here `{Year}` means the year in which the site is built (usually the current year).

# Custom layouts

There are two layout files under `layouts/partials/` that you may want to override: `head_custom.html` and `foot_custom.html`.
This is how you inject arbitrary HTML code to the head and foot areas.
For example, this site has a file `layouts/partials/foot_custom.html` to support LaTeX math via MathJax and center images automatically:

```html
<script defer src="//yihui.org/js/math-code.js"></script>
<script defer src="//mathjax.rstudio.com/latest/MathJax.js?config=TeX-MML-AM_CHTML">
</script>

<script defer src="//yihui.org/js/center-img.js"></script>
```

You can certainly enable highlight.js for syntax highlighting by yourself through `head_custom.html` and `foot_custom.html` if you want.

If you do not like the default fonts, you may provide your own `static/css/fonts.css` under the root directory of your website to override the `fonts.css` in the theme.

# Other features

This theme can support additional features, such as:

- [Enable Google Analytics](https://github.com/yihui/hugo-xmin/pull/3)

- [Enable Disqus comments](https://github.com/yihui/hugo-xmin/pull/4)

- [Enable highlight.js for syntax highlighting of code blocks](https://github.com/yihui/hugo-xmin/pull/5)

- [Display categories and tags on a page](https://github.com/yihui/hugo-xmin/pull/2)

- [Add a table of contents](https://github.com/yihui/hugo-xmin/pull/7)

- [Add a link in the footer of each page to "Edit this page" on Github](https://github.com/yihui/hugo-xmin/pull/6)

To fully understand these examples, you have to read [the section on Hugo templates](https://bookdown.org/yihui/blogdown/templates.html) in the **blogdown** book.

# Conclusion

The source code of the original XMin theme is [on Github](https://github.com/yihui/hugo-xmin).
Happy hacking!
