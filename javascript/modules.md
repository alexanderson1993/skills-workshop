# Modules

There are two ways to use modules in JavaScript, with varying levels of support

# CommonJS

`module.exports.myModule = {}`;

or 

`module.exports = {}`;

then

`const myModule = require('module-package').myModule;`

or

`const myModule = require('module-package');`


# `import/export` or the ES2015 Standard

`export myModule;`

or

`export default myModule;`

then

`import {myModule} from 'module-package'; // Note the destructuring`

or 

`import Module from 'module-package'; // Named whatever I want`


> From my experience, module loading is still really complicated and volitile. In my opinion, best way on the server is to use `module.exports/require()` syntax. For the client, use Webpack with ES2015 `import/export` syntax.