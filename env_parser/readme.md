# ENV PARSER

Util that loads environment variables from a .env file into process.env.

## Usage

```javascript
/**
 * Load environment variables
 */
const LoadEnv = require('./[path_to]/envLoader');

const parsedObject = LoadEnv.load({
    path: 'path_to_env_file',
});

console.log(parsedObject);
console.log(process.env)
```

### Env file format

Create a *env* file with *.env* extension (ie. *prod.env*) and add environment-specific variables on new lines in the form of **NAME=VALUE**

```
DB_HOST=localhost
DB_USER=root
DB_PASS=password
```
