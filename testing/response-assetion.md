## class `ResponseAssertion`

The `ResponseAssertion`  class is built on [`jest`](https://jestjs.io/) and [`supertest`](https://www.npmjs.com/package/supertest) modules. The class encapsulates methods for testing responses. 

The class and it's instance can be imported as follows:

```typescript

    import { ResponseAssertion } from 'zero/testing/response-assertion'
    import { assert } from 'zero/testing/response-assertion'
    
```

*NPM Dependencies*
* jest
* supertest
* @jest/globals

The class encapsulates the following methods:

### 1. `respondsWithMethodNotAllowed()`

Parameters:
* `response`: `Response` -  Response object from supertest

Tests:
* status code `405`

Returns:
* `void`

### 2. `respondsWithConflict()`

Parameters:
* `response`: `Response` -  Response object from supertest

Tests:
* status code `409`

Returns:
* `void`

### 3. `respondsWithBadRequest()`

Parameters:
* `response`: `Response` -  Response object from supertest

Tests:
* status code `400`

Returns:
* `void`

### 4. `respondsWithValidationErrors()`

Parameters:
* `response`: `Response` -  Response object from supertest

Tests:
* Errors array in the response body

Returns:
* `void`

### 5. `respondsWithCreatedResource()`

Parameters:
* `response`: `Response` -  Response object from supertest

Tests:
* status code `201`
* `_id` property in the response payload
* resource url in the `response.header.location`

Returns:
* `void`

### 6. `respondsWithAllDataProperties()`

Paramters:
* `properties`: `string`[]
* `response`: `Response` -  Response object from supertest

Tests:
* Presence of all expected properties in the response payload.

Returns:
* `void`

### 7. `respondsWithNotFound()`

Parameters:
* `response`: `Response` -  Response object from supertest

Tests:
* status code 404

Returns:
* `void`

### 8. `respondsWithFoundResource()`

Parameters:
* `response`: `Response` -  Response object from supertest

Tests:
* status code `200`
* an object in the response body
* a property `_id` in the response body

Returns:
* `void`

### 9. `respondsWithEmptyResourceArray()`

Parameters:
* `response`: `Response` -  Response object from supertest

Tests:
* Response body has an array of length 0

Returns:
* `void`

### 10. `respondsWithPaginatedResource()`

Parameters:
* `response`: `Response` -  Response object from supertest
* `limit`: `number` - Pagination limit

Tests:
* Lenght of the resource array in the response body is equal to `limit`

Returns:
* `void`

### 11. `respondsWithItemsArray()`

Parameters:
* `response`: `Response` -  Response object from supertest

Tests:
* Response body contains array payload.

Returns:
* `void`

### 12. `respondsWithModifedResource()`

Parameters: 
* `response`: `Response` -  Response object from supertest

Tests:
* `_id` property in the response payload
* resource url in the `response.header.location`

Returns:
* `void`

### 13. `respondsWithUpdatedResource()`

Parameters: 
* `response`: `Response` -  Response object from supertest

Tests:
* `_id` property in the response payload
* resource url in the `response.header.location`

Returns:
* `void`

### 14. `respondsWithSuccess()`

Parameters: 
* `response`: `Response` -  Response object from supertest

Tests:
* status code `200`

Returns:
* `void`

### 15. `respondsWithDeletedResource()`

Parameters:
* `response`: `Response` -  Response object from supertest

Tests:
* item Id in the response body

Returns:
* `void`

### 16. `respondsWithToken()`

Parameters:
* `response`: `Response` -  Response object from supertest

Tests:
* status code `201`
* Jsonwebtoken in the response body

Returns:
* `void`

### 17. `respondsWithUnathorised()`

Parameters:
* `response`: `Response` -  Response object from supertest

Tests:
* status code `401`

Returns:
* `void`

### 18. `respondsWithForbidden()`

Parameters:
* `response`: `Response` -  Response object from supertest

Tests:
* status code `403`

Returns:
* `void`
