# Fountain Angular 1 Generator

[![Angular 1](http://fountainjs.io/assets/imgs/angular1.png)](https://docs.angularjs.org/guide)

> This Yeoman generator allows you to start an Angular1 web app with the best Developer Experience out of the box!

> No matter what framework or module management you want to use, we got you covered with a cutting edge working configuration.

> We use [Gulp 4](http://gulpjs.com/) as a task manager but we'll ask you questions about:
- Modules management: Webpack, SystemJS, none
- JS preprocessor: Babel, TypeScript, none
- CSS preprocessor: Sass, Stylus, Less, none

## Generator Fountain Angular 1 structure

To take profit of the best of the Yeoman infrastructure, we heavily relies on the composability natures of the generators.

Thereby, each needs of your future application will be addressed by a dedicated Yeoman generator (each will be used depending of the options you selected or not).


## Usage

### Requirement Node 6+ && NPM 3+
This generator is targeted to be used with Node >= 6.0.0 and NPM => 3.0.0. You can check your version number with the command
```
node --version && npm --version
```

### Install

##### Install required tools `yo`:
```
npm install -g yo
```

##### Install `generator-fountain-angular1`:
```
npm install -g generator-fountain-angular1
```


### Run

##### Create a new directory, and go into:
```
mkdir my-new-project && cd my-new-project
```

##### Run `yo fountain-angular1`, and select desired technologies:
```
yo fountain-angular1
```
#### Use NPM scripts

- `npm run build` to build an optimized version of your application in /dist
- `npm run serve` to launch a browser sync server on your source files
- `npm run serve:dist` to launch a server on your optimized application
- `npm run test` to launch your unit tests with Karma
- `npm run test:auto` to launch your unit tests with Karma in watch mode


#### Or Gulp tasks

If you have [`gulp-cli`](https://www.npmjs.com/package/gulp-cli) installed in global packages you can use equivalent:

- `gulp` or `gulp build`
- `gulp serve`
- `gulp serve:dist`
- `gulp test`
- `gulp test:auto`

**If you don't have [`gulp-cli`](https://www.npmjs.com/package/gulp-cli) installed in global, you should have this error:**
> /usr/local/lib/node_modules/gulp/bin/gulp.js:121
    gulpInst.start.apply(gulpInst, toRun);
TypeError: Cannot read property 'apply' of undefined

### Sub-generators

Few sub-generators are available. You can see the full list by running `yo --generators`.  
Each generator has 2 options:
- You can set the name of the generated item with `--name`
- You can set the path of the generated item with `--dir`

**Example:**

```
yo fountain-angular1:component --name myComponent --dir components/game
