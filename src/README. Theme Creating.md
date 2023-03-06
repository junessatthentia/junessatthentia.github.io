# Theme Creating

## 1. Create Theme Folder
Inside src/themes/ named with "themeName". For example "src/themes/wiredassent".

## 2. Create sass files
Inside theme folder:
1. _variables.sass - unique theme variables.
2. theme.sass - main theme file which will be compiled to CSS.

## 3. Create favicon
1. Create favicon files using:
https://realfavicongenerator.net/
2. Put files into src/themeName/favicon
3. Also create _favicon.html file in src/themeName/favicon. 
4. Copy favicon html from Realfavicongenerator to _favicon.html, something like:


```bash
<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
<link rel="manifest" href="/site.webmanifest">
<link rel="mask-icon" href="/safari-pinned-tab.svg" color="#5bbad5">
<meta name="msapplication-TileColor" content="#da532c">
<meta name="theme-color" content="#ffffff">
```
5. Remove slash from href="/image..." (href="image...").

Restart Gulp and it will copy files into dist/themeName/favicon and inserts _favicon.html to html pages <head>. 


## 4. Start Gulp to compile themes
#### For development:
```bash
gulp
```
Contains SASS-Sourcemaps

#### For production:

```bash
gulp-prod
```
Minified CSS, Optimized Images

## 5. When creating New Theme
Restart gulp to compile it.
