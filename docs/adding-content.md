---
title: Adding content
permalink: /adding-content.html
---
# Adding Content

All your documentation is located in the **docs** directory. Just like with any Jekyll powered site, you can use Markdown and html in your files. A good starting point for a new entry would be and Markdown file that looks something like this:

```markdown
---
title: Adding content
permalink: /page.html
---
your content here
```

## Adjusting links in the sidebar

Configuration for the sidebar is located in **_data/table_of_contents.yaml** file. Here's an example of this configuration:

```yaml
entries:
  - title: Getting started
    items:
      - title: Installation
        permalink: /getting-started/installation.html
      - title: Running the app
        permalink: /getting-started/running-app-on-emulator.html
      - title: Running the server
        permalink: /getting-started/running-server.html
  - title: Project Structure
    permalink: /project-structure.html
  - title: Configuration
    permalink: /configuration.html
```

**Note:** Permalink attribute needs to match permalink setting in the page content shown above. 
