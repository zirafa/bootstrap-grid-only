Bootstrap-Grid-Only (3.2.0)
===================

Bootstrap's responsive grid and responsive utility classes only, without any extras. Lightweight yet still powerful. Style to taste. 

# Instructions
Include one of the precompiled grids (grid12.css, grid24.css, grid30.css, grid100.css) in your site, or customize and compile grid.css.less with command line lessc or LessPHP (no extends are used). 

# Included
- Standard [Bootstrap grid classes](http://getbootstrap.com/css/#grid): columns, offsets, push and pull classes
- Standard [Bootstrap responsive utility classes](http://getbootstrap.com/css/#responsive-utilities): .visible-\*, .hidden-\*
- Clearfix class, * {box-sizing:border-box} declaration, pull-right, pull-left.
- Precompiled stylesheets for 12, 24, 30, and 100 columns. Gutter-width for each is respectively 30px, 15px, 10px, 2px. The 100 column grid yields results similar to [Unsemantic](http://unsemantic.com/) and is good if you like semantic class naming (col-md-50 means exactly 50% width) or need extremely granular layout positioning (62 col + 38 col) 
- LESS file grid.css.less for building your own bootstrap grid, including variables for the grid ( @grid-columns, and @gutter-width) as well as breakpoint cutoff declarations (@screen-xs, @screen-sm, @screen-md, @screen-lg)

# What's not included:
- Pretty much everything else. It's really up to you. No styles, no javascript - not even a CSS reset.

# Notes
You could also use [Bootstrap's Customizer](http://getbootstrap.com/customize/) to compile only the grid + responsive utilities you need. Actually, I recommend trying that first (here's a [config.json](https://gist.github.com/anonymous/e9d4b16ac54805b9ec6f)). However, for my needs, I wanted total control over class naming and reduced LESS file count, and needed to support LessPHP.

I needed LESS files in order to do server-side compilation with LessPHP on a Drupal site. LessPHP doesn't support extends, which this version doesn't have. This may also save you time in having to sift through the Bootstrap LESS source files, and allow you to understand and deconstruct how the grid is made. For instance, I had a project where I needed to change all the class names col-xs, col-md, col-sm, col-lg to match an existing convention: col-mobile, col-narrow, col-normal, col-wide. 
