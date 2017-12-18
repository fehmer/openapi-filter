# openapi-filter

Filter internal paths, operations, parameters, schemas etc from OpenAPI/Swagger definitions

Simply tag any object within the definition with an `x-internal` specification extension, and it will be removed from the output.

Works with OpenAPI/Swagger 2.0 and 3.0.x and AsyncAPI 1.x definitions.

```
Usage: openapi-filter [options] {infile} [{outfile}]

Options:
  -h, --help     Show help                                             [boolean]
  --version      Show version number                                   [boolean]
  -i, --inverse  output filtered elements only                         [boolean]
```

or 

```javascript
let openapiFilter = require('openapi-filter');
let options = {};
let res = openapiFilter.filter(obj,options);
```
