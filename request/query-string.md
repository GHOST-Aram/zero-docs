## class `QueryString`
The `QueryString` class encapsulates methods that manage the data from request query params. 

The class and it's instance can be imported as expressed below:

```javascript

import { QueryString } from 'zero/request'
import { queryString } from 'zero/request'
```

*NPM Dependencies*
* None

The following methods are implemented in the `QueryString` class:

### 1. `createSearchDocument()`

Parameters:
* `query`:`ParsedQs`
* `searchablePaths`: `string`[]

Returns:
* `Object` literal

### 2. `getPaginationParams()`

Parameters: 
* `query`: `ParsedQs`

Returns:
* `Paginator` an object of the [`Paginator`](../interfaces/paginator.md) interface.