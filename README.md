Bootstrap-Grid-Only (3.2.0)
===================

Bootstrap's responsive grid and responsive utility classes only, without any extras. Lightweight yet still powerful. Add styles to taste. 

# Instructions
Include one of the precompiled grids (grid12.css, grid24.css, grid30.css, grid100.css) in your site, or customize and compile grid.css.less with command line lessc or LessPHP (no extends are used). 

# Included
- Standard [Bootstrap grid classes](http://getbootstrap.com/css/#grid): columns, offsets, push and pull classes
- Standard [Bootstrap responsive utility classes](http://getbootstrap.com/css/#responsive-utilities): .visible-\*, .hidden-\*
- Clearfix class, * {box-sizing:border-box} declaration, pull-right, pull-left.
- Precompiled stylesheets for 12, 24, 30, and 100 columns. Gutter-width for each is respectively 30px, 15px, 10px, 10px. The 100 column grid yields results similar to [Unsemantic](http://unsemantic.com/) and is good if you like semantic class naming (col-md-50 means exactly 50% width) or need extremely granular layout positioning (62 col + 38 col) 
- LESS file grid.css.less for building your own bootstrap grid, including variables for the grid ( @grid-columns, and @gutter-width) as well as breakpoint cutoff declarations (@screen-xs, @screen-sm, @screen-md, @screen-lg)

# What's not included:
- Pretty much everything else. It's really up to you. No styles, no javascript - there isn't even a reset.css or normalize.css included. 
