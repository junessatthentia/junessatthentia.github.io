# Disclaimer

# Date Time Picker and A-Checker
Flatpickr.js used as a Date Time Picker. It's source code changed to add accesebility.
!!! DO NOT replace flatpickr.js with a newer version or if replace add changes !!!
Changes in flatpickr.js commented with:
// A-Cheker correction Start. Thentia
  ...Some new or changed code
// A-Cheker correction End. Thentia

# Versions:
npm: 6.9.0
Node.js 11
Temporary solution to keep build system working

# Themes Compilation

Gulp compiles themes.
Folder common/ - contain common assets - pug, sass, images, fonts, js.
Folder themes/ - contain themes folders. Gulp automatically takes names of folders and compiles them into themes.
Each themeName folder (wiredassent, metricshub ... etc) have unique images img/ - which also to be added to dist/themeName/img/ folder.
Each compiled theme is independent and includes all needed assets - theme css, fonts, images, js, html.
File src/index.pug - is navigation page with list of themes. Which you see in website root (or in http://localhost:3000). To be compiled to dist/ folder.

## Gulp AUTOMATICALLY !!! DELETES /DIST FOLDER !!! - before compile themes (gulpfile.js > task 'clean-and-start'). Make sure to !!! PUT ALL ASSETS INTO SRC/ FOLDER !!!

## Gulp.js Template for Design to HTML Work

SASS/Pug Compilcation, Server/Livereload, Images Optimization, CSS minification.

## Quick Start

You should have installed Node.js

```bash
# Navigate to project folder with package.json and gulpfiles.js and Install Gulp dependencies
npm install

# Default task - for development. Provides SASS/SCSS Sourcemaps and NOT-minified CSS. Starts Server/Livereload, SASS, Pug
gulp

# Production task - provides minified CSS, without Sourcemaps. Then starts Server/Livereload, SASS, Pug
gulp prod

```
