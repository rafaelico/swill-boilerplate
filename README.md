# Swill Boilerplate

![Swill Boilerplate Logo](https://raw.githubusercontent.com/tiagoporto/swill-boilerplate/stylus-version/src/images/touch/chrome-touch-icon-192x192.png)

Boilerplate Front-End with [Gulp.js](http://gulpjs.com/), all you need to start multi-device development for business proposals.

> If you're like me and prefer stylus use the [stylus-version](https://github.com/tiagoporto/swill-boilerplate/tree/stylus-version).
>
> If you will work with Ionic you use the [mobile-version](https://github.com/tiagoporto/swill-boilerplate/tree/mobile-version).

## Table of Contents

* [Technologies](#technologies)
* [Includes](#includes)
* [Features](#features)
* [Folder Structure](#folder-structure)
* [Installing Dependencies](#installing-dependencies)
* [Usage](#usage)
	* [Tasks](#tasks)
	* [AngulaJS](#angularjs)
	* [BrowserSync](#browsersync)
	* [Bitmap Sprite](#sprite)
	* [SVG Sprite](#svg*sprite)
* [License](license)

## Technologies

Uses the following technologies:

* [Autoprefixer](https://github.com/postcss/autoprefixer)
* [Bower](http://bower.io/)
* [BrowserSync](http://www.browsersync.io/)
* [EditorConfig](http://editorconfig.org/)
* [Gulp.js](http://gulpjs.com/)
* [JSHint](http://www.jshint.com/)
* [Node.js](http://nodejs.org/)
* [NPM](https://www.npmjs.com/)
* [Sass](http://sass-lang.com/)

## Includes

* [AngularJS](http://angularjs.org/)
* [Animate.css](http://daneden.github.io/animate.css/)
* [Font Awesome](http://fortawesome.github.io/Font-Awesome/)
* [Google Analytics](http://www.google.com/analytics/)
* [jQuery](http://jquery.com/)
* [Normalize.css](http://necolas.github.io/normalize.css/)
* [Outdated Browser](http://outdatedbrowser.com/)
* [Retina.js](http://imulus.github.io/retinajs/)
* [Semantic GRID SYSTEM](http://semantic.gs/)
* [Twitter Bootstrap](http://getbootstrap.com/)

## Features

* Clean the assets (images, css, js) in the project to maintain the directory organized
* Compress Images
* Generate Sprites with .png
* Generate Sprites with .svg and a fallback .png
* Concatenate And Minify Scripts
* Analyze JavaScript with jshint
* Compile Sass
* Functions and mixins to use with Sass
* Notify when tasks are complete
* Monitors changes in the files and reload browser with [BrowserSync](http://www.browsersync.io/)
* Configs from [HTML5 Boilerplate](https://github.com/h5bp/html5-boilerplate)
* Check if the browser is outdated with [Outdated Browser](http://outdatedbrowser.com/)
* Build the project compressing the HTML and the CSS.


## Folder Structure

```
./
├──┐
│  ├─ node_modules // Will appear after installed the NPM packages
│  │  └─ // NPM packages
│  │
│  ├─ build // Folder with the builded project
│  │
│  ├─ public // Files for deployment
│  │  ├─ css
│  │  │  └─ // Public styles
│  │  │
│  │  ├─ fonts
│  │  │  └─ // Web Fonts
│  │  │
│  │  ├─ images
│  │  │  │
│  │  │  ├─ copyright // Images with copyright metadata
│  │  │  │
│  │  │  ├─ logos // Logos
│  │  │  │
│  │  │  └─ // Public images
│  │  │
│  │  ├─ js
│  │  │  └─ // Public scripts
│  │  │
│  │  ├─ lang
│  │  │  ├─ outdated_browser // Langs to outdated browser plugin
│  │  │  │
│  │  │  │
│  │  │  └─ // Langs to multilingue sites
│  │  │
│  │  ├─ .htaccess // Configuration for use on web servers running the Apache Web Server
│  │  │
│  │  ├─ 404.html // Page to 404 error
│  │  │
│  │  ├─ apple-touch-icon.png // Icon for Safari on iOS
│  │  │
│  │  ├─ crossdomain.xml // Permission to handle data across multiple domains
│  │  │
│  │  ├─ example.html // Simple page with example of the components
│  │  │
│  │  ├─ favicon.ico //Icon for address bar and bookmark
│  │  │
│  │  ├─ index.html
│  │  │
│  │  ├─ manifest.json //Provides information about an Chrome app https://developer.chrome.com/extensions/manifest
│  │  │
│  │  ├─ manifest.webapp //Provides information about an Firefox OS app https://developer.mozilla.org/pt-BR/Apps/Manifest
│  │  │
│  │  ├─ robots.txt //Give instructions about their site to search engines
│  │  │
│  │  └─ // HTML, PHP, etc Files
│  │
│  └─ src // Source files for the projects
│       ├─ images // Original imagens, don't compressed
│       │  │
│       │  ├─ sprite // Images to generate the sprite
│       │  │
│       │  ├─ svg-sprite // Svgs to generate the svg-sprite
│       │  │
│       │  └─ touch // Icons
│       │      │
│       │      ├─ chrome-touch-icon-192x192.png // Icon for Chrome on Android
│       │      │
│       │      ├─ icon-128x128.png // Icon for Firefox on FirefoxOS
│       │      │
│       │      ├─ tile.png // Tile icon for Win8
│       │      │
│       │      ├─ tile-wide.png // Wide tile icon for Win8
│       │      │
│       │      └─ // .jpg, .jpeg, .gif, .svg and .bmp to be compressed
│       │
│       ├─ scripts
│       │  │
│       │  ├─ angular // Development with AngularJS
│       │  │
│       │  ├─ dependencies
│       │  │  │
│       │  │  ├─ frameworks
│       │  │  │
│       │  │  ├─ libs
│       │  │  │
│       │  │  ├─ modules
│       │  │  │
│       │  │  └─ plugins
│       │  │
│       │  ├─ jquery
│       │  │  │
│       │  │  ├─ onread // Open and close elements of Jquery
│       │  │  │
│       │  │  └─ // Development with JQuery
│       │  │
│       │  ├─ settings
│       │  │  │
│       │  │  ├─ google_analytics.js // Settings to Analytics
│       │  │  │
│       │  │  └─ outdatedbrowser.js // Settings to Browser Outdated
│       │  │
│       │  └─ // Development with Pure Javascript, the files
│       │
│       └─ stylesheets
│            │
│            ├─ components //Styles used by external plugins
│            │
│            ├─ dependencies //Styles used by external plugins
│            │
│            ├─ helpers
│            │  │
│            │  ├─ functions
│            │  │  │
│            │  │  └ //
│            │  │
│            │  ├─ mixins
│            │  │  │
│            │  │  └ //
│            │  │
│            │  ├─ _functions.styl
│            │  │
│            │  ├─ _helpers.styl
│            │  │
│            │  ├─ _mixins.styl
│            │  │
│            │  ├─ _placeholders.styl
│            │  │
│            │  ├─ _sprite.styl
│            │  │
│            │  ├─ _svg-sprite.styl
│            │  │
│            │  └─ _variables.styl
│            │
│            ├─ media_queries
│            │
│            ├─ typography
│            │
│            ├─ _base.styl // Main Styles
│            │
│            └─ styles.scss // Base Sass file with imports
│
├─ .editorconfig // Settings of editorconfig plugin
├─ .jshintrc // JSHint configuration file
├─ bower.json // Bower dependencies
├─ gulpfile.js // Gulp.js configuration file
├─ package.json // NPM dependencies
└─ README.md // Documentation
```

## Installing Dependencies

1. Install [EditorConfig](http://editorconfig.org/)

	* Download and install the [EditorConfig plugin](http://editorconfig.org/#download) for you text editor.

1. Download and install [Node.js](http://nodejs.org/download/)

	`Select npm package manager`


1. Install [Gulp.js](http://gulpjs.com/)

	* Open command line and execute

	```sh
	$ npm install gulp -g
	```

	For Mac or Linux User

	```sh
	$ sudo npm install gulp -g
	```

1. In Windows is necessary install [Ruby](https://www.ruby-lang.org/)

	* Download and install [Ruby](http://rubyinstaller.org/).

1. Install Gem [Sass](http://sass-lang.com/)

	* Open command line and execute

	```sh
	$ gem install sass
	```

1. Install [Bower](http://bower.io/)

	* Execute

	```sh
	$ npm install -g bower
	```

## Usage

1. Install [NPM](https://www.npmjs.com/) dependencies

	* In the command line go to the local folder

	```sh
	$ cd {yourFolderStructure}/swill-boilerplate
	```

	* Execute

	```sh
	$ npm install
	```

1. Open the file `bower.json`
	* Remove the dependencies that you will not use.

1. Open the command line
	* Go to the local folder

	```sh
	$ cd {yourFolderStructure}/swill-boilerplate
	```

1. Install [Bower](http://bower.io/) Dependencies
	* Execute

	```sh
	$ bower install
	```

	```sh
	$ gulp bower
	```

1. Execute the task `gulp` to start the development

```sh
$ gulp
```

### Tasks

Execute to build the project

```sh
$ gulp gulp
```

```sh
$ gulp compile
```

```sh
$ gulp build
```

```sh
$ gulp build:serve
```

### AngulaJS

To use Angular go to the `gulpfile.js` uncomment the lines with `mangle: false`.

### BrowserSync

If you will work with dinamic files like .php, it's necessary make changes in `gulpfile.js` to BrowserSync works

Remove the lines
```javascript
server: {
	baseDir: [basePaths.src, basePaths.dest]
}
```
Set the url to the server
```javascript
proxy: "localhost/swill-boilerplate/public/"
```

### Bitmap Sprite

This template uses [gulp.spritesmith](https://www.npmjs.org/package/gulp.spritesmith) to generate sprites.

When the sprite is generated, a file `_sprite.sass` is created with four mixins and the variables of the parameters of the images, like height and width (the names of the variables is same of the original file before the compilation).

**`_sprite.sass` example**

```sass

$left-arrow-x: 0px;
$left-arrow-y: 0px;
$left-arrow-offset-x: 0px;
$left-arrow-offset-y: 0px;
$left-arrow-width: 32px;
$left-arrow-height: 32px;
$left-arrow-total-width: 32px;
$left-arrow-total-height: 66px;
$left-arrow-image: '../images/sprite.png';

@mixin sprite-width($sprite) {
  width: nth($sprite, 5);
}

@mixin sprite-height($sprite) {
  height: nth($sprite, 6);
}

@mixin sprite-position($sprite) {
  $sprite-offset-x: nth($sprite, 3);
  $sprite-offset-y: nth($sprite, 4);
  background-position: $sprite-offset-x  $sprite-offset-y;
}

@mixin sprite-image($sprite) {
  $sprite-image: nth($sprite, 9);
  background-image: url(#{$sprite-image});
}

@mixin sprite($sprite) {
  @include sprite-image($sprite);
  @include sprite-position($sprite);
  @include sprite-width($sprite);
  @include sprite-height($sprite);
}
```

Just use the mixins with the variables as parameters.

**Example**

```sass
#arrow
	sprite($left-arrow)

	&:hover
		sprite-position($right-arrow)
```

**Output**

```css
#arrow {
	background-image: url(../images/sprite.png);
	background-position: 0px 0px;
	width: 32px;
	height: 32px;
}
#arrow:hover {
	background-position: 0px -34px;
}
```

### Svg Sprite


## License

Swill Boilerplate is released under the terms of the [MIT license](http://opensource.org/licenses/MIT).