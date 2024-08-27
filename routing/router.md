## class `GhostRouter`

The class can be extended by the route handler classes in the app. Every class that extends the `GhostRouter` class should override the public method in the base class with custom implementation.

The class implements a `constructor` method that accepts the following params:

* `controller`: `Controller` - a class that implements the [`Controllable`](../bases/controllable.md)
* `authenticator`: `Authenticator ` An object of the [`Authenticator`](../auth/auth.md) class

The class can be imported as follows:

```typescript

import { GhostRouter } from 'zero/routing'

```

The `GhostRouter` class implements the [`AppRouter`](../interfaces/app-router.md) interface.

The class implements one method that should be overidden by it's subclass.

### 1. `registerRoutes()`

Parameters:
* None

Returns:
* `Router` -  an object of the Express [Router](https://expressjs.com/en/guide/routing.html).


