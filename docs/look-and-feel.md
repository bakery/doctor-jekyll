---
title: Look and Feel
permalink: /look-and-feel.html
---
# Look and Feel

There are a couple of things you can tweak to customize what your documentation looks like.

## Themes

Doctor Jekyll leverages the eight color themes defined by [Lanyon](https://github.com/poole/lanyon). You can update the theme color by updating **_sass/_variables.scss**:

```scss
/* Selected Theme */
$theme_color: $red;
```

## Responsive Layout

By default, the navigation sidebar is shown above the `$medium-bp` breakpoint (960px). Below that screen width, the navigation menu is hidden and the drawer icon appears to toggle the menu. You can change the breakpoint value in  **_variables.scss**. 