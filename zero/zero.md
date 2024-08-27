## class `Zero`

The `Zero` class builds on [`express`](https://expressjs.com/). The class encapsulates methods for configuring and setting up a Nodejs backend app. 

The class and it's instance can be imported as follows:

```typescript

import { zero } from 'zero/zero'
import { Zero } from 'zero/zero/zero'

```

*NPM Dependencies*
* express
* mongoose
* morgan
* cors

The following methods are encapsulated in the `Zero` class:

### 1. `initializePayloadParsers()`

Parameters:
* None

Returns:
* `void`

### 2. `allowCrossOriginResourceSharing()`

Parameters:
* None

Returns:
* `void`

### 3. `setUpSecurityMiddleware()`

Parameters:
* None

Returns:
* `void`

### 4. `setUpAuthenticator()`

Parameters:
* `secretOrKey`: `string`
* `authDbConnection`: `Connection` - mongoose [Connection](https://mongoosejs.com/docs/api/connection.html) object.

Returns:
* `void`

### 5. `logRequestsandResponses()`

Parameters:
* None

Returns:
* `void`

### 6. `listenToRequests()`

Parameters:
* `port`: `number` 
* `appName`: `string`

Returns:
* `void`

### 7 `configureRouter()`

Parameters:
* `config`: `RouterConfig` -  An object of the [RouterConfig](../interfaces/router-config.md) interface

Returns:
* `Router` - an object of the Express [Router](https://expressjs.com/en/guide/routing.html).

### 8. `configureUrls()`

Parameters:
* `routesMetadata`: `URLMetadata`[] - an array containing objects of the [URLMetadata](../interfaces/url-metadata.md) interface

Returns:
* `void`

### 9. `handleServerErrors()`

Parameters:
* None

Returns:
* `void`

### 10. `handleUnknownUrls()`

Parameters:
* None

Returns:
* `void`
