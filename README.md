# Drupal Bootstrap

> A [Drupal 8](https://www.drupal.org) configuration with less boostrap for fast starting.

## Installation
Clone this repository in your www target folder

```bash
git clone https://github.com/CODEheures/drupalBootstrap.git my_target_folder
```

Install packages
```bash
$ composer install
```

Install [NodeJS](https://nodejs.org/en/) and after install LESS
```bash
$ npm install less -g
```

## CSS Personalisation
Adapt yours rules on /web/themes/contrib/codeheures/less/custom.less

Example:
```less
@import "../bootstrap/less/variables";
@container-lg: @container-large-desktop+150px;
h1 {
    color: red;
}
```

## CSS Compilation
Compile /web/themes/contrib/codeheures/less/style.less to  /web/themes/contrib/codeheures/css/style.css
```bash
$ cd /web/themes/contrib/codeheures/less
$ lessc style.less ../css/style.css
```

Optionaly:
- Use a file watcher (I personnaly use the intelliJ IDE with his own filewatcher)
- Use [livereload](http://livereload.com/) (Destock APP + Chrome extension)

## License

[Apache License 2.0](LICENSE) © [CODEheures](https://codeheures.fr/)