---
tags:
  - MkDocs
---

# Create MkDocs Blog James Willet Video 

### Initial Setup

- sets blog directory to . since this is only a blog. All posts will just go in the docs folder

``` yaml title="mkdocs.yml"
site_name: Our Awesome Blog
site_description: A blogging site built with Material for MkDocs
site_url: https://sitename.example
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
plugins:
  - search
  - blog:
      blog_dir: .
```

- Now remove everything from docs/index.md and it's just:

``` markdown title="docs/index.md"
# Blog
```
### Creating Posts
- An empty posts folder is created under docs automatically.
- Created docs/posts/firstpost.md and secondpost.md and thirdpost.md

``` markdown title="firstpost.md"
---
date:
  created: 2024-11-06
  categories: 
    - Tech
  tags:
    - technology
---

# My First Blog Post

This is the text for my first blog post.

<!-- more -->

All the text here appears in the blog post.
```

- `draft: true` means the post appears in mkdocs serve but not in mkdocs build.

``` markdown title="secondpost.md"
---
date:
  created: 2024-11-09
draft: true
categories:
  - Tech
  - Lifestyle
tags:
  - Health
---

# My Second Post!

This is my second blog post. I'm actually setting it as a draft so it doesn't appear yet...

<!-- more -->

lorem ipsum text here.
```

``` markdown title="thirdpost.md"
---
date:
  created: 2024-12-07
  updated: 2024-12-08
readtime: 5
---

# My Third Blog Post

This is the text for my third blog post.

<!-- more -->

lorem ipsum again
```

- MkDocs automatically calculates readtime, but you can set it as above.
- You can put subdirectories under posts. He created one called lifeupdates.
- To add an image to a blog post:

`![Cartoon Software Engineer](cartoonEngineer1.png)`

- MkDocs creates an archive by year.
- If you want it to break the archive down by month and year instead of the default of just year:

``` yaml title="blog part of mkdocs.yml"
- blog:
    blog_dir: .
    archive_date_format: MM/yyyy
    archive_url_date_format: MM/yyyy
```

- You can limit what categories are allowed in mkdocs.yml. 
- He also added in tags, but the video is old enough that he used a tag_file. So what I did in the Thomas Wilde video should be used instead.
- He showed setting up different authors. Not relevant to me. Uses a file called `.authors`
- Authors file can include avatars and links (like to his Youtube page)
- Can set slugs (urls). He doesn't like the default date in the slug. Again in blog part of mkdocs.yml `post_url_format: "{slug}"`
- Can set slug in metadata of a blog post if you want `slug: my-first-post`
- Skipped rss feed, social media buttons, comments using Discuss 3rd party app, git revisions, and github deployment.
