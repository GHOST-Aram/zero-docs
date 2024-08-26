## class `Validator`

The validator class build on top of the `express-validator` module and encapsulates methods for validating user input. The methods encapsulated in this class can be used to validate input data in the request body, url params and query params.

The class and its instance can be imported as follows:

```typescript

import { Validator } from 'zero/validation'
import { Validator } from 'zero/validation/validator'

```

*NPM Dependencies*
* [express-validator]
* [express]

The following methods are implemented in the validator class:

### 1. `validateObjectId()`

Parameters:

* `fieldName`: `string`, 
* `option`: `ValidationOption` - An object of the [ValidationOption](../interfaces/validation-option.md) interface

Returns:
* `ValidationChain` : [ValidationChain]()

### 2. `validateObjectIDArray()`

Parameters:

* `fieldName`: `string`, 
* `option`: `ValidationOption` - An object of the [ValidationOption](../interfaces/validation-option.md) interface

Returns:
* `ValidationChain` : [ValidationChain]()

### 3. `validateReferenceId()`

Parameters:

* `paramName`: `string`, 
* `option`: `ValidationOption` - An object of the [ValidationOption](../interfaces/validation-option.md) interface

Returns:
* `ValidationChain` : [ValidationChain]()

### 4. `validateName()`

Parameters:

* `fieldName`: `string`, 
* `option`: `ValidationOption` - An object of the [ValidationOption](../interfaces/validation-option.md) interface

Returns:
* `ValidationChain` : [ValidationChain]()

### 5. `validateNumber()`

Parameters:

* `fieldName`: `string`, 
* `option`: `ValidationOption` - An object of the [ValidationOption](../interfaces/validation-option.md) interface

Returns:
* `ValidationChain` : [ValidationChain]()

### 6. `validateReferenceName()`

Parameters:

* `paramName`: `string`, 
* `option`: `ValidationOption` - An object of the [ValidationOption](../interfaces/validation-option.md) interface

Returns:
* `ValidationChain` : [ValidationChain]()

### 7. `validateNameField()`

Parameters:

* `fieldName`: `string`, 
* `option`: `ValidationOption` - An object of the [ValidationOption](../interfaces/validation-option.md) interface

Returns:
* `ValidationChain` : [ValidationChain]()

### 8. `validateBooleanField()`

Parameters:

* `field`: `string`, 
* `option`: `ValidationOption` - An object of the [ValidationOption](../interfaces/validation-option.md) interface

Returns:
* `ValidationChain` : [ValidationChain]()

### 9. `validateBooleanQuery()`

Parameters:
* `field`: `string`, 

Returns:
* `ValidationChain` : [ValidationChain]()

### 11. `validateNumberQuery()`

Parameters:
* `field`: `string`, 

Returns:
* `ValidationChain` : [ValidationChain]()

### 12. `validateStringQuery()`

Parameters:
* `field`: `string`, 

Returns:
* `ValidationChain` : [ValidationChain]()

### 14. `validateString()`

Parameters:

* `fieldName`: `string`, 
* `option`: `ValidationOption` - An object of the [ValidationOption](../interfaces/validation-option.md) interface

Returns:
* `ValidationChain` : [ValidationChain]()

### 15. `validateDescription()`

Parameters:

* `field`: `string`, 
* `option`: `ValidationOption` - An object of the [ValidationOption](../interfaces/validation-option.md) interface

Returns:
* `ValidationChain` : [ValidationChain]()

### 16. `validateFile()`

Parameters:
* `req`: `Request` - Express `Request`
* `res`: `Response` - Express `Response`
* `next`: `NextFunction` - Express `NextFunction`

Returns:
* `Response` or `undefined`

### 17. `validateFiles()`

Parameters:
* `req`: `Request` - Express `Request`
* `res`: `Response` - Express `Response`
* `next`: `NextFunction` - Express `NextFunction`

Returns:
* `Response` or `undefined`

### 18. `rejectEmptyDataObject()`

Parameters:
* None

Returns:
* `ValidationChain` : [ValidationChain]()

### 19. `rejectUnwantedPaths()`

Parameters:
*  `acceptedPaths`: `string`[]

Returns:
* `ValidationChain` : [ValidationChain]()


### 20. `handleValidationErrors()`

Parameters:
* `req`: `Request` - Express `Request`
* `res`: `Response` - Express `Response`
* `next`: `NextFunction` - Express `NextFunction`

Returns:
* `void`

