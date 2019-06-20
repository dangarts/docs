Common build tools are webpack, gulp, and grunt. React projects commonly use webpack, though any build tool can be used.

Processes that are automated by build tools in a typical React app include:

Babel is used to transpile (or convert) next-generation JavaScript into a version that has better cross-browser support. When using Babel, developers write their code in one version of JavaScript, and Babel re-writes that JavaScript into another version of JavaScript that's loaded by the browser. Babel has to be run after every change to the source code. Build tools are generally set up to watch for changes to JavaScript files, and to run Babel when changes are detected.
ESLint is used to check for errors and to raise warnings in the source code.
PostCSS is used to make the CSS more cross-browser compatible.