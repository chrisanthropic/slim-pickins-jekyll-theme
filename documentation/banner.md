---
layout: page
title: "banner"
permalink: /documentation/banner.html
---  
This theme is configured with a 'wrap' of 1920px so banner images look best at that width.

First it checks a pages yaml frontmatter for the header image, if none is found then it checks for a site-wide default in your config.yml, if none is found then no banner image is displayed.

**Site-Wide**
You can set a site-wide default banner image by adding the following to your _config.yml:
  `header_image: "path/to/image.jpg"`

**Per Page**
You can also override it per page by adding the following code to a pages yaml front matter:
  `header_image: path/to/image.jpg`


