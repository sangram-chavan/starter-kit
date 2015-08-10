# Starter Kit
Web project start kit including tooling, best practices and template seed.

It is based on our experience in large web projects, with architecture choices
aiming for a clean, no-brainer development experience even for beginner teams.

# Getting Started

1. Install required tools `gulp` and `bower`:
```
npm install -g gulp bower
```
2. Install project tools, go to project folder:
```
npm install
```
3. Launch development server:
```
gulp serve
```

# Project Structure
```
gulp/                   individual gulp tasks
sources/                project source code
|- data/                other project data, will be copied as-is
|- fonts/               project fonts
|- images/              project images
|- libraries/           bower libraries
|- main/                main module, for entry points and global style
|  |- main.js           js entry point
|  +- main.less         style entry point
|- modules/             project components and modules
|  |- helpers/          helper services
|  |- screens/          application screens
|  |- shell/            application shell
|  |- ui-components/    shared UI components
|  |- web-services/     web services
|  |- wrappers/         AngularJS module wrappers for external librairies
|  +- ...               additional project modules
|- translations/        translations files
+- index.html           html entry point
e2e/                    end-to-end tests
dist/                   compiled version
```

# Main Tasks

TODO

# Coding Guide

TODO: naming conventions, code style, best pratices, pitfalls

- [JavaScript](docs/js-guide.md)
- [CSS](docs/css-guide.md)
- [HTML](docs/html-guide.md)


# Additional Documentation
- [Proxy configuration](docs/proxy.md)
- [All gulp tasks](docs/tasks.md)

# Features

## Languages
- [TypeScript](http://www.typescriptlang.org), JavaScript
- [Less](http://lesscss.org), CSS
- [Jade](http://jade-lang.com), HTML
- [Gettext](https://angular-gettext.rocketeer.be) (for translations)

## Quality
- [TSLint](https://github.com/palantir/tslint)
- [JSHint](http://jshint.com)
- [JSCS](http://jscs.info)
- Unit tests ([Jasmine](http://jasmine.github.io))
- End-to-end tests ([Protractor](https://github.com/angular/protractor))

## Development
- Automation with [gulp](http://gulpjs.com)
- Development server with API proxy and live reload
  ([BrowserSync](http://www.browsersync.io))
- [JSDoc](http://usejsdoc.org) generation with angular support

## Build
- JS+CSS+HTML bundling and minification (useref, uglify, minify-html, csso) 
- CSS browser support (autoprefixer)
- Images optimization (imagemin)
- Automatic angular module annotation (ngAnnotate)
- Asset revisionning (rev)

## Libraries
- [AngularJS](https://angularjs.org)
- [Angular-gettext](https://angular-gettext.rocketeer.be)
- [AngularUI Router](https://github.com/angular-ui/ui-router)
- [UI Bootsrap](https://angular-ui.github.io/bootstrap)
- [Bootstrap](http://getbootstrap.com)
- [Font Awesome](http://fortawesome.github.io/Font-Awesome)
- [Lodash](https://lodash.com)

# Roadmap

## v1
- Add coding guides with best practices
- Improve project template
- Add default components (for logging, REST, data dependencies...)

## v2
- Mobile version (Cordova + ngCordova, Ionic, Crosswalk...)
- Add Sass support
- Custom icons management (font icons or SVG->CSS icons)

## v3
- Improve documentation (micro training, cheat sheets, posters...)
- Add bower package [cleaning](https://github.com/braddenver/preen)
- Npm dependencies flattening to ease usage on Windows platforms
- Repository for common base components?
- Consider integration with yeoman?

# Credits

This starter kit was initially based on a seed generated by the 
[gulp-angular](https://github.com/Swiip/generator-gulp-angular) Yeoman generator.
