# demo

## Create app
```
$ npm install -g @vue/cli
$ vue create vue-import-bootstrap
```

## Adding Bootstrap to a Vue CLI Project
```
npm i bootstrap jquery popper.js
```

### Add to src/main.js
````javascript
import 'bootstrap';
import 'bootstrap/dist/css/bootstrap.min.css';
import jQuery from 'jquery'
window.$ = window.jQuery = jQuery
````

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
