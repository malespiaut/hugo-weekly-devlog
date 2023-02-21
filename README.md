# weekly-devlog Hugo theme

## _Keep it simple, but not simpler_

**weekly-devlog** is a fork of the *XMin* Hugo theme written by [Yihui Xie](https://yihui.org), that is inspired by the [“weekly-am2” blog from SEGA AM2](https://web.archive.org/web/20040703062543id_/http://www.sega-am2.co.jp/jp/wam2/2004/2004_06_29/2004_06_29_1.html).

The complete source code doesn't exceed 200 lines.

```bash
find . -not -path '*/exampleSite/*' \( -name '*.html' -o -name '*.css' \) | xargs wc -l
```

```
 107 ./static/css/style.css
   1 ./static/css/fonts.css
  24 ./layouts/partials/header.html
   0 ./layouts/partials/head_custom.html
   9 ./layouts/partials/footer.html
   0 ./layouts/partials/foot_custom.html
  13 ./layouts/_default/terms.html
  12 ./layouts/_default/single.html
  20 ./layouts/_default/list.html
   5 ./layouts/404.html
 191 total
```

## License

This project is licensed under the MIT License. See the LICENSE file for details.
