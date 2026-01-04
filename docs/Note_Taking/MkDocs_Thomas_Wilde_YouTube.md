---
tags:
  - MkDocs
---
# Create MkDocs Documentation Site Thomas Wilde Video
### Normal Install Stuff
- Create and activate a virtual environment

``` shell
pip install mkdocs-material mkdocs
mkdir MyAwesomeWebsite
cd MyAwesomeWebsite
mkdocs new .
mkdocs serve
```

### Navigation
- Create about folder and put two files in it - about.md and childhood.md
 - edit mkdocs.yml
	 - He didn't explain much of this so I'll have to look at the docs to see if I really want all of these options. 
	 - I'm pretty sure navigation.tabs puts the navigation at the top rather than in the sidebar. 
	 - navigation.tabs.sticky means you can always see the tabs at the top of the web page no matter how far you tab down. 
	 - navigation.top puts a back to top button on an article so it's easy to go back to the beginning
	 - toc.integrate moves the table of contents in articles (made from subheaders) to the left sidebar. Default is right.
	 - content.copy.code puts a copy button inside code blocks.

``` yaml title="mkdocs.yml"
 theme:
   name: material
   palette: 
     # Palette toggle for light mode
     - scheme: default
       toggle:
	     icon: material/brightness-7 
	     name: Switch to dark mode
     # Palette toggle for dark mode
     - scheme: slate
       toggle:
	     icon: material/brightness-4
	     name: Switch to light mode
   features:
     - navigation.instant
     - navigation.instant.progress
     - navigation.tracking
     - navigation.tabs
     - navigation.tabs.sticky
     - navigation.sections
     - navigation.expand
     - navigation.top
     - search.suggest
     - search.highlight
	 - search.sharing
     - content.code.copy
plugins:
	- search
	- tags:
	    tags_file: tags.md
    - blog
      - blog/index.md

markdown_extensions:
  - pymdownx.highlight:
      anchor_linenums: true
      line_spans: __span
      pygments_lang_class: true
  - pymdownx.inlinehilite
  - pymdownx.snippets
  - pymdownx.superfences
	         
nav:
  - Home: index.md
  - Code Docs:
    - Java: coding/my-first-java-file.md
  - About:
    - About Me: about/about.md
    - Childhood: about/childhood.md
  - Tags: tags.md
  - Blog:
    - blog/index.md
      
```

### Tags
- added tags plugin to mkdocs.yml
- Created tags.md at top level of docs (docs/tags.md)
``` markdown
# Tags

My Tags

<!-- material/tags -->
```
### Code Blocks
- You can have a title on a code block. Don't forget the quotes
``` python title="Print Statement"
print("Testing")
```
- You have to have a blank line after a code block

### Blogging
- Posts require some metadata

``` yaml title="Blog Post Template"
---
date: 2024-01-31
categories: 
  - Documentation
tags:
  - MkDocs
---

# My first blog post!

Today I learned how to deploy a documentation site!

```

### Git Deployment
- Not sure I care. Starts at 17 minutes of the video if I decide to go back.
