
# SCSS Form Reset

SASS Mixins/Placeholders to reset all form elements
Forked from `https://gist.github.com/mjlescano/fc472f778e77c4b760ab`

## Table of contents

- [Install](#install)
- [Usage](#usage)
- [License](#license)
- [Credits](#credits)


## Instalation

Download `_form-reset.scss` or install via [NPM](https://www.npmjs.com/) `npm install scss-form-reset --save`

Then, import `_form-reset.scss` depending of your configuration and file structure.

* `@import "~scss-form-reset";` with [sass-loader](https://github.com/webpack-contrib/sass-loader) or [node-sass-package-importer](https://github.com/maoberlehner/node-sass-package-importer) **(recommended)**
* `@import "sass-form-reset/form-reset";` when using node-sass’ `includePaths` to resolve `node_modules` dir
* `@import "./../../node_modules/sass-form-reset/form-reset";` if none of the above and working in something like `./src/scss/main.scss`
* `@import "vendor/form-reset";` if manually copied `_form-reset.scss` in a `vendor` folder, for example


## Usage

MIXINS: for very specific use cases, when you don't want to reset absolutly all the forms, very verbose output.

PLACEHOLDER SELECTORS: use as extending classes. Less verbose, more generic overrides.

```scss
input {
  @extend %form-reset-input;
}

label {
  @extend %form-reset-label;
}

select {
  @extend %form-reset-select;
}

button {
  @extend %form-reset-button;
}

textarea {
  @extend %form-reset-textarea;
}
```


## License

SCSS Form Reset is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

## Credits

[Anthony Short](https://github.com/anthonyshort)

[Matías Lescano](https://github.com/mjlescano)
