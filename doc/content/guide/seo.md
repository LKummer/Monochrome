---
title: 'Search Engine Optimization'
description: 'Learn to configure SEO features correctly.'
categories:
  - 'Application'
---

The theme includes structured data for search engine optimization. Make sure to
configure all options correctly to achieve the best results.

## Site Configuration

Configuring the site title and author(s) in the site configuration are required
for the structured data to be correctly formed. 

```toml
title = "Hugo Themes"

[author]
  name = "Steve Francia"
```

A description, organization logo and default article images are also required.

The organization logo `params.seo.logo` image must be in either JPG or PNG
format, and sized 600px wide and 60px high.
[As per Google's AMP logo guidelines](https://developers.google.com/search/docs/data-types/article#logo-guidelines).

The default article images `params.seo.defaultImages` should contain three
images, all of them at least 1200px wide.
The images should have 1x1, 4x3 and 16x9 aspect ratios for the best results.
For more information
[see the documentation of the image property of articles](https://developers.google.com/search/docs/data-types/article#article-types).

```toml
[params]
  [params.seo]
    description = "Monochrome theme demo website."
    logo = "logo.png"
    defaultImages = [
      "image-1x1.png",
      "image-4x3.png",
      "image-16x9.png"
    ]
```

**Do not** begin image locations with a `/` as it will cause issues with Hugo's
URL functions.

## Page Configuration

Each page should have a `description` and optimally it's own `images`.

Page `images` _should_ follow the same guidelines as `defaultImages`.

```toml
description = "Nice description for your article."
images = [
  "image-1x1.png",
  "image-4x3.png",
  "image-16x9.png"
]
```
