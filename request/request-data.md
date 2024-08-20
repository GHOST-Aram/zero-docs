## `request-data` module

The request data module exports one function whose sole purpose is to extract user data and user input from request. 


The function can be imported as follows:

```typescript

import { getDataFromRequest } from 'zero/request/request-data'

```

*NPM Dependencies*
* `express`
* `@types/express`

The function signature is as follows:

### 1. `getDataFromRequest()`

Parameters:
* `req`: `Request` - Express request object.


Returns: 
* `RequestData` object - [RequestData](../interfaces/request-data.md) interface

