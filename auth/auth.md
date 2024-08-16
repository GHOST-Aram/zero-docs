# auth module
The auth module includes an Authenticator class. The class includes methods for configuration authentication strategy, initializing authentication, controlling authorization and other methods related to user authentication and authorization.

The module exports the following.

`Authenticator` as a class.
`authenticator` as an instance of the authenticator class.

The exports can be imported as follows:
```typescript

import Authenticator from 'zero/auth/auth'
import { Authenticator } from 'zero/auth'
import { authenticator } from 'zero/auth'
import { createTokenPayload } from 'zero/auth'
```

*NPM Dependencies:*
* `passport`
* `passport-jwt`
* `jsonwebtoken`


The Authenticator class includes the following methods:

**`Authenticator.configureStrategy()`** 

This method configure authentication by JWT tokens.

The method accepts two parameters 

* `secretOrKey`: `string` - The secret key for decrypting JWT tokens.
* `authDbConnection`: `mongoose.Connection` - An actvie `Mongoose.Connection` object for accessing the database.

Returns `void`.

**`Authenticator.initialize()`**

Initializes the authentication middleware. The method accepts one parameter named below.

* `app`: `Express.Application`

Returns `void`.

**`Authenticator.authenticate()`**

Returns a JWT authentication middleware that allows only users with valid JWT tokens to access the system. 

Parameters:
* None

Returns: `passport.Authenticator.authenticate` - A route handler middleware.

**`Authenticator.restrictAccess()`**
An authorization control method that allows only users that meet a specific condition to access the part of the system that requires restricted access. The access condition is evaluated by a developer-defined utility callback fuction that returns a `boolean` value. 

Parameters:
* `allowThisUserGroup:(user: any) => boolean`: A utility function that accepts a user object, checks if user meets a certain condition and returns `true` or `false`.

Returns:
* `(req: Request, res: Response, next: NextFunction) => void`: An Express request handler middleware.

**`Authenticator.createTokenPayload()`**
Accepts a user object and creates a minimised object with important but less sensitive user data. The user data returned is used in another authentication apps as token payload. 

Parameters:
* `user`: `ZeroUser` -  any user object that extend the [`ZeroUser`](../interfaces/zero-user.md) interface. 

Returns:
`TokenPayload`: An object that matches the [`TokenPayload`](../interfaces/token-payload.md) interface.



