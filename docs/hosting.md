---
title: Hosting
permalink: /hosting.html
---

# Hosting your Documentation

With Jekyll and Github hosting is easy. Head to **Settings** tab of your Github repository and scroll down to **GitHub Pages** section. Specify which branch you want to use and additionally adjust domain information. Take note of the url for your documentation and head to **config.yaml** and update _base_url_ option:

```yaml
baseurl: 'https://YOURORG.github.io/PROJECT_NAME/'
```   