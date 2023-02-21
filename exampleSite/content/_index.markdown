---
title: Home
---

[<img src="https://simpleicons.org/icons/github.svg" style="max-width:15%;min-width:40px;float:right;" alt="Github repo" />](https://github.com/malespiaut/hugo-weekly-devlog)

# weekly-devlog

## _Keep it simple, but not simpler_

**weekly-devloh** is a fork of the **XMin** Hugo theme written by [Yihui Xie](https://yihui.org), with a design inspired from SEGA AM2's weekly-am2 blog.
This theme provides a minimal example to beginners of Hugo templates.
This theme contains less than 200 lines of code in total, including the code in HTML templates and CSS (also counting empty lines).

```bash
find . -not -path '*/exampleSite/*' \( -name '*.html' -o -name '*.css' \) | xargs wc -l
```

```
       5 ./layouts/404.html
      12 ./layouts/_default/single.html
      20 ./layouts/_default/list.html
      13 ./layouts/_default/terms.html
       0 ./layouts/partials/foot_custom.html
       0 ./layouts/partials/head_custom.html
       9 ./layouts/partials/footer.html
      20 ./layouts/partials/header.html
      51 ./static/css/style.css
       7 ./static/css/fonts.css
     137 total
```

This theme is fully functional.
It supports pages (including the home page), blog posts, a navigation menu, categories, tags, and RSS.
With [some customization](https://github.com/yihui/hugo-xmin/blob/master/exampleSite/layouts/partials/foot_custom.html), it can support LaTeX math expressions, e.g.,

`$${\sqrt {n}}\left(\left({\frac {1}{n}}\sum _{i=1}^{n}X_{i}\right)-\mu \right)\ {\xrightarrow {d}}\ N\left(0,\sigma ^{2}\right)$$`

All pages not under the root directory of the website are listed below. You can also visit the list page of a single section, e.g., [posts](/post/). See the [About](/about/) page for the usage of this theme.
