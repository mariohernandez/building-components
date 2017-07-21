# Building Components - Breaking it down
#### A sandbox project by [Mario Hernandez](http://mariohernandez.io).

This is a sandbox project that show how to break a page down into smaller pieces to
effectively build components.  Main goal of building components is to reduce code duplication by making components reusable across an entire site.

![Building Components](/dist/assets/components.png "Building Components")

---

## About the code
You will find all working files within the `/src` folder.  This project was built with Twig, which is a PHP templating system, but it can also be built with plain html, jekyll or handlebars.  Reason for using Twig was that this is the platform I use for buiding drupal themes.

All code changes get compiled into `/dist` by using gulp.  See commands below for compiling Sass, JS, Styleguide.

## Styleguide
This project uses [KSS Node](https://github.com/kss-node/kss-node), which facilitates creating a styleguide to catalog your components.  To view this project's styleguide go to http://localhost/components/dist/style-guide/. (change localhost to match your local path).

## Getting Started
If you haven't yet, install nvm:
https://github.com/creationix/nvm

### Clone or download this project

### Run the following commands from project's root directory

#### Use the right version of node with:
`nvm use`

_This command will look at your `.nvmrc` file and use the version node.js specified in it. This ensures all developers use the same version of node for consistency._

#### If that version of node isn't installed, install it with:
`nvm install`

#### Install npm dependencies with
`npm install`

_This command looks at `package.json` and installs all the npm dependencies specified in it.  Some of the dependencies include gulp, autoprefixer, gulp-sass and others._

#### Runs default task
`npm run build`

_This will run whatever the default task is._

#### Compiles Sass
`npm run compile`

_This will perform a one-time Sass compilation._

#### Runs the watch command
`npm run watch`

_This is ideal when you are doing a lot of Sass changes and you want to make sure every time a change is saved it automatically gets compiled to CSS_

#### Cleans complied directory
`npm run clean`

_This will perform a one-time deletion of all compiled files within the dist/ directory._
