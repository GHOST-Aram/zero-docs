## class `HTTPErrors`
The `HTTPErrors` class encapsulates methods used to handle `404` and `500` status errors.

This class does not implement a constructor.

The module exports the class and an isntance of the class. The exports can be imported as follows:

```typescript

import { HTTPErrors } from 'zero/http'
import { httpErrors } from 'zero/http'

```
*NPM Dependencies*
* `express`
* `@types/express`

The following methods are implemented in the `HTTPErrors` class.

### 1. `handleUnknownUrls()`

Parameters:
* `req`: `Request` -  Express Request Object
* `res`: `Response` -  Express Response Object
* `next`: `NextFunction` -  Express NextFunction

Returns: 
* `void`


### 2. `handleServerErrors()`

Parameters:
* `req`: `Request` -  Express Request Object
* `res`: `Response` -  Express Response Object
* `next`: `NextFunction` -  Express NextFunction

Returns: 
* `void`
