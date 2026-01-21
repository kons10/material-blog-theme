# hugo-blog-theme

A hugo theme for [kons10](https://hugo.kto.f5.si/)

## Install

```sh
mkdir theme
cd theme
git submodule add https://github.com/m1yam0t0/hugo-blog-theme.git hugo-blog-theme
```

## Update

```sh
git submodule update --init --recursive
```

## Configuration

### Menu

You can add entries to menus from `config.toml`.

See [Add Non-content Entries to a Menu.](https://gohugo.io/content-management/menus/#add-non-content-entries-to-a-menu)

This is a example configuration.

```toml
[[menu.main]]
  name = "Posts"
  url = "/posts/"
  weight = 1
  [menu.main.params]
    icon = "article"

[[menu.main]]
  name = "Tags"
  url = "/tags/"
  weight = 2
  [menu.main.params]
    icon = "label"

[[menu.main]]
  name = "About"
  url = "/about/"
  weight = 3
  [menu.main.params]
    icon = "info"
```

**Note:** The `icon` parameter is optional. If provided, the menu will display Material Design icons. If omitted, it will display text links instead. You can find available icon names at [Google Fonts Icons](https://fonts.google.com/icons).

### Social Links

You can add entries to use `config.toml`.

This is a example configuration.

```toml
[[Params.social]]
  name = "GitHub"
  url = "https://github.com/m1yam0t0"

[[Params.social]]
  name = "Twitter"
  url = "https://twitter.com/m1yam0t0"
```
