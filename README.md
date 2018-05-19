[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg)](http://standardjs.com)

<image src="https://user-images.githubusercontent.com/5190217/30834260-b90148f8-a228-11e7-8682-d09df8721da4.png" width="300">
<image src="http://static1.squarespace.com/static/57bf65a78419c24a012e3072/t/589a223520099e1857157ff0/1486496312107/white_background_logo.png?format=1000w" width="300">

# Envronment Leap JS

TO DO


## Getting started

Run dev server

```shell
npm run start
# or
yarn start
```

After run dev server: [localhost:8884](http://localhost:8884)


Run build:

```shell
npm run build
# or
yarn build
```

Every built file will be in `/public` folder


## Project structure

```
/src
  /assets
  /elements
  /javascripts
  /layouts
/config
  /scripts
  /webpack
/public
```

* `src` where all scene have to stay. Each `.tmpl` page is a scene
  * `assets` static files (images, videos, 3d models etc)
  * `elements` Nunjucks macros. Reusable elements like a `room` or `hand controls`
  * `javascripts` I think the name is self explained
  * `layouts` Templates to be extended
* `config` project environment settings
  * `scripts` node tooling
  * `webpack` webpack environment setting files
* `public` webpack build target


## JavaScript

The main JavaScript file is `index.js`. Every script imported there will be executed on scene. You can change this setting in `config/webpack/config.js`.

As the project has Webpack and Babe, the ES6 (and a little of ES7) syntax is able to be applied. [A-FRAME components]() can be easily imported.

`src/javascripts/index.js`

```javascript
import aframe from 'aframe';
import aframeExtras from 'aframe-extras';
import aframePhysicsSystem from 'aframe-physics-system';

// your imports and scripts
```

--

Made with some :beers: by [@taltk9](https://github.com/taltk9) and [@gutofoletto](https://github.com/gutofoletto)
