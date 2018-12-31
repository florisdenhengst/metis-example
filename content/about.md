---
title: About Metis
---

**Metis** is a simple Hugo theme for academics, it features a blog section with [MathJax](https://www.mathjax.org/).
It is very, very minimal and you probably want to change it up a bit.

The theme is named after [Metis](https://www.greekmythology.com/Titans/Metis/metis.html), the
Titaness of wisdom, skill and craft who helped Zeus to free his siblings from his fathers' stomach
by creating a potion causing him to vomit them out.

# config.toml

```
[permalinks]
    post = "/post/:year/:month/:day/:slug/"
    note = "/note/:year/:month/:day/:slug/"
```

The menu can be defined here:

```
[[menu.main]]
    name = "Home"
    url = "/"
    weight = 1
[[menu.main]]
    name = "About"
    url = "/about/"
    weight = 2
[[menu.main]]
    name = "Categories"
    url = "/categories/"
    weight = 3
[[menu.main]]
    name = "Tags"
    url = "/tags/"
    weight = 4
[[menu.main]]
    name = "Subscribe"
    url = "/index.xml"
```

Alternatively, you can add `menu: main` to the front matter of your content to make them show up in the menu.

The page footer can be defined in `.Params.footer`, and the text is treated as Markdown, e.g.,

```
[params]
    footer = "&copy; [Floris den Hengst](https://florisdenhengst.github.io)"
```

# Customization 

There are two layout files under `layouts/partials/` that you may want to override: `head_custom.html` and `foot_custom.html`. 

There are only two CSS files in `static/css/fonts.css` and `static/css/style.css` which you may alter as you please.

# Acknowledgements

This theme wouldn't have been possible without the awesome Hugo documentation and the excellent [Xmin](https://xmin.yihui.name/) theme as an example.
