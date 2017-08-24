# Before Webpack

## This branch shows the project after the use of Webpack

- Using Webpack, we no longer have to worry about the order of the imports script files.
  - We can simply import the bundle.js script file that we specified the location of in package.json under the build script.
  - The build script `"build": "webpack src/js/app.js dist/bundle.js"` in package.json tells webpack our entry point is app.js and the destination is bundle.js in the new dist/ folder

- Its important to note that for Webpack to work correctly, we need to make Webpack aware of our dependencies by exporting 'components', 'variables', 'functions' etc and then importing them to the places that we use them.
  - ex. In dom-loader.js, both var holding the DOM elements are exported, and then we import the two DOM elements in app.js.
    - Since app.js is specified as the entry point, webpack will begin looking there when it builds its dependency graph
