# Doctor Jekyll

Doctor Jekyll is a fork of [Lanyon](https://github.com/poole/lanyon), a [Jekyll](http://jekyllrb.com) theme, built specifically for publishing documentation. It includes a few useful addition over Lanyon such as:

- Algolia search
- Sass based styles
- Pagination
- Github & Twitter buttons


## Contents

- [Usage](#usage)
- [Configuration](#configuration)
  - [Table of Contents](#table-of-contents)
  - [Themes](#themes)
  - [Algolia](#algolia)
  - [Github button](#github-button)
- [Development](#development)
- [Author](#author)
- [License](#license)


## Configuration

Doctor Jekyll is a theme built on top of [Poole](https://github.com/poole/poole), which provides a fully furnished Jekyll setup—just download and start the Jekyll server. See [the Poole usage guidelines](https://github.com/poole/poole#usage) for how to install and use Jekyll.

### Table of contents

Overwrite the `table_of_content.yaml` in the `_data` folder.

### Themes

Doctor Jekyll leverages the eight color themes defined by Lanyon. You can update the theme color by updating `_sass/_variables.scss`:

```scss
/* Selected Theme */
$theme_color: $red;
```

### Algolia

TODO

### Github Button

You can configure the URL of the Github button in `_config.yml`:

```
github:
  repository_url:    https://github.com/bakery/doctor-jekyll
```

### Responsive Layout

By default, the navigation sidebar is shown above the `$medium-bp` breakpoint (860px). Below that screen width, the navigation menu is hidden and the drawer icon appears to toggle the menu. You can change the breakpoint value in  `_variables.scss`. 


## Credits

**Mark Otto** for building Lanyon & Poole.

- <https://github.com/mdo>
- <https://twitter.com/mdo>


## License

Open sourced under the [MIT license](LICENSE.md).

<3
