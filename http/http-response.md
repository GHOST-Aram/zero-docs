## class `HttpResponse`

The `HttpResponse` class encapsulates methods that send HTTP responses with standard response codes.

The class declares one public field below that is initilized in the class `constructor`:

* `microserviceName`: `string` -  the name of the app that depends on this class.

The class can be imported as follows:

```javascript

import { HttpResponse } from 'zero/http'

```

*NPM Dependencies*
* `mongoose`
* `express`

The following methods are implemented in the `HttpResponse` class:

### 1. `respondWithMethodNotAllowed()`
This is a standard Express Route handler method

Parameters:
* `req`: `Request` - Express Request object
* `res`: `Response` - Express Response object

Returns:
* `void`

### 2. `respondWithConflict()`

Parameters: 
* `res`: `Response` - Express Response object

Returns:
* `void`

### 3. `respondWithCreatedResource()`

Parameters:
* `resource`: `any` -  A Javascript object 
* `res`: `Response` - Express Response object


Returns:
* `void`

### 4. `respondWithFoundResource()`

Parameters:
* `resource`: `Object`[]| `Object`
* `res`: `Response`


Returns:
* `void`

### 5. `respondWithNotFound()` 
Parameters:
* `res`: `Response`

Returns:
* `void`

### 6. `respondWithModifiedResource()`

Parameters:
* `item`: `HydratedDocument<any>`
* `res`: `Response`

Returns:
* `void`

### 7. `respondWithUpdatedResource()`

Parameters:
* `resource`: `HydratedDocument<any>`
* `res`: `Response`

Returns:
* `void`

### 8. `respondWithDeletedResource()`

Parameters:
* `id`: `string`
* `res`: `Response`

Returns: 
* `void`

### 9. `respondWithForbidden()`

Parameters:
* `res`: `Response`
* `reason`: `string`

Returns:
* `void`

### 10. `respondWithUnauthorised()`

Parameters:
* `res`: `Response`
* `reason`: `string`

Returns:
* `void`

### 11. `respondWithToken()`

Parameters:
* `token`: `JWT token`
* `res`: `Response`

Returns: 
* `void`




