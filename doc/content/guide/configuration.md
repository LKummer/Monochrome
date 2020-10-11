---
title: 'Configuration'
description: 'Set up your site and page configurations.'
categories:
  - 'Application'
---

This guide assumes you are starting with the configuration of the quick start
(_demo_) site. It only describes the options the theme provides, not which Hugo
options should be set for the theme to work.

## Site Configuration

To set a favicon, use the `params.site.favicon` option. Make sure the location
does not start with `/` to avoid Hugo URL resolution quirks.

To set which section (or page) is rendered as the index, use the
`params.site.indexSection` option.

```toml
[params]
  [params.site]
    favicon = "favicon.svg"
    indexSection = "article"
```

[Read the SEO guide]({{< ref "seo.md" >}})
for information about search engine optimization related options.

## Page Configuration

For the best results, set the `title`, `date`, `tags` and `description` front
matter options of each content page.

```toml
+++
title = "Title of Your Article"
date = "2020-10-20"
description = "Description of your article."
tags = [
    "markdown",
    "text",
]
+++
```

A `minimal` layout is available for single pages where you wish the page wont
render a title, date and tags above the content. It is used in the about page
of the demo.

```toml
+++
layout = "minimal"
+++
```

Do not forget to [check out the SEO guide]({{< ref "seo.md" >}}) to configure
your pages for optimal results.
