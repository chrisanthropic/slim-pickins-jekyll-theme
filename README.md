slim-pickins-jekyll-theme
=============

Live Demo [HERE](http://chrisanthropic.github.io/slim-pickins-jekyll-theme/)

Slim Pickins is what I consider to be a minimal 'core' theme with everything I need to quickly develop new themes for Jekyll.

## Basic features include:

* SASS
* Responsive grid
* Responsive navigation
* Sticky footer
* Javascript free*
* Custom Rakefile with tasks for deploying, minifying, optimizing images, and notifying search engines about updates

### SASS
Includes the following variables:

**Base Colors**
* $primary-color
* $secondary-color
* $complimentary-color
* $body-bg
* $text-color

**Text**
* $base-font-family
* $base-font-size
* $small-font-size
* $base-line-height


**Primary Navbar Settings**
* $navbar-color
* $navbar-text-color
* $navbar-hover-color

**Socials Navbar Settings**
* $socials-text-color
* $socials-hover-color

**Utility**
* $spacing-unit

**Footer**
* $footer-height
* $footer-color

### GRID
Uses minimal sass [components](https://github.com/zurb/bower-foundation/tree/master/scss/foundation/components) from Zurb Foundation:

* [grid](http://foundation.zurb.com/docs/components/grid.html)
* [visibility](http://foundation.zurb.com/docs/components/visibility.html)
* [media query](http://foundation.zurb.com/docs/media-queries.html)

### NAVIGATION
A fully responsive navigation bar with the following features:

* 2 navigation areas
  * Left - Primary navigation 
  * Right - Social media links
* Both navigation areas are populated using Jekyll 'data' files, nav.yml and socials.yml respectively
* Easily customizable text, link, and background colors using the supplied sass variables

### STICKY FOOTER
I like my footers to stay on the bottom of the page no matter what. You can easily edit the size and color using the supplied sass variables.

### JAVASCRIPT FREE
The only thing in the theme that uses Javascript is the optional use of google analytics.

### RAKEFILE
Includes the following custom tasks:

* *optimizeimages* - uses minimagick to compress and optimize all images in the /images folder.
* *minify_html* - uses HTML_compressor to minify HTML
* *notify* - pings google and bing to notify them about changes to the site/sitemap

These 3 tasks have been bundled into custom build and deploy tasks

* *build* - runs `jekyll build` and then `optimize images` followed by `minify_html`
* *deploy* - runs `s3_website push` and then `notify`

## Basic Use
For now theming on Jekyll sucks in that it's not super easy to change themes. For now it's best to start fresh or install the them and then transfer over any old files (posts, images, etc) from your old site.

* Git clone this repo, cd into the directory and run `bundle install --binstubs --path=vendor` to install the required dependencies.
* Edit your config.yml file
  * Change the title and description at a minimum.
* Update your navigation 
  * edit the `_data/nav.yml` file as needed
* Update your social links
  * edit the `_data/socials.yml` file as needed
* For google analytics just add your google_universal_analytics ID to the _config.yml file.

## Deploying
I use S3 to host my site and the [s3_website](https://github.com/laurilehmijoki/s3_website) plugin to deploy, if you don't do both of these, delete the `s3_website.yml` file and edit the deploy raketask to fit your needs.

If you plan on using S3 make sure you edit the configs:

* FIRST - add the s3_website.yml file to your gitignore so your credentials don't end up on the web.
* s3_website.yml
  * add your `s3_id`. `s3_secret`, and `s3_bucket`
* Update the Rakefile notify task to use your url
  * replace `site = "www.YOUR-URL.com"` with your actual url.

## MISC.
The blog posts included are duplicated from my actual blog and are the documentation of how I created this theme. From starting with a fresh Jekyll installation to the final product.