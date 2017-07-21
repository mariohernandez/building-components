# Building Components - Breaking it down
#### A sandbox project by [Mario Hernandez](http://mariohernandez.io).

This is a sandbox project that show how to break a page down into smaller pieces to
effectively build components.  Main goal of building components is to reduce code duplication by making components reusable across an entire site.

![Building Components](/dist/assets/components.png "Building Components")


## Breaker code
```html
<section class="breaker">
  <div class="breaker__hero">
    <img src='../assets/hero.png' alt='Alt text'>
  </div>

  <div class="breaker__top">
    <p class="eyebrow  breaker__eyebrow">Drupal Development</p>
    <h2 class="breaker__heading">Component main heading here</h2>
    <p class="breaker__intro">Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Aenean lacinia bibendum nulla sed consectetur. Cras mattis consectetur purus sit amet fermentum.</p>
  </div>

  <div class="breaker__cards">
    <article class="card breaker__card breaker__card--first">
      <span class="card__icon"><svg>...</svg></span>
      <h3 class="card__heading">Fully responsive content</h3>
      <p class="card__teaser">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.</p>
    </article>

    <article class="card breaker__card breaker__card">
      <span class="card__icon"><svg>...</svg></span>
      <h3 class="card__heading">Fully responsive content</h3>
      <p class="card__teaser">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.</p>
    </article>

    <article class="card breaker__card breaker__card--last">
      <span class="card__icon"><svg>...</svg></span>
      <h3 class="card__heading">Fully responsive content</h3>
      <p class="card__teaser">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus sagittis lacus vel augue laoreet rutrum faucibus dolor auctor.</p>
    </article>
  </div>
</section>
```
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
